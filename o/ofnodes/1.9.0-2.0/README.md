# Comparing `tmp/ofnodes-1.9.0.tar.gz` & `tmp/ofnodes-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.9.0.tar", max compression
+gzip compressed data, was "ofnodes-2.0.tar", max compression
```

## Comparing `ofnodes-1.9.0.tar` & `ofnodes-2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.9.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.9.0/README.md
--rw-r--r--   0        0        0      590 2024-04-30 21:31:53.616928 ofnodes-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-1.9.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.9.0/src/ofnodes/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.9.0/src/ofnodes/components/nodes/__init__ copy.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.9.0/src/ofnodes/components/nodes/__init__.py
--rw-r--r--   0        0        0     2676 2024-04-30 04:04:14.832970 ofnodes-1.9.0/src/ofnodes/components/nodes/descriptors.py
--rw-r--r--   0        0        0      819 2024-04-30 18:38:02.940918 ofnodes-1.9.0/src/ofnodes/components/nodes/mixins.py
--rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.9.0/src/ofnodes/components/structures/__init__.py
--rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.9.0/src/ofnodes/components/structures/descriptors.py
--rw-r--r--   0        0        0    20486 2024-04-26 16:35:49.237665 ofnodes-1.9.0/src/ofnodes/components/structures/mixins.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.9.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1520 2024-04-26 16:35:56.197622 ofnodes-1.9.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.9.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-30 21:34:11.068241 ofnodes-1.9.0/src/ofnodes/sorting/__init__.py
--rw-r--r--   0        0        0     3449 2024-04-30 21:41:45.001882 ofnodes-1.9.0/src/ofnodes/sorting/mixins.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.9.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0     2842 2024-04-30 21:42:46.537555 ofnodes-1.9.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     2139 2024-04-26 14:35:49.613667 ofnodes-1.9.0/src/ofnodes/structures/stack.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-2.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-2.0/README.md
+-rw-r--r--   0        0        0      588 2024-05-11 15:26:44.285220 ofnodes-2.0/pyproject.toml
+-rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-2.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-2.0/src/ofnodes/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-2.0/src/ofnodes/components/nodes/__init__ copy.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-2.0/src/ofnodes/components/nodes/__init__.py
+-rw-r--r--   0        0        0     2712 2024-05-11 14:42:17.923628 ofnodes-2.0/src/ofnodes/components/nodes/descriptors.py
+-rw-r--r--   0        0        0      838 2024-05-11 14:41:55.031803 ofnodes-2.0/src/ofnodes/components/nodes/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-2.0/src/ofnodes/components/structures/__init__.py
+-rw-r--r--   0        0        0     9137 2024-05-11 15:14:12.690257 ofnodes-2.0/src/ofnodes/components/structures/descriptors.py
+-rw-r--r--   0        0        0    19197 2024-05-11 15:11:36.999269 ofnodes-2.0/src/ofnodes/components/structures/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-2.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1557 2024-05-11 16:24:33.683641 ofnodes-2.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-2.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 21:45:59.484524 ofnodes-2.0/src/ofnodes/sorting/__init__.py
+-rw-r--r--   0        0        0    11004 2024-05-11 15:14:52.185997 ofnodes-2.0/src/ofnodes/sorting/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-2.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0     3961 2024-05-09 21:36:54.532398 ofnodes-2.0/src/ofnodes/structures/randomaccessarray.py
+-rw-r--r--   0        0        0     4872 2024-05-10 20:24:17.377084 ofnodes-2.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     2139 2024-04-26 14:35:49.613667 ofnodes-2.0/src/ofnodes/structures/stack.py
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 ofnodes-2.0/PKG-INFO
```

### Comparing `ofnodes-1.9.0/LICENSE` & `ofnodes-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.9.0/README.md` & `ofnodes-2.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.9.0/pyproject.toml` & `ofnodes-2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.9.0"
+version = "2.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.9.0/src/ofnodes/__init__.py` & `ofnodes-2.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.9.0/src/ofnodes/components/nodes/descriptors.py` & `ofnodes-2.0/src/ofnodes/components/nodes/descriptors.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Methods:
         __get__(self, instance, owner): Getter method for retrieving the value of the data attribute.
         __set__(self, instance, value): Setter method for setting the value of the data attribute.
         __delete__(self, instance): Deleter method for deleting the data attribute.
 
     """
-
+    __slots__ = ()
     def __get__(self, instance, owner):
         """Getter method for retrieving the value of the data attribute."""
         return instance._data
 
     def __set__(self, instance, value):
         """Setter method for setting the value of the data attribute."""
         if value:  # TODO: perform data validation
@@ -44,15 +44,15 @@
 
     Methods:
         __get__(self, instance, owner): Getter method for retrieving the value of the next attribute.
         __set__(self, instance, value): Setter method for setting the value of the next attribute.
         __delete__(self, instance): Deleter method for deleting the next attribute.
 
     """
