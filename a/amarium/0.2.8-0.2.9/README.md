# Comparing `tmp/amarium-0.2.8.tar.gz` & `tmp/amarium-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amarium-0.2.8.tar", last modified: Tue Jan 23 10:59:17 2024, max compression
+gzip compressed data, was "amarium-0.2.9.tar", last modified: Wed Jan 24 18:23:34 2024, max compression
```

## Comparing `amarium-0.2.8.tar` & `amarium-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-23 10:59:17.620459 amarium-0.2.8/
--rw-r--r--   0 julian    (1000) julian    (1000)     3650 2024-01-23 10:59:17.620459 amarium-0.2.8/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)     3068 2024-01-23 10:07:20.000000 amarium-0.2.8/README.md
--rw-r--r--   0 julian    (1000) julian    (1000)      690 2024-01-23 10:59:03.000000 amarium-0.2.8/pyproject.toml
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-01-23 10:59:17.620459 amarium-0.2.8/setup.cfg
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-23 10:59:17.612458 amarium-0.2.8/src/
--rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-01-23 10:07:20.000000 amarium-0.2.8/src/__init__.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-23 10:59:17.616458 amarium-0.2.8/src/amarium/
--rw-r--r--   0 julian    (1000) julian    (1000)      462 2024-01-23 10:14:39.000000 amarium-0.2.8/src/amarium/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2803 2024-01-23 10:07:20.000000 amarium-0.2.8/src/amarium/checks.py
--rw-r--r--   0 julian    (1000) julian    (1000)      231 2024-01-23 10:07:20.000000 amarium-0.2.8/src/amarium/checks.pyi
--rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-01-23 10:07:20.000000 amarium-0.2.8/src/amarium/csv_utils.py
--rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-01-23 10:07:20.000000 amarium-0.2.8/src/amarium/csv_utils.pyi
--rw-r--r--   0 julian    (1000) julian    (1000)     5927 2024-01-23 10:07:20.000000 amarium-0.2.8/src/amarium/encryption.py
--rw-r--r--   0 julian    (1000) julian    (1000)      221 2024-01-23 10:07:20.000000 amarium-0.2.8/src/amarium/encryption.pyi
--rw-r--r--   0 julian    (1000) julian    (1000)    14320 2024-01-23 10:24:19.000000 amarium-0.2.8/src/amarium/utils.py
--rw-r--r--   0 julian    (1000) julian    (1000)      941 2024-01-23 10:07:20.000000 amarium-0.2.8/src/amarium/utils.pyi
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-23 10:59:17.616458 amarium-0.2.8/src/amarium.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)     3650 2024-01-23 10:59:17.000000 amarium-0.2.8/src/amarium.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      528 2024-01-23 10:59:17.000000 amarium-0.2.8/src/amarium.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-01-23 10:59:17.000000 amarium-0.2.8/src/amarium.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       19 2024-01-23 10:59:17.000000 amarium-0.2.8/src/amarium.egg-info/requires.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       17 2024-01-23 10:59:17.000000 amarium-0.2.8/src/amarium.egg-info/top_level.txt
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-23 10:59:17.616458 amarium-0.2.8/tests/
--rw-r--r--   0 julian    (1000) julian    (1000)     2296 2024-01-23 10:07:20.000000 amarium-0.2.8/tests/test_checks.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2097 2024-01-23 10:07:20.000000 amarium-0.2.8/tests/test_encryption.py
--rw-r--r--   0 julian    (1000) julian    (1000)    13965 2024-01-23 10:24:19.000000 amarium-0.2.8/tests/test_file_utils.py
--rw-r--r--   0 julian    (1000) julian    (1000)      514 2024-01-23 10:07:20.000000 amarium-0.2.8/tests/test_init_imports.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-24 18:23:34.150718 amarium-0.2.9/
+-rw-r--r--   0 julian    (1000) julian    (1000)     3650 2024-01-24 18:23:34.150718 amarium-0.2.9/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     3068 2024-01-23 10:07:20.000000 amarium-0.2.9/README.md
+-rw-r--r--   0 julian    (1000) julian    (1000)      690 2024-01-24 18:19:39.000000 amarium-0.2.9/pyproject.toml
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-01-24 18:23:34.150718 amarium-0.2.9/setup.cfg
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-24 18:23:34.150718 amarium-0.2.9/src/
+-rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-01-23 10:07:20.000000 amarium-0.2.9/src/__init__.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-24 18:23:34.150718 amarium-0.2.9/src/amarium/
+-rw-r--r--   0 julian    (1000) julian    (1000)      462 2024-01-23 10:14:39.000000 amarium-0.2.9/src/amarium/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2803 2024-01-23 10:07:20.000000 amarium-0.2.9/src/amarium/checks.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      231 2024-01-23 10:07:20.000000 amarium-0.2.9/src/amarium/checks.pyi
+-rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-01-23 10:07:20.000000 amarium-0.2.9/src/amarium/csv_utils.py
+-rw-r--r--   0 julian    (1000) julian    (1000)        0 2024-01-23 10:07:20.000000 amarium-0.2.9/src/amarium/csv_utils.pyi
+-rw-r--r--   0 julian    (1000) julian    (1000)     5927 2024-01-23 10:07:20.000000 amarium-0.2.9/src/amarium/encryption.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      221 2024-01-23 10:07:20.000000 amarium-0.2.9/src/amarium/encryption.pyi
+-rw-r--r--   0 julian    (1000) julian    (1000)    15436 2024-01-24 18:23:26.000000 amarium-0.2.9/src/amarium/utils.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      941 2024-01-23 10:07:20.000000 amarium-0.2.9/src/amarium/utils.pyi
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-24 18:23:34.150718 amarium-0.2.9/src/amarium.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)     3650 2024-01-24 18:23:34.000000 amarium-0.2.9/src/amarium.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)      528 2024-01-24 18:23:34.000000 amarium-0.2.9/src/amarium.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-01-24 18:23:34.000000 amarium-0.2.9/src/amarium.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       19 2024-01-24 18:23:34.000000 amarium-0.2.9/src/amarium.egg-info/requires.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       17 2024-01-24 18:23:34.000000 amarium-0.2.9/src/amarium.egg-info/top_level.txt
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-01-24 18:23:34.150718 amarium-0.2.9/tests/
+-rw-r--r--   0 julian    (1000) julian    (1000)     2296 2024-01-23 10:07:20.000000 amarium-0.2.9/tests/test_checks.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2097 2024-01-23 10:07:20.000000 amarium-0.2.9/tests/test_encryption.py
+-rw-r--r--   0 julian    (1000) julian    (1000)    15435 2024-01-24 18:22:28.000000 amarium-0.2.9/tests/test_file_utils.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      514 2024-01-23 10:07:20.000000 amarium-0.2.9/tests/test_init_imports.py
```

### Comparing `amarium-0.2.8/PKG-INFO` & `amarium-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarium
-Version: 0.2.8
+Version: 0.2.9
 Summary: Filesystem handling utilities
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amarium Version: 0.2.8 Summary: Filesystem handling
+Metadata-Version: 2.1 Name: amarium Version: 0.2.9 Summary: Filesystem handling
 utilities Author-email: "Julian M. Kleber"
 gmail.com> Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Requires-Dist: numpy Requires-Dist: cryptography # Amarium [![status-
