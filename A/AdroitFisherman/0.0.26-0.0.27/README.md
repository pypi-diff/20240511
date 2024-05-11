# Comparing `tmp/AdroitFisherman-0.0.26.tar.gz` & `tmp/AdroitFisherman-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdroitFisherman-0.0.26.tar", last modified: Mon May  6 13:15:33 2024, max compression
+gzip compressed data, was "AdroitFisherman-0.0.27.tar", last modified: Sat May 11 10:01:52 2024, max compression
```

## Comparing `AdroitFisherman-0.0.26.tar` & `AdroitFisherman-0.0.27.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.124081 AdroitFisherman-0.0.26/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.102141 AdroitFisherman-0.0.26/AdroitFisherman/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.117099 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/
--rw-rw-rw-   0        0        0      937 2024-05-06 10:26:31.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/CircularSingleLinkedList.py
--rw-rw-rw-   0        0        0      763 2024-05-06 09:36:54.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SequentialList.py
--rw-rw-rw-   0        0        0      903 2024-05-06 09:36:54.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedList.py
--rw-rw-rw-   0        0        0      942 2024-05-06 09:36:54.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
--rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.119093 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/
--rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
--rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.26/AdroitFisherman/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.120091 AdroitFisherman-0.0.26/AdroitFisherman/__pycache__/
--rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.26/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.123082 AdroitFisherman-0.0.26/AdroitFisherman/includes/
--rw-rw-rw-   0        0        0      834 2024-05-06 10:24:31.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/CircularSingleLinkedList.c
--rw-rw-rw-   0        0        0     8255 2024-05-06 13:15:10.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/CircularSingleLinkedList.h
--rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.c
--rw-rw-rw-   0        0        0     5147 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.h
--rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.c
--rw-rw-rw-   0        0        0     8093 2024-05-04 03:47:56.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.h
--rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
--rw-rw-rw-   0        0        0     9086 2024-05-04 05:59:20.000000 AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
-drwxrwxrwx   0        0        0        0 2024-05-06 13:15:33.108125 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/
--rw-rw-rw-   0        0        0     3192 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 13:15:33.000000 AdroitFisherman-0.0.26/AdroitFisherman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.26/MANIFEST.in
--rw-rw-rw-   0        0        0     3192 2024-05-06 13:15:33.124081 AdroitFisherman-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.26/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 13:15:33.126076 AdroitFisherman-0.0.26/setup.cfg
--rw-rw-rw-   0        0        0     1641 2024-05-06 10:23:43.000000 AdroitFisherman-0.0.26/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:01:52.903818 AdroitFisherman-0.0.27/
+drwxrwxrwx   0        0        0        0 2024-05-11 10:01:52.863924 AdroitFisherman-0.0.27/AdroitFisherman/
+drwxrwxrwx   0        0        0        0 2024-05-11 10:01:52.894842 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/
+-rw-rw-rw-   0        0        0     1034 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/CircularSingleLinkedList.py
+-rw-rw-rw-   0        0        0     1174 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/DoubleLinkedList.py
+-rw-rw-rw-   0        0        0      860 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/SequentialList.py
+-rw-rw-rw-   0        0        0     1000 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/SingleLinkedList.py
+-rw-rw-rw-   0        0        0     1039 2024-05-11 10:01:47.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
+-rw-rw-rw-   0        0        0       32 2024-04-29 14:08:58.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:01:52.896837 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/__pycache__/
+-rw-rw-rw-   0        0        0     1781 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
+-rw-rw-rw-   0        0        0      202 2024-04-29 14:15:36.000000 AdroitFisherman-0.0.27/AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0        0 2024-04-29 04:35:09.000000 AdroitFisherman-0.0.27/AdroitFisherman/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 10:01:52.897834 AdroitFisherman-0.0.27/AdroitFisherman/__pycache__/
+-rw-rw-rw-   0        0        0      166 2024-04-29 04:35:10.000000 AdroitFisherman-0.0.27/AdroitFisherman/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-05-11 10:01:52.902820 AdroitFisherman-0.0.27/AdroitFisherman/includes/
+-rw-rw-rw-   0        0        0      834 2024-05-06 10:24:31.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/CircularSingleLinkedList.c
+-rw-rw-rw-   0        0        0     8594 2024-05-11 09:48:35.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/CircularSingleLinkedList.h
+-rw-rw-rw-   0        0        0     1103 2024-05-11 09:23:06.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/DoubleLinkedList.c
+-rw-rw-rw-   0        0        0     9854 2024-05-11 09:37:50.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/DoubleLinkedList.h
+-rw-rw-rw-   0        0        0      720 2024-04-29 03:59:20.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/SeqList.c
+-rw-rw-rw-   0        0        0     5179 2024-05-11 09:55:01.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/SeqList.h
+-rw-rw-rw-   0        0        0     1103 2024-04-29 04:03:41.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedList.c
+-rw-rw-rw-   0        0        0     8383 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedList.h
+-rw-rw-rw-   0        0        0      883 2024-05-04 05:23:21.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
+-rw-rw-rw-   0        0        0     9370 2024-05-11 10:00:29.000000 AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
+drwxrwxrwx   0        0        0        0 2024-05-11 10:01:52.875893 AdroitFisherman-0.0.27/AdroitFisherman.egg-info/
+-rw-rw-rw-   0        0        0     3192 2024-05-11 10:01:52.000000 AdroitFisherman-0.0.27/AdroitFisherman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1402 2024-05-11 10:01:52.000000 AdroitFisherman-0.0.27/AdroitFisherman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 10:01:52.000000 AdroitFisherman-0.0.27/AdroitFisherman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-11 10:01:52.000000 AdroitFisherman-0.0.27/AdroitFisherman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      107 2024-04-25 11:08:16.000000 AdroitFisherman-0.0.27/MANIFEST.in
+-rw-rw-rw-   0        0        0     3192 2024-05-11 10:01:52.903818 AdroitFisherman-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2024-04-25 07:13:31.000000 AdroitFisherman-0.0.27/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 10:01:52.908804 AdroitFisherman-0.0.27/setup.cfg
+-rw-rw-rw-   0        0        0     1778 2024-05-11 09:42:45.000000 AdroitFisherman-0.0.27/setup.py
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/CircularSingleLinkedList.py` & `AdroitFisherman-0.0.27/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from AdroitFisherman.CircularSingleLinkedList import SingleLinkedList
+from AdroitFisherman.SingleLinkedListWithoutHeadNode import SingleLinkedList
 
 
 class ListObject:
     def __init__(self):
         self.__list = SingleLinkedList()
         self.__list.init_list()
 