-
+    __slots__ = ()
     def __get__(self, instance, owner):
         """Getter property for the next node in the singly linked list.
 
         Note:
             This property allows access to the next node in the linked list.
             Modifying the next node should be done using linked list methods
             for consistency and to maintain the integrity of the linked list structure.
```

### Comparing `ofnodes-1.9.0/src/ofnodes/components/nodes/mixins.py` & `ofnodes-2.0/src/ofnodes/components/nodes/mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ofnodes/components/nodes/mixins.py
 #from ofnodes.nodes.singlynode import SinglyNode
 class AddMixin:
+    __slots__ = ()
     def __add__(self, other):
         """Add data to the node's data attribute.
 
         Args:
             other: The data to add to the node's data attribute.
 
         Raises:
```

### Comparing `ofnodes-1.9.0/src/ofnodes/components/structures/descriptors.py` & `ofnodes-2.0/src/ofnodes/components/structures/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ofnodes.nodes.singlynode import SinglyNode
 
 class Head:
+    __slots__ = ()
     def __get__(self, instance, owner):
         """Descriptor for managing the head/top of a data structure.
 
         This descriptor provides getter, setter, and deleter methods for managing the
         head/top of a data structure. It encapsulates the logic related to setting,
         getting, and deleting the head/top element of the data structure.
 
@@ -103,15 +104,15 @@
         ...     tail = Tail()
         ...
         >>> llist = SinglyLinkedList()
         >>> llist.tail = "first node"
         >>> llist.tail
         'first node'
     """
-
+    __slots__ = ()
     def __get__(self, instance, owner):
         """Getter method for the tail of the data structure.
 
         Args:
             instance: An instance of the class where the descriptor is used.
             owner: The class that owns the instance.
 
@@ -201,15 +202,15 @@
         >>> class SinglyLinkedList:
         ...     target = Target()
         ...
         >>> sllist = SinglyLinkedList()
         >>> sllist.target = '5 node'
         Empty SinglyLinkedList(). Target data is assigned to SinglyLinkedList's target property.
     """
-
+    __slots__ = ()
     def __get__(self, instance, owner):
         """Getter method for the target node data of the data structure.
 
         Args:
             instance: An instance of the class where the descriptor is used.
             owner: The class that owns the instance.
```

### Comparing `ofnodes-1.9.0/src/ofnodes/components/structures/mixins.py` & `ofnodes-2.0/src/ofnodes/components/structures/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 from ofnodes.nodes.singlynode import SinglyNode
 
 class SearchMixin:
     """Mixin class providing search functionality for linked lists."""
-
+    __slots__ = ()
     def search(self, target_data):
         """Searches each node's data in a linked list until the first occurrence of
         the target is found.
 
         Args:
             target_data (Any): The value to search for in the linked list.
 
@@ -43,15 +43,15 @@
             if current_node.data == target_data:
                 return True
             current_node = current_node.next
         return False
 
 class RemoveMixin:
     """Mixin class providing remove functionality for linked structures."""
-
+    __slots__ = ()
     def remove(self, target_data):
         """Removes the first occurrence of a node with the specified target data from the linked structure.
 
         Args:
             target_data (Any | Node): The data or node to be removed from the linked structure.
 
         Raises:
@@ -105,16 +105,17 @@
 
         if getattr(self._head, 'data') == self._target:
             return self.remove_head()
 
         current_node = self._head
         while current_node.next is not self._tail:
             if current_node.next.data == self._target:
+                node = current_node.next
                 setattr(current_node, '_next', current_node.next.next)
-                return
+                return node
             current_node = current_node.next
 
         if getattr(self._tail, 'data') == self._target:
             return self.remove_tail()
 
     def remove_head(self) -> None:
         """Removes the head node from the linked structure.
@@ -153,46 +154,17 @@
             return  node
         if self._head and self._head is not self._tail:
             node = self._head
             self._head = self._head.next
             return node
         raise ValueError("Cannot remove head from empty linked structure")
 
