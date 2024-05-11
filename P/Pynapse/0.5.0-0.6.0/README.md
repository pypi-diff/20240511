# Comparing `tmp/pynapse-0.5.0.tar.gz` & `tmp/pynapse-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynapse-0.5.0.tar", last modified: Sat May 11 04:30:25 2024, max compression
+gzip compressed data, was "pynapse-0.6.0.tar", last modified: Sat May 11 04:37:08 2024, max compression
```

## Comparing `pynapse-0.5.0.tar` & `pynapse-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 04:30:25.456611 pynapse-0.5.0/
--rw-rw-rw-   0        0        0     1835 2024-05-11 04:30:25.455614 pynapse-0.5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 04:30:25.423797 pynapse-0.5.0/Pynapse/
--rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-0.5.0/Pynapse/__init__.py
--rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-0.5.0/Pynapse/main.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:30:25.453636 pynapse-0.5.0/Pynapse.egg-info/
--rw-rw-rw-   0        0        0     1835 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1714 2024-05-11 04:30:15.000000 pynapse-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 04:30:25.457608 pynapse-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      316 2024-05-11 04:29:34.000000 pynapse-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:37:08.928706 pynapse-0.6.0/
+-rw-rw-rw-   0        0        0     2734 2024-05-11 04:37:08.927262 pynapse-0.6.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 04:37:08.898445 pynapse-0.6.0/Pynapse/
+-rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-0.6.0/Pynapse/__init__.py
+-rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-0.6.0/Pynapse/main.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:37:08.925268 pynapse-0.6.0/Pynapse.egg-info/
+-rw-rw-rw-   0        0        0     2734 2024-05-11 04:37:08.000000 pynapse-0.6.0/Pynapse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-11 04:37:08.000000 pynapse-0.6.0/Pynapse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 04:37:08.000000 pynapse-0.6.0/Pynapse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 04:37:08.000000 pynapse-0.6.0/Pynapse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 04:37:08.000000 pynapse-0.6.0/Pynapse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2613 2024-05-11 04:36:40.000000 pynapse-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 04:37:08.928706 pynapse-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      316 2024-05-11 04:36:47.000000 pynapse-0.6.0/setup.py
```

### Comparing `pynapse-0.5.0/PKG-INFO` & `pynapse-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Pynapse
-Version: 0.5.0
+Version: 0.6.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
 # USAGE EXAMPLES
 
 ### VIDEO
 
 - to be inserted
 
-### EXAMPLE
+### EXAMPLE FOR SAVING (remove Net_Save to not save your network)
 
 ```python
 from Pynapse import Dense, Activation_Sigmoid, Network, Net_Save, Activation_ReLU, Bin_Round
 import numpy as np
 
 layers = [
     Dense(2, 10),             # 2 inputs, 10 output connections
@@ -44,9 +44,32 @@
 print(prediction)
 
 prediction = Bin_Round.Bin_Round(net.forward(np.array([[1,0]])))
 print(prediction)                                   # Round the output of the output of the output layer to binary 1 or 0    e.g. 1
 ```
 
 
-# WHY CALLED "Pynapse"
-#### This module has been called "Pynapse" meaning Python and Synapse
+### EXAMPLE FOR LOADING
+
+```python
+from Pynapse import Dense, Activation_Sigmoid, Network, Net_Save, Activation_ReLU
+import numpy as np
+
+layers = [
+    Dense(2, 10),             # 2 inputs, 10 output connections
+    Activation_ReLU(),        # ReLU activation function
+    Dense(10, 1),             # 10 inputs (output from previous layer), 1 output neuron
+    Activation_Sigmoid()      # Sigmoid activation function for output to be between 1 and 0
+]
+
+
+net = Network(layers)                               # Set the network to use the provided layers
+
+Net_Save.load('model.json', layers)                 # Load the network from a json file
+
+prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
+print(prediction)                                   # Print the prediction
+```
+
+
+# WHY NAMED "Pynapse"
+#### This module has been named "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-0.5.0/Pynapse/main.py` & `pynapse-0.6.0/Pynapse/main.py`

 * *Files identical despite different names*