@@ -31,7 +31,11 @@
         return self.__list.list_insert(index, elem)
 
     def list_delete(self, index):
         return self.__list.list_delete(index)
 
     def __del__(self):
         self.__list.destroy_list()
+
+    def __str__(self):
+        self.__list.traverse_list()
+        return "traverse result"
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SequentialList.py` & `AdroitFisherman-0.0.27/AdroitFisherman/Utilities/SingleLinkedList.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from AdroitFisherman.SequentialList import SeqList
+from AdroitFisherman.SingleLinkedList import List
 
 
 class ListObject:
-    def __init__(self, size):
-        self.__list = SeqList()
-        self.__list.init_list(size)
+    def __init__(self):
+        self.__list = List()
+        self.__list.init_list()
 
     def destroy(self):
         self.__list.destroy_list()
 
     def clear_list(self):
         self.__list.clear_list()
 
@@ -17,15 +17,25 @@
 
     def list_length(self):
         return self.__list.list_length()
 
     def get_elem(self, index):
         return self.__list.get_elem(index)
 
+    def add_first(self, elem):
+        return self.__list.add_first(elem)
+
+    def add_after(self, elem):
+        return self.__list.add_after(elem)
+
     def list_insert(self, index, elem):
         return self.__list.list_insert(index, elem)
 
     def list_delete(self, index):
         return self.__list.list_delete(index)
 
     def __del__(self):
         self.__list.destroy_list()
+
+    def __str__(self):
+        self.__list.traverse_list()
+        return "traverse result"
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedList.py` & `AdroitFisherman-0.0.27/AdroitFisherman/Utilities/CircularSingleLinkedList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from AdroitFisherman.SingleLinkedList import List
+from AdroitFisherman.CircularSingleLinkedList import SingleLinkedList
 
 
 class ListObject:
     def __init__(self):
