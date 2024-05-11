# Comparing `tmp/rag_pychunk-1.0.2.tar.gz` & `tmp/rag_pychunk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_pychunk-1.0.2.tar", last modified: Fri May 10 16:50:10 2024, max compression
+gzip compressed data, was "rag_pychunk-1.0.3.tar", last modified: Sat May 11 16:07:28 2024, max compression
```

## Comparing `rag_pychunk-1.0.2.tar` & `rag_pychunk-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.868325 rag_pychunk-1.0.2/
--rw-r--r--   0 Jaime      (502) staff       (20)     1076 2024-05-10 11:33:20.000000 rag_pychunk-1.0.2/LICENSE
--rw-r--r--   0 Jaime      (502) staff       (20)       17 2024-05-08 16:43:09.000000 rag_pychunk-1.0.2/MANIFEST.in
--rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-10 16:50:10.868002 rag_pychunk-1.0.2/PKG-INFO
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.865102 rag_pychunk-1.0.2/pychunk/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-09 06:52:18.000000 rag_pychunk-1.0.2/pychunk/__init__.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.865430 rag_pychunk-1.0.2/pychunk/chunkers/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:40:23.000000 rag_pychunk-1.0.2/pychunk/chunkers/__init__.py
--rw-r--r--   0 Jaime      (502) staff       (20)     3157 2024-05-10 15:59:52.000000 rag_pychunk-1.0.2/pychunk/chunkers/base.py
--rw-r--r--   0 Jaime      (502) staff       (20)     9616 2024-05-10 15:52:23.000000 rag_pychunk-1.0.2/pychunk/chunkers/python_chunker.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.866125 rag_pychunk-1.0.2/pychunk/nodes/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:47:25.000000 rag_pychunk-1.0.2/pychunk/nodes/__init__.py
--rw-r--r--   0 Jaime      (502) staff       (20)     4205 2024-05-10 08:20:39.000000 rag_pychunk-1.0.2/pychunk/nodes/base.py
--rw-r--r--   0 Jaime      (502) staff       (20)     3070 2024-05-10 08:23:09.000000 rag_pychunk-1.0.2/pychunk/nodes/nodes.py
--rw-r--r--   0 Jaime      (502) staff       (20)      780 2024-05-10 11:18:52.000000 rag_pychunk-1.0.2/pychunk/nodes/types.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.866546 rag_pychunk-1.0.2/pychunk/utils/
--rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:45:35.000000 rag_pychunk-1.0.2/pychunk/utils/__init__.py
--rw-r--r--   0 Jaime      (502) staff       (20)      543 2024-05-09 08:16:14.000000 rag_pychunk-1.0.2/pychunk/utils/files_handler.py
--rw-r--r--   0 Jaime      (502) staff       (20)     7991 2024-05-10 10:46:57.000000 rag_pychunk-1.0.2/pychunk/utils/nodes_utils.py
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.867785 rag_pychunk-1.0.2/rag_pychunk.egg-info/
--rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-10 16:50:10.000000 rag_pychunk-1.0.2/rag_pychunk.egg-info/PKG-INFO
--rw-r--r--   0 Jaime      (502) staff       (20)      603 2024-05-10 16:50:10.000000 rag_pychunk-1.0.2/rag_pychunk.egg-info/SOURCES.txt
--rw-r--r--   0 Jaime      (502) staff       (20)        1 2024-05-10 16:50:10.000000 rag_pychunk-1.0.2/rag_pychunk.egg-info/dependency_links.txt
--rw-r--r--   0 Jaime      (502) staff       (20)        8 2024-05-10 16:50:10.000000 rag_pychunk-1.0.2/rag_pychunk.egg-info/top_level.txt
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.864585 rag_pychunk-1.0.2/scripts/
-drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-10 16:50:10.867576 rag_pychunk-1.0.2/scripts/python-scripts/
--rwxr-xr-x   0 Jaime      (502) staff       (20)     5374 2024-05-10 10:54:57.000000 rag_pychunk-1.0.2/scripts/python-scripts/classify-python-code.sh
--rwxr-xr-x   0 Jaime      (502) staff       (20)      788 2024-05-10 10:12:20.000000 rag_pychunk-1.0.2/scripts/python-scripts/find-node-relationships.sh
--rwxr-xr-x   0 Jaime      (502) staff       (20)     7163 2024-05-10 14:27:25.000000 rag_pychunk-1.0.2/scripts/python-scripts/generate-node-metadata.sh
--rw-r--r--   0 Jaime      (502) staff       (20)       38 2024-05-10 16:50:10.868379 rag_pychunk-1.0.2/setup.cfg
--rw-r--r--   0 Jaime      (502) staff       (20)     1716 2024-05-10 16:49:53.000000 rag_pychunk-1.0.2/setup.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.656921 rag_pychunk-1.0.3/
+-rw-r--r--   0 Jaime      (502) staff       (20)     1076 2024-05-10 11:33:20.000000 rag_pychunk-1.0.3/LICENSE
+-rw-r--r--   0 Jaime      (502) staff       (20)       17 2024-05-08 16:43:09.000000 rag_pychunk-1.0.3/MANIFEST.in
+-rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-11 16:07:28.656629 rag_pychunk-1.0.3/PKG-INFO
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.653416 rag_pychunk-1.0.3/pychunk/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-09 06:52:18.000000 rag_pychunk-1.0.3/pychunk/__init__.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.653749 rag_pychunk-1.0.3/pychunk/chunkers/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:40:23.000000 rag_pychunk-1.0.3/pychunk/chunkers/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     3157 2024-05-10 15:59:52.000000 rag_pychunk-1.0.3/pychunk/chunkers/base.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     9616 2024-05-10 15:52:23.000000 rag_pychunk-1.0.3/pychunk/chunkers/python_chunker.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.654312 rag_pychunk-1.0.3/pychunk/nodes/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:47:25.000000 rag_pychunk-1.0.3/pychunk/nodes/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     4177 2024-05-11 15:33:13.000000 rag_pychunk-1.0.3/pychunk/nodes/base.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     3070 2024-05-10 08:23:09.000000 rag_pychunk-1.0.3/pychunk/nodes/nodes.py
+-rw-r--r--   0 Jaime      (502) staff       (20)      780 2024-05-10 11:18:52.000000 rag_pychunk-1.0.3/pychunk/nodes/types.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.654744 rag_pychunk-1.0.3/pychunk/parser/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-11 15:34:39.000000 rag_pychunk-1.0.3/pychunk/parser/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     1511 2024-05-11 16:03:58.000000 rag_pychunk-1.0.3/pychunk/parser/langchain_parser.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     2169 2024-05-11 15:58:22.000000 rag_pychunk-1.0.3/pychunk/parser/llama_index_parser.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.655149 rag_pychunk-1.0.3/pychunk/utils/
+-rw-r--r--   0 Jaime      (502) staff       (20)        0 2024-05-08 16:45:35.000000 rag_pychunk-1.0.3/pychunk/utils/__init__.py
+-rw-r--r--   0 Jaime      (502) staff       (20)      543 2024-05-09 08:16:14.000000 rag_pychunk-1.0.3/pychunk/utils/files_handler.py
+-rw-r--r--   0 Jaime      (502) staff       (20)     7991 2024-05-10 10:46:57.000000 rag_pychunk-1.0.3/pychunk/utils/nodes_utils.py
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.656385 rag_pychunk-1.0.3/rag_pychunk.egg-info/
+-rw-r--r--   0 Jaime      (502) staff       (20)     1404 2024-05-11 16:07:28.000000 rag_pychunk-1.0.3/rag_pychunk.egg-info/PKG-INFO
+-rw-r--r--   0 Jaime      (502) staff       (20)      702 2024-05-11 16:07:28.000000 rag_pychunk-1.0.3/rag_pychunk.egg-info/SOURCES.txt
+-rw-r--r--   0 Jaime      (502) staff       (20)        1 2024-05-11 16:07:28.000000 rag_pychunk-1.0.3/rag_pychunk.egg-info/dependency_links.txt
+-rw-r--r--   0 Jaime      (502) staff       (20)        8 2024-05-11 16:07:28.000000 rag_pychunk-1.0.3/rag_pychunk.egg-info/top_level.txt
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.652880 rag_pychunk-1.0.3/scripts/
+drwxr-xr-x   0 Jaime      (502) staff       (20)        0 2024-05-11 16:07:28.656168 rag_pychunk-1.0.3/scripts/python-scripts/
+-rwxr-xr-x   0 Jaime      (502) staff       (20)     5374 2024-05-10 10:54:57.000000 rag_pychunk-1.0.3/scripts/python-scripts/classify-python-code.sh
+-rwxr-xr-x   0 Jaime      (502) staff       (20)      788 2024-05-10 10:12:20.000000 rag_pychunk-1.0.3/scripts/python-scripts/find-node-relationships.sh
+-rwxr-xr-x   0 Jaime      (502) staff       (20)     7163 2024-05-10 14:27:25.000000 rag_pychunk-1.0.3/scripts/python-scripts/generate-node-metadata.sh
+-rw-r--r--   0 Jaime      (502) staff       (20)       38 2024-05-11 16:07:28.656978 rag_pychunk-1.0.3/setup.cfg
+-rw-r--r--   0 Jaime      (502) staff       (20)     1716 2024-05-11 15:34:48.000000 rag_pychunk-1.0.3/setup.py
```

### Comparing `rag_pychunk-1.0.2/LICENSE` & `rag_pychunk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/PKG-INFO` & `rag_pychunk-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-pychunk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Improve your RAG pipelines for your python repositories.
 Author: Jaime Sancho Molero
 Author-email: jimysanchomolero@gmail.com
 License-File: LICENSE
 
 
     It leverages the python programming language syntax to improve:
```

### Comparing `rag_pychunk-1.0.2/pychunk/chunkers/base.py` & `rag_pychunk-1.0.3/pychunk/chunkers/base.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/pychunk/chunkers/python_chunker.py` & `rag_pychunk-1.0.3/pychunk/chunkers/python_chunker.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/pychunk/nodes/base.py` & `rag_pychunk-1.0.3/pychunk/nodes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,20 +77,20 @@
             self.__node_relationships[relationship_type] = {node.id: [line_of_occurence]}
         else: 
             if node.id in self.__node_relationships[relationship_type]: 
                 self.__node_relationships[relationship_type][node.id].append(line_of_occurence)
             else:
                 self.__node_relationships[relationship_type][node.id] = [line_of_occurence]
         
-    def filter_relationships(self, relationship_type: NodeRelationshipType) -> List[Tuple[Type['BaseNode'], int | None]] | List:
+    def filter_relationships(self, relationship_type: NodeRelationshipType) -> Dict[str, List[int]]:
         relationship_type = relationship_type.value
         filtered_relationships = [rel for rel_type, rel in self.__node_relationships.items() if rel_type == relationship_type]
         if len(filtered_relationships) > 0:
             return filtered_relationships[0]
-        return []
+        return {}
     
     def check_relationship(self, node: Type['BaseNode'], relationship_type: NodeRelationshipType) -> bool:
         try:
             return node.id in self.__node_relationships[relationship_type.value]
         except KeyError:
             return False