```

### Comparing `amarium-0.2.8/README.md` & `amarium-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `amarium-0.2.8/pyproject.toml` & `amarium-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amarium"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Julian M. Kleber", email="julian.m.kleber@gmail.com" },
 ]
 description = "Filesystem handling utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `amarium-0.2.8/src/amarium/checks.py` & `amarium-0.2.9/src/amarium/checks.py`

 * *Files identical despite different names*

### Comparing `amarium-0.2.8/src/amarium/encryption.py` & `amarium-0.2.9/src/amarium/encryption.py`

 * *Files identical despite different names*

### Comparing `amarium-0.2.8/src/amarium/utils.py` & `amarium-0.2.9/src/amarium/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,20 +36,56 @@
         if os.path.isdir(file_name):
             continue
         else:
             delete_file(file_name)
 
 
 def read_file(file_name: str, encoding="ISO-8859-1") -> str:
+    """read contents of a file specified
+
+    Args:
+        file_name (str): path to file
+        encoding (str, optional): Encodings. Defaults to "ISO-8859-1".
+
+    Returns:
+        str: String with content
+    """
     with open(file_name, "r", encoding=encoding) as f:
         content = f.read()
     return content
 
 
-def write_file(content: str, file_name: str, encoding: str = "ISO-8859-1"):
+def write_list_to_file(
+    content_list: List[str], file_name: str, encoding: str = "ISO-8859-1"
+) -> None:
+    """Write a list to a file
+
+    Args:
+        content_list (List[str]): Content of list
+        file_name (str): Path to save file
+        encoding (str, optional): Encoding of the file written to disk. Defaults to "ISO-8859-1".
+    """
+
+    file_name = prepare_file_name_saving(file_name=file_name)
+    with open(file_name, "w", encoding=encoding) as file:
+        for line in content_list:
+            file.write(line)
+            file.write("\n")
+    logging.info("Wrote file to " + file_name)
+
+
+def write_file(content: str, file_name: str, encoding: str = "ISO-8859-1") -> None:
+    """Write a file with content to destination specified standard encoding is ISO-8859-1
+
+    Args:
+        content (str): string content to write into file
+        file_name (str): _description_
+        encoding (str, optional): _description_. Defaults to "ISO-8859-1".
+    """
+
     file_name = prepare_file_name_saving(file_name=file_name)
     with open(file_name, "w", encoding=encoding) as txt_file:
         txt_file.write(content)
     logging.info("Wrote file to " + file_name)
 
 
 def prepare_file_name_saving(
```

### Comparing `amarium-0.2.8/src/amarium/utils.pyi` & `amarium-0.2.9/src/amarium/utils.pyi`

 * *Files identical despite different names*

### Comparing `amarium-0.2.8/src/amarium.egg-info/PKG-INFO` & `amarium-0.2.9/src/amarium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amarium
-Version: 0.2.8
+Version: 0.2.9
 Summary: Filesystem handling utilities
 Author-email: "Julian M. Kleber" <julian.m.kleber@gmail.com>
 Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amarium Version: 0.2.8 Summary: Filesystem handling
+Metadata-Version: 2.1 Name: amarium Version: 0.2.9 Summary: Filesystem handling
 utilities Author-email: "Julian M. Kleber"
 gmail.com> Project-URL: Homepage, https://www.codeberg.org/cap_jmk/amarium.git
 Project-URL: Bug Tracker, https://www.codeberg.org/cap_jmk/amarium.git/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Requires-Dist: numpy Requires-Dist: cryptography # Amarium [![status-
```

### Comparing `amarium-0.2.8/src/amarium.egg-info/SOURCES.txt` & `amarium-0.2.9/src/amarium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amarium-0.2.8/tests/test_checks.py` & `amarium-0.2.9/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `amarium-0.2.8/tests/test_encryption.py` & `amarium-0.2.9/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `amarium-0.2.8/tests/test_file_utils.py` & `amarium-0.2.9/tests/test_file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     insert_string_in_file_name,
     remove_all_files_from_dir,
     prepare_file_name_saving,
     delete_all_files_in_dir,
     make_date_file_name,
     load_json_from_file,
     convert_str_to_bool,
+    write_list_to_file,
     make_full_filename,
     save_json_to_file,
     delete_empty_dir,
     search_subdirs,
     attach_slash,
     combine_dirs,
     delete_file,
@@ -25,14 +26,53 @@
     read_file,
     copy_dir,
 )
 
 from src.amarium.checks import check_make_file_name_suffix, check_make_dir
 
 