-        self.__list = List()
+        self.__list = SingleLinkedList()
         self.__list.init_list()
 
     def destroy(self):
         self.__list.destroy_list()
 
     def clear_list(self):
         self.__list.clear_list()
@@ -30,8 +30,12 @@
     def list_insert(self, index, elem):
         return self.__list.list_insert(index, elem)
 
     def list_delete(self, index):
         return self.__list.list_delete(index)
 
     def __del__(self):
-        self.__list.destroy_list()
+        self.__list.destroy_list()
+
+    def __str__(self):
+        self.__list.traverse_list()
+        return "traverse result"
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py` & `AdroitFisherman-0.0.27/AdroitFisherman/Utilities/SequentialList.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from AdroitFisherman.SingleLinkedListWithoutHeadNode import SingleLinkedList
+from AdroitFisherman.SequentialList import SeqList
 
 
 class ListObject:
-    def __init__(self):
-        self.__list = SingleLinkedList()
-        self.__list.init_list()
+    def __init__(self, size):
+        self.__list = SeqList()
+        self.__list.init_list(size)
 
     def destroy(self):
         self.__list.destroy_list()
 
     def clear_list(self):
         self.__list.clear_list()
 
@@ -17,21 +17,19 @@
 
     def list_length(self):
         return self.__list.list_length()
 
     def get_elem(self, index):
         return self.__list.get_elem(index)
 
-    def add_first(self, elem):
-        return self.__list.add_first(elem)
-
-    def add_after(self, elem):
-        return self.__list.add_after(elem)
-
     def list_insert(self, index, elem):
         return self.__list.list_insert(index, elem)
 
     def list_delete(self, index):
         return self.__list.list_delete(index)
 
     def __del__(self):
-        self.__list.destroy_list()
+        self.__list.destroy_list()
+
+    def __str__(self):
+        self.__list.traverse_list()
+        return "traverse result"
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc` & `AdroitFisherman-0.0.27/AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/CircularSingleLinkedList.c` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/CircularSingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/CircularSingleLinkedList.h` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/CircularSingleLinkedList.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #ifndef CIRCULARSINGLELINKEDLIST_H_INCLUDED
 #define CIRCULARSINGLELINKEDLIST_H_INCLUDED
 #define TRUE 1
 #define FALSE -1
 typedef PyObject* ElemType;
 typedef struct Node
 {
+    PyObject_HEAD
     ElemType elem;
     struct Node* next;
 }LNode;
 typedef struct {
+    PyObject_HEAD
     LNode* instance;
 }List;
 static void LNode_destroy(LNode* self)
 {
     Py_DECREF(self->elem);
     Py_DECREF(self->next);
     Py_TYPE(self)->tp_free(self);
@@ -279,25 +281,37 @@
         del = p->next;
         p->next = del->next;
         PyMem_FREE(del);
         del = NULL;
         Py_RETURN_TRUE;
     }
 }
+static PyObject* TraverseList(List* self, PyObject* args)
+{
+    LNode *p=self->instance->next;
+    while(p!=self->instance)
+    {
+        PyObject_Print(p->elem,stdout,0);
+        p=p->next;
+    }
+    printf("\n");
+    Py_RETURN_NONE;
+}
 static PyMethodDef List_methods[] = {
     {"init_list",InitList,METH_VARARGS,""},
     {"destroy_list",DestroyList,METH_VARARGS,""},
     {"clear_list",ClearList,METH_VARARGS,""},
     {"list_empty",ListEmpty,METH_VARARGS,""},
     {"list_length",ListLength,METH_VARARGS,""},
     {"get_elem",GetElem,METH_VARARGS,""},
     {"add_first",AddFirst,METH_VARARGS,""},
     {"add_after",AddAfter,METH_VARARGS,""},
     {"list_insert",ListInsert,METH_VARARGS,""},
     {"list_delete",ListDelete,METH_VARARGS,""},
+    {"traverse_list",TraverseList,METH_VARARGS,""},
     {NULL}
 };
 static PyTypeObject LNodeObject = {
     PyVarObject_HEAD_INIT(NULL,0)
     .tp_name = "CircularSingleLinkedList.LNode",
     .tp_new = LNode_new,
     .tp_init = (initproc)LNode_init,
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.c` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/SeqList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/SeqList.h` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/SeqList.h`

 * *Files 2% similar despite different names*

```diff
@@ -171,18 +171,19 @@
     }
 }
 static PyObject* TraverseList(SeqList* self, PyObject* args)
 {
     int i = 0;
     while (i < self->length)
     {
-        PyObject_Print(self->elem[i], stdout, 0);
+        PyObject_Print((PyObject*)self->elem[i], stdout, 0);
         i++;
     }
     printf("\n");
+    Py_RETURN_NONE;
 }
 static PyMethodDef SeqList_methods[] = {
     {"init_list",InitList,METH_VARARGS,""},
     {"destroy_list",DestroyList,METH_VARARGS,""},
     {"clear_list",ClearList,METH_VARARGS,""},
     {"list_empty",ListEmpty,METH_VARARGS,""},
     {"list_length",ListLength,METH_VARARGS,""},
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.c` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedList.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedList.h` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedList.h`

 * *Files 2% similar despite different names*

```diff
@@ -278,25 +278,37 @@
             temp->next = del->next;
             PyMem_FREE(del);
             del = NULL;
             Py_RETURN_TRUE;
         }
     }
 }