-    def remove_tail(self) -> None:
-        """Removes the tail node from the linked structure.
-
-        Raises:
-            ValueError: If the linked structure is empty.
-
-        Returns:
-            None
-
-        Examples:
-            >>> linked_structure = LinkedStructure()
-            >>> linked_structure
-            LinkedStructure(head=None, tail=None)
-            >>> linked_structure.head = True
-            >>> linked_structure
-            LinkedStructure(head=Node(data=True), tail=Node(data=True))
-            >>> linked_structure.tail = ['strings', Node(lambda x: str(x)*2)]
-            >>> linked_structure
-            LinkedStructure(head=Node(data=True), tail=Node(data=['strings', Node(data=<function <lambda> at 0x74a9932a2fc0>)]))
-            >>> linked_structure.tail
-            Node(data=['strings', Node(data=<function <lambda> at 0x74a9932a2fc0>)])
-            >>> linked_structure.tail.data[1].data
-            <function <lambda> at 0x74a9932a2fc0>
-            >>> x = linked_structure.tail.data[1].data
-            >>> x("skrrt")
-            'skrrtskrrt'
-            >>> linked_structure.remove_tail()
-            >>> x("skrrt")
-            'skrrtskrrt'
-            >>> linked_structure.tail
-            Node(data=True)
-            """
+    def remove_tail(self):
+        """
+        """
         match self._head:
             case None:
                 raise ValueError("Cannot remove tail from empty list")
             case self._head:
                 if not getattr(self._head, "_next"):
                     # it's a one node list
                     node = self._tail
@@ -202,27 +174,25 @@
                 if getattr(self._head, "next") is self._tail:
                     # there are two nodes
                     node = self._tail
                     setattr(self, "_tail", self._head)
                     setattr(self._tail, "_next", None)
                     return node
                 # there are more than two nodes
-                node = self._head
-                # find second to last node
-                while getattr(node, "_next") and getattr(node._next, "_next"):
-                    if getattr(node._next, "_next") is self._tail:
-                        node = getattr(node, "_next")  # target found
-                        break
-                    node = getattr(node, "_next")  # keep looking
-                setattr(node, "_next", None)  # point the second to last node to None
-                setattr(self, "_tail", node)  # assign tail to the node
-                return node
+                current = self._head
+                old_tail = self._tail
+                while current.next.next:
+                    current = current.next
+                setattr(current, '_next', None) # bypass the tail
+                setattr(self, '_tail', current) # set the tail
+                return old_tail
 
 class PrintMixin:
     """Mixin class providing node data print functionality"""
+    __slots__ = ()
     def print_node_data(self) -> None:
         """Traverse the linked data structure and print the data attribute of each node.
 
         Returns:
             None
 
         Notes:
@@ -246,14 +216,15 @@
         current_node = self._head
         while current_node:
             print(current_node.data)
             current_node = current_node.next
 
 class InsertHeadMixin:
     """Mixin providing functionality to insert a node at the beginning of a linked structure."""
+    __slots__ = ()
     def insert_head(self, data: Any) -> None:
         """ Inserts a new node with the provided data at the head of the linked list.
 
         Args:
             data: The data to be inserted into the new node. If the data is already a
                 `SinglyNode` object, it is inserted directly; otherwise, a new
                 `SinglyNode` object is created with the provided data.
@@ -292,14 +263,15 @@
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='to be assigned to `SinglyNode.data` then `SinglyLinkedList.head`'), SinglyNode(data='4 node'), SinglyNode(data='1 node'))
         """
         self.head = data  # trigger the head setter
 
 class InsertTailMixin:
     """Mixin providing functionality to insert a node at the end of a linked structure."""
+    __slots__ = ()
     def insert_tail(self, data: Any) -> None:
         """Inserts a new node with the provided data at the tail of the linked list.
 
         Args:
             data: The data to be inserted into the new node. If the data is already a
                 `SinglyNode` object, it is inserted directly; otherwise, a new
                 `SinglyNode` object is created with the provided data.
@@ -344,14 +316,15 @@
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='is passed to setter to become SinglyNode()'))
         """
         self.tail = data  # trigger the tail setter
 
 class InsertAfterTargetMixin:
     """Mixin providing functionality to insert a node after a target node in a linked structure."""
+    __slots__ = ()
     def insert_after_target(self, target_data: Any, data_to_insert: Any) -> bool:
         """
         Inserts a new node containing the specified data after the first occurrence
         of the target data in the linked list.
 
         Args:
             target_data (Any): The data value to search for in the linked list.
@@ -395,14 +368,15 @@
             self.tail = data_to_insert  # # trigger the setter, tail property will validate input
             return True
         # no target match
         return False
 
 class InsertBeforeTargetMixin:
     """Mixin providing functionality to insert a node before a target node in a linked structure."""
+    __slots__ = ()
     def insert_before_target(self, target_data: Any, data_to_insert: Any) -> bool:
         """
         Inserts a new node containing the specified data before the first occurrence
         of the target data in the linked list.
 
         Args:
             target_data: The data value to search for in the linked list or the reference to the node.
```

### Comparing `ofnodes-1.9.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-2.0/src/ofnodes/nodes/singlynode.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 next node in the list.
 
 Example:
     Typical usage example:
 
         uni_node = SinglyNode("a string of characters")
 """