+def test_write_list_to_file(): 
+    
+    #base variables
+    prefix =  "./tests/empty_dir/"
+    file = "test_list.csv"
+    file_name = make_full_filename(prefix=prefix, file_name=file)
+    
+
+    #case1 
+    content_list = []
+    write_list_to_file(content_list=content_list, file_name=file_name)
+    content = read_file(file_name=file_name)
+    assert file in os.listdir(prefix)
+    assert content == "".join(content), str(content) + str("".join(content))
+    delete_file(file_name=file_name)
+    #case2 
+
+    content_list = ["A"]
+    write_list_to_file(content_list=content_list, file_name=file_name)
+    content = read_file(file_name=file_name)
+    assert file in os.listdir(prefix)
+    assert content == "".join(content), str(content) + str("".join(content))
+    delete_file(file_name=file_name)
+    #case 3 
+    content_list = ["A", "B"]
+    write_list_to_file(content_list=content_list, file_name=file_name)
+    content = read_file(file_name=file_name)
+    assert file in os.listdir(prefix)
+    assert content == "".join(content), str(content) + str("".join(content))
+    delete_file(file_name=file_name)
+    #case 4 
+    #file_existing
+    content_list = ["A", "B", "C"]
+    write_list_to_file(content_list=content_list, file_name=file_name)
+    content = read_file(file_name=file_name)
+    assert file in os.listdir(prefix)
+    assert content == "".join(content), str(content) + str("".join(content))
+    delete_file(file_name=file_name)
+
 def test_remove_files_directory():
     # case 1
     dir_name = "./tests/empty_dir/"
 
     remove_all_files_from_dir(dir_name)
     assert len(os.listdir(dir_name)) == 0
     # case 2
```

### Comparing `amarium-0.2.8/tests/test_init_imports.py` & `amarium-0.2.9/tests/test_init_imports.py`

 * *Files identical despite different names*