+static PyObject* TraverseList(List*self,PyObject*args)
+{
+    LNode *p=self->instance->next;
+    while(p!=NULL)
+    {
+        PyObject_Print(p->elem, stdout, 0);
+        p=p->next;
+    }
+    printf("\n");
+    Py_RETURN_NONE;
+}
 static PyMethodDef List_methods[] = {
     {"init_list",InitList,METH_VARARGS,""},
     {"destroy_list",DestroyList,METH_VARARGS,""},
     {"clear_list",ClearList,METH_VARARGS,""},
     {"list_empty",ListEmpty,METH_VARARGS,""},
     {"list_length",ListLength,METH_VARARGS,""},
     {"get_elem",GetElem,METH_VARARGS,""},
     {"add_first",AddFirst,METH_VARARGS,""},
     {"add_after",AddAfter,METH_VARARGS,""},
     {"list_insert",ListInsert,METH_VARARGS,""},
     {"list_delete",ListDelete,METH_VARARGS,""},
+    {"traverse_list",TraverseList,METH_VARARGS,""},
     {NULL}
 };
 static PyTypeObject LNodeObject = {
     PyVarObject_HEAD_INIT(NULL,0)
     .tp_name = "SingleLinkedList.LNode",
     .tp_new = LNode_new,
     .tp_init = (initproc)LNode_init,
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h` & `AdroitFisherman-0.0.27/AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h`

 * *Files 3% similar despite different names*

```diff
@@ -305,25 +305,37 @@
             p->next = del->next;
             PyMem_FREE(del);
             del = NULL;
             Py_RETURN_TRUE;
         }
     }
 }