### Comparing `pynapse-0.5.0/Pynapse.egg-info/PKG-INFO` & `pynapse-0.6.0/Pynapse.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Pynapse
-Version: 0.5.0
+Version: 0.6.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
 # USAGE EXAMPLES
 
 ### VIDEO
 
 - to be inserted
 
-### EXAMPLE
+### EXAMPLE FOR SAVING (remove Net_Save to not save your network)
 
 ```python
 from Pynapse import Dense, Activation_Sigmoid, Network, Net_Save, Activation_ReLU, Bin_Round
 import numpy as np
 
 layers = [
     Dense(2, 10),             # 2 inputs, 10 output connections
@@ -44,9 +44,32 @@
 print(prediction)
 
 prediction = Bin_Round.Bin_Round(net.forward(np.array([[1,0]])))
 print(prediction)                                   # Round the output of the output of the output layer to binary 1 or 0    e.g. 1
 ```
 
 
-# WHY CALLED "Pynapse"
-#### This module has been called "Pynapse" meaning Python and Synapse
+### EXAMPLE FOR LOADING
+
+```python
+from Pynapse import Dense, Activation_Sigmoid, Network, Net_Save, Activation_ReLU
+import numpy as np
+
+layers = [
+    Dense(2, 10),             # 2 inputs, 10 output connections
+    Activation_ReLU(),        # ReLU activation function
+    Dense(10, 1),             # 10 inputs (output from previous layer), 1 output neuron
+    Activation_Sigmoid()      # Sigmoid activation function for output to be between 1 and 0
+]
+
+
+net = Network(layers)                               # Set the network to use the provided layers
+
+Net_Save.load('model.json', layers)                 # Load the network from a json file
+
+prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
+print(prediction)                                   # Print the prediction
+```
+
+
+# WHY NAMED "Pynapse"
+#### This module has been named "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-0.5.0/README.md` & `pynapse-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # USAGE EXAMPLES
 
 ### VIDEO
 
 - to be inserted
 
-### EXAMPLE
+### EXAMPLE FOR SAVING (remove Net_Save to not save your network)
 
 ```python
 from Pynapse import Dense, Activation_Sigmoid, Network, Net_Save, Activation_ReLU, Bin_Round
 import numpy as np
 
 layers = [
     Dense(2, 10),             # 2 inputs, 10 output connections
@@ -38,9 +38,32 @@
 print(prediction)
 
 prediction = Bin_Round.Bin_Round(net.forward(np.array([[1,0]])))
 print(prediction)                                   # Round the output of the output of the output layer to binary 1 or 0    e.g. 1
 ```
 
 
-# WHY CALLED "Pynapse"
-#### This module has been called "Pynapse" meaning Python and Synapse
+### EXAMPLE FOR LOADING
+
+```python
+from Pynapse import Dense, Activation_Sigmoid, Network, Net_Save, Activation_ReLU
+import numpy as np
+
+layers = [
+    Dense(2, 10),             # 2 inputs, 10 output connections
+    Activation_ReLU(),        # ReLU activation function
+    Dense(10, 1),             # 10 inputs (output from previous layer), 1 output neuron
+    Activation_Sigmoid()      # Sigmoid activation function for output to be between 1 and 0
+]
+
+
+net = Network(layers)                               # Set the network to use the provided layers
+
+Net_Save.load('model.json', layers)                 # Load the network from a json file
+
+prediction = net.forward(np.array([[1,0]]))[0][0]   # You can remove brackets in a variable like this
+print(prediction)                                   # Print the prediction
+```
+
+
+# WHY NAMED "Pynapse"
+#### This module has been named "Pynapse" meaning Python and Synapse
```