```

### Comparing `rag_pychunk-1.0.2/pychunk/nodes/nodes.py` & `rag_pychunk-1.0.3/pychunk/nodes/nodes.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/pychunk/nodes/types.py` & `rag_pychunk-1.0.3/pychunk/nodes/types.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/pychunk/utils/files_handler.py` & `rag_pychunk-1.0.3/pychunk/utils/files_handler.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/pychunk/utils/nodes_utils.py` & `rag_pychunk-1.0.3/pychunk/utils/nodes_utils.py`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/rag_pychunk.egg-info/PKG-INFO` & `rag_pychunk-1.0.3/rag_pychunk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag-pychunk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Improve your RAG pipelines for your python repositories.
 Author: Jaime Sancho Molero
 Author-email: jimysanchomolero@gmail.com
 License-File: LICENSE
 
 
     It leverages the python programming language syntax to improve:
```

### Comparing `rag_pychunk-1.0.2/scripts/python-scripts/classify-python-code.sh` & `rag_pychunk-1.0.3/scripts/python-scripts/classify-python-code.sh`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/scripts/python-scripts/find-node-relationships.sh` & `rag_pychunk-1.0.3/scripts/python-scripts/find-node-relationships.sh`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/scripts/python-scripts/generate-node-metadata.sh` & `rag_pychunk-1.0.3/scripts/python-scripts/generate-node-metadata.sh`

 * *Files identical despite different names*

### Comparing `rag_pychunk-1.0.2/setup.py` & `rag_pychunk-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rag-pychunk',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     scripts=['scripts/python-scripts/classify-python-code.sh', 
              'scripts/python-scripts/find-node-relationships.sh', 
              'scripts/python-scripts/generate-node-metadata.sh'],
     author="Jaime Sancho Molero", 
     author_email="jimysanchomolero@gmail.com", 
     description="Improve your RAG pipelines for your python repositories.",
```