+static PyObject* TraverseList(List*self,PyObject*args)
+{
+    LNode *p=self->instance;
+    while(p!=NULL)
+    {
+        PyObject_Print(p->elem, stdout, 0);
+        p=p->next;
+    }
+    printf("\n");
+    Py_RETURN_NONE;
+}
 static PyMethodDef List_methods[] = {
     {"init_list",InitList,METH_VARARGS,""},
     {"destroy_list",DestroyList,METH_VARARGS,""},
     {"clear_list",ClearList,METH_VARARGS,""},
     {"list_empty",ListEmpty,METH_VARARGS,""},
     {"list_length",ListLength,METH_VARARGS,""},
     {"get_elem",GetElem,METH_VARARGS,""},
     {"add_first",AddFirst,METH_VARARGS,""},
     {"add_after",AddAfter,METH_VARARGS,""},
     {"list_insert",ListInsert,METH_VARARGS,""},
     {"list_delete",ListDelete,METH_VARARGS,""},
+    {"traverse_list",TraverseList,METH_VARARGS,""},
     {NULL}
 };
 static PyTypeObject LNodeObject = {
     PyVarObject_HEAD_INIT(NULL,0)
     .tp_name = "SingleLinkedListWithoutHeadNode.LNode",
     .tp_new = LNode_new,
     .tp_init = (initproc)LNode_init,
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman.egg-info/PKG-INFO` & `AdroitFisherman-0.0.27/AdroitFisherman.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.26
+Version: 0.0.27
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AdroitFisherman-0.0.26/AdroitFisherman.egg-info/SOURCES.txt` & `AdroitFisherman-0.0.27/AdroitFisherman.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 setup.py
 AdroitFisherman/__init__.py
 AdroitFisherman.egg-info/PKG-INFO
 AdroitFisherman.egg-info/SOURCES.txt
 AdroitFisherman.egg-info/dependency_links.txt
 AdroitFisherman.egg-info/top_level.txt
 AdroitFisherman/includes/CircularSingleLinkedList.c
+AdroitFisherman/includes/DoubleLinkedList.c
 AdroitFisherman/includes/SeqList.c
 AdroitFisherman/includes/SingleLinkedList.c
 AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
 AdroitFisherman/Utilities/CircularSingleLinkedList.py
+AdroitFisherman/Utilities/DoubleLinkedList.py
 AdroitFisherman/Utilities/SequentialList.py
 AdroitFisherman/Utilities/SingleLinkedList.py
 AdroitFisherman/Utilities/SingleLinkedListWithoutHeadNode.py
 AdroitFisherman/Utilities/__init__.py
 AdroitFisherman/Utilities/__pycache__/SingleLinkedList.cpython-310.pyc
 AdroitFisherman/Utilities/__pycache__/__init__.cpython-310.pyc
 AdroitFisherman/__pycache__/__init__.cpython-310.pyc
 AdroitFisherman/includes/CircularSingleLinkedList.c
 AdroitFisherman/includes/CircularSingleLinkedList.h
+AdroitFisherman/includes/DoubleLinkedList.c
+AdroitFisherman/includes/DoubleLinkedList.h
 AdroitFisherman/includes/SeqList.c
 AdroitFisherman/includes/SeqList.h
 AdroitFisherman/includes/SingleLinkedList.c
 AdroitFisherman/includes/SingleLinkedList.h
 AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c
 AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.h
```

### Comparing `AdroitFisherman-0.0.26/PKG-INFO` & `AdroitFisherman-0.0.27/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdroitFisherman
-Version: 0.0.26
+Version: 0.0.27
 Summary: This is a simple package about Data Structure packed by C/C++ language.
 Home-page: UNKNOWN
 Author: adroit_fisherman
 Author-email: 1295284735@qq.com
 License: UNKNOWN
 Platform: Windows
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `AdroitFisherman-0.0.26/README.md` & `AdroitFisherman-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `AdroitFisherman-0.0.26/setup.py` & `AdroitFisherman-0.0.27/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup,Extension
 SeqList=Extension("AdroitFisherman.SequentialList",sources=['AdroitFisherman/includes/SeqList.c'])
 SingleLinkedList=Extension("AdroitFisherman.SingleLinkedList",sources=['AdroitFisherman/includes/SingleLinkedList.c'])
 SingleLinkedListWithoutHeadNode=Extension("AdroitFisherman.SingleLinkedListWithoutHeadNode",sources=['AdroitFisherman/includes/SingleLinkedListWithoutHeadNode.c'])
 CircularSingleLinkedList=Extension("AdroitFisherman.CircularSingleLinkedList",sources=['AdroitFisherman/includes/CircularSingleLinkedList.c'])
+DoubleLinkedList=Extension("AdroitFisherman.DoubleLinkedList",sources=['AdroitFisherman/includes/DoubleLinkedList.c'])
 read_me = open('README.md', 'r',encoding='utf-8')
 setup(
     name="AdroitFisherman",
-    version="0.0.26",
+    version="0.0.27",
     author="adroit_fisherman",
     author_email="1295284735@qq.com",
     platforms="Windows",
     description="This is a simple package about Data Structure packed by C/C++ language.",
     long_description_content_type="text/markdown",
     long_description=read_me.read(),
     classifiers=[
@@ -22,10 +23,10 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Topic :: Utilities"
     ],
     include_package_data=True,
     packages=['AdroitFisherman.Utilities'],
-    ext_modules=[SeqList,SingleLinkedList,SingleLinkedListWithoutHeadNode,CircularSingleLinkedList]
+    ext_modules=[SeqList,SingleLinkedList,SingleLinkedListWithoutHeadNode,CircularSingleLinkedList,DoubleLinkedList]
 )
 read_me.close()
```