-
+from difflib import get_close_matches
 from typing import Any, Optional
 from ofnodes.components.nodes.descriptors import Data, Next
 from ofnodes.components.nodes.mixins import AddMixin
 
 
 class SinglyNode(AddMixin):
     """Represents a node in a singly linked list.
```

### Comparing `ofnodes-1.9.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-2.0/src/ofnodes/structures/stack.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,65 @@
 from typing import Optional, Any
 
 from ofnodes.nodes.singlynode import SinglyNode
-from ofnodes.components.structures.descriptors import Head, Tail, Target
-from ofnodes.components.structures.mixins import SearchMixin, RemoveMixin, InsertHeadMixin, InsertTailMixin, InsertAfterTargetMixin, InsertBeforeTargetMixin, PrintMixin
-from ofnodes.sorting.mixins import BubbleSortMixin, ReverseOrderMixin
-
-class SinglyLinkedList(SearchMixin, RemoveMixin, InsertHeadMixin, InsertTailMixin, InsertAfterTargetMixin, InsertBeforeTargetMixin, PrintMixin, BubbleSortMixin, ReverseOrderMixin):
-    """A class representing a singly linked list.
-
-    This class provides functionality to create and manipulate a singly linked list
-    data structure. Each node in the linked list contains a reference to the next
-    node in the sequence.
-
-    Attributes:
-        _head (Optional[SinglyNode]): The head of the linked list.
-        _tail (Optional[SinglyNode]): The tail of the linked list.
-        _target (Optional[Any]): The target data or node instance.
-
-    Examples:
-        >>> linked_list = SinglyLinkedList()
-        >>> linked_list
-        SinglyLinkedList(head=None, tail=None, target=None)
-    """
+from ofnodes.components.structures.descriptors import Head
+from ofnodes.components.structures.mixins import RemoveMixin,  PrintMixin
 
-    __slots__ = ('_head', '_tail', '_target',)
+class Stack(RemoveMixin, PrintMixin):
+
+    __slots__ = ('_head',)# '_target',) #'_tail', )
     head = Head()
-    tail = Tail()
-    target = Target()
+    #tail = Tail()
+    #target = Target()
     def __init__(self, values=None) -> None:
         self._head: Optional[SinglyNode] = None
-        self._tail: Optional[SinglyNode] = None
-        self._target: Optional[Any|SinglyNode] = None
+        #self._tail: Optional[SinglyNode] = None
+        #self._target: Optional[Any|SinglyNode] = None
         if values:
             for value in values:
-                self.tail = value
+                self.head = value
+
+    def push(self, data):
+        self.head = data  # trigger the setter, setter validates data
 
-    def cycle_detection(self):
+    def pop(self):
+        return self.remove_head()
 
-        if self.tail.next is not None:
-            return True
-        return False
+    def peek(self):
+        if self._head:
+            return self._head.data
+        raise IndexError("Stack is empty, cannot peek at top element")
 
-    def __add__(self, other):
-        self.tail = other  # tail attr will validate
+    def display(self):
+        self.print_node_data()
 
+    def is_empty(self):
+        return self._head is None
+
+    def __dir__(self) -> list[str]:
+        # Get the list of attributes and methods from the parent classes
+        parent_dir = set(super().__dir__())
+        # Filter out private attributes and methods
+        parent_dir = {attr for attr in parent_dir if attr not in {'_head', '_tail', '_target'}}
+        # Return a sorted list of all attributes and methods
+        return sorted(parent_dir)
 
     def __repr__(self) -> str:
         #return f"{type(self).__name__}(head={type(self.head).__name__}, tail={self.tail})"
         if not self._head:
-            return "SinglyLinkedList()"
+            return f"{type(self).__name__}()"
         node = self._head
         nodes = []
         while node:
             nodes.append(repr(node.data))
             node = node.next
         return f"{type(self).__name__}([" + ', '.join(nodes) + "])"
 
     def __str__(self) -> str:
         if not self._head:
-            return "Empty Singly Linked List"
+            return f"Empty {type(self).__name__}"
         node = self._head
         nodes = []
         while node:
             nodes.append(str(node.data))
             node = node.next
-        return ' -> '.join(nodes)
-
-    def __dir__(self) -> list[str]:
-        # Get the list of attributes and methods from the parent classes
-        parent_dir = set(super().__dir__())
-        # Filter out private attributes and methods
-        parent_dir = {attr for attr in parent_dir if attr not in {'_head', '_tail', '_target'}}
-        # Return a sorted list of all attributes and methods
-        return sorted(parent_dir)
+        return ' -> '.join(nodes)
```

### Comparing `ofnodes-1.9.0/PKG-INFO` & `ofnodes-2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.9.0
+Version: 2.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

