# Comparing `tmp/tgqSim-0.1.2.tar.gz` & `tmp/tgqSim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.1.2.tar", last modified: Mon May  6 06:10:07 2024, max compression
+gzip compressed data, was "tgqSim-0.1.3.tar", last modified: Fri May 10 08:15:36 2024, max compression
```

## Comparing `tgqSim-0.1.2.tar` & `tgqSim-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.921466 tgqSim-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-06 06:10:06.000000 tgqSim-0.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-06 06:10:06.000000 tgqSim-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      752 2024-05-06 06:10:07.920466 tgqSim-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-06 06:10:06.000000 tgqSim-0.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 06:10:07.921466 tgqSim-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-06 06:10:07.000000 tgqSim-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.918466 tgqSim-0.1.2/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.920466 tgqSim-0.1.2/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21020 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.920466 tgqSim-0.1.2/tgqSim/lib/
--rw-rw-rw-   0 root         (0) root         (0)    67288 2024-05-06 06:10:06.000000 tgqSim-0.1.2/tgqSim/lib/tgq_simulator.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 06:10:07.919466 tgqSim-0.1.2/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      752 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-06 06:10:07.000000 tgqSim-0.1.2/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 08:15:36.891467 tgqSim-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-10 08:15:34.000000 tgqSim-0.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-10 08:15:34.000000 tgqSim-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-10 08:15:36.891467 tgqSim-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-05-10 08:15:34.000000 tgqSim-0.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 08:15:36.891467 tgqSim-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-10 08:15:35.000000 tgqSim-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 08:15:36.888467 tgqSim-0.1.3/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 08:15:36.890467 tgqSim-0.1.3/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-10 08:15:34.000000 tgqSim-0.1.3/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5413 2024-05-10 08:15:34.000000 tgqSim-0.1.3/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-10 08:15:34.000000 tgqSim-0.1.3/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-10 08:15:34.000000 tgqSim-0.1.3/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21865 2024-05-10 08:15:34.000000 tgqSim-0.1.3/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-10 08:15:35.000000 tgqSim-0.1.3/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-05-10 08:15:34.000000 tgqSim-0.1.3/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 08:15:36.891467 tgqSim-0.1.3/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    73408 2024-05-10 08:15:34.000000 tgqSim-0.1.3/tgqSim/lib/tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 08:15:36.889467 tgqSim-0.1.3/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-10 08:15:36.000000 tgqSim-0.1.3/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-10 08:15:36.000000 tgqSim-0.1.3/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 08:15:36.000000 tgqSim-0.1.3/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-10 08:15:36.000000 tgqSim-0.1.3/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-10 08:15:36.000000 tgqSim-0.1.3/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.1.2/LICENSE` & `tgqSim-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.2/PKG-INFO` & `tgqSim-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.2
+Version: 0.1.3
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.1.2/setup.py` & `tgqSim-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.1.2',
+    version='0.1.3',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
```

### Comparing `tgqSim-0.1.2/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.3/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.2/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.3/tgqSim/GateSimulation/SingleGate.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,21 @@
         for l in prange(0, i):
             i0 = l | klist[k]  # to find a(*...*0_j*...)
             i1 = i0 | i  # to find a(*...*1_j*...) by plus a(00001_j0000)
             temp = np.dot(Gate_mat, np.array([psi[i0], psi[i1]]))
             psi[i0], psi[i1] = temp[0], temp[1]
     return psi
 
+def normalization(psi:list, num_qubits: int):
+    norm = np.linalg.norm(psi)
+    if 0 == norm:
+        return [1 if 0 == i else 0 for i in range(2**num_qubits)]
+    else:
+        return list(np.divide(psi, norm))
+
 
 def ActOn_State(psi, num_qubits, gate_type:str, gate_pos, *angles):
     """
     单比特门作用于线路的实现
     :param psi:
     :param num_qubits:
     :param gate_type: 门类型
@@ -104,8 +111,35 @@
     elif gate_type.lower() == 'tdg':
         rz_mat = np.array(
             [
                 [1, 0], 
                 [0, cm.exp(-np.pi / 4 * 1j)]
             ]
         )
-        return SingleMatirx_ActOn_State(psi, num_qubits, Gate_mat=rz_mat, Gate_pos=gate_pos)
+        return SingleMatirx_ActOn_State(psi, num_qubits, Gate_mat=rz_mat, Gate_pos=gate_pos)
+    elif gate_type.lower() == "damp_i":
+        error_rate = angles[0]
+        rz_mat = np.array(
+            [
+                [1, 0],
+                [0, np.sqrt(1 - error_rate)]
+            ]
+        )
+        return normalization(SingleMatirx_ActOn_State(psi, num_qubits, Gate_mat=rz_mat, Gate_pos=gate_pos), num_qubits)
+    elif gate_type.lower() == "pd":
+        error_rate = angles[0]
+        rz_mat = np.array(
+            [
+                [0, 0],
+                [0, np.sqrt(error_rate)]
+            ]
+        )
+        return normalization(SingleMatirx_ActOn_State(psi, num_qubits, Gate_mat=rz_mat, Gate_pos=gate_pos), num_qubits)
+    elif gate_type.lower() == "ad":
+        error_rate = angles[0]
+        rz_mat = np.array(
+            [
+                [0, np.sqrt(error_rate)],
+                [0, 0]
+            ]
+        )
+        return normalization(SingleMatirx_ActOn_State(psi, num_qubits, Gate_mat=rz_mat, Gate_pos=gate_pos), num_qubits)
```

### Comparing `tgqSim-0.1.2/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.3/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.2/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.3/tgqSim/QuantumCircuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
 
 class QuantumCircuit:
     def __init__(self, qbit_number=None):
         self.qbit_list = [] if not qbit_number else self.add_qubits(number=qbit_number)
         self.cbit_list = []
         self.gate_list = []
         self.qbit_register = {}
-        self.base_single_gate = ['h', 'x', 'y', 'z', 'rx', 'ry', 'rz', 'u3', 's', 'sdg', 't', 'tdg']
+        self.base_single_gate = ['h', 'x', 'y', 'z', 'rx', 'ry', 'rz', 'u3', 's', 'sdg', 't', 'tdg', "damp_I", "pd", "ad"]
         self.base_double_gate = ['cx', 'swap', 'iswap', 'cz', 'cp', 'rxx', 'ryy', 'rzz', 'syc']
         self.base_triple_gate = ['ccx', 'cswap']
-        self.noise_mapper = {"bit_flip": "BF", "asymmetric_depolarization": "ADP", "depolarize": "DP", "phase_flip": "PF"}
+        self.noise_mapper = {"bit_flip": "BF", "asymmetric_depolarization": "ADP", "depolarize": "DP", "phase_flip": "PF", "phase_damp": "PD", "amplitude_damp": "AD"}
         self.width = 0
         self.state = []
         self.circuit_diag = []
         self.isgpu = False
         self.deviceid = []
         self.noise_circuit = []
         self.current_gate_info = ()
@@ -184,27 +184,29 @@
         initial_state = [Float2(1.0, 0.0) if i == 0 else Float2(0.0, 0.0) for i in range(2 ** self.width)]
         psi = (Float2 * len(initial_state))(*initial_state)
         lib.execute_circuit(psi, gateInfoCData, len(gateInfo), self.width, self.deviceid[0])
         for i, ele in enumerate(psi):
             self.state[i] = ele.x + 1j * ele.y
 
     def run_with_noise(self, shots:int=1000):
-        noise_type = ["bit_flip", "asymmetric_depolarization", "depolarize", "phase_flip"]
+        noise_type = ["bit_flip", "asymmetric_depolarization", "depolarize", "phase_flip", "phase_damp", "amplitude_damp"]
         result_dict = {}
         for _ in range(shots):
             new_circuit = []
             for (gate_pos, gate_info) in self.noise_circuit:
                 if gate_info[0] in noise_type:
                     noise_gate = QuantumCircuit.parse_noise(noise_type=gate_info[0], gate_pos=gate_pos, error_rate=gate_info[1])
+                    # print(noise_gate)
                     if noise_gate is not None:
                         new_circuit.append(noise_gate)
                 else:
                     new_circuit.append((gate_pos, gate_info))
             self.gate_list = new_circuit
             result = self.measure(measure_bits_list=[i for i in range(self.width)], shots=1)
+            # print(self.state)
             key = list(result.keys())[0]
             if key in result_dict:
                 result_dict[key] += 1
             else:
                 result_dict[key] = 1
         self.prob_result = result_dict
 
@@ -269,19 +271,23 @@
             gate_name = QuantumCircuit.bit_flip(error_rate)
         elif "asymmetric_depolarization" == noise_type:
             gate_name = QuantumCircuit.asymmetric_depolarization(error_rate)
         elif "depolarize" == noise_type:
             gate_name = QuantumCircuit.depolarize(error_rate)
         elif "phase_flip" == noise_type:
             gate_name = QuantumCircuit.phase_flip(error_rate)
+        elif "phase_damp" == noise_type:
+            gate_name = QuantumCircuit.phase_damp(error_rate)
+        elif "amplitude_damp" == noise_type:
+            gate_name = QuantumCircuit.amplitude_damp(error_rate)
         else:
             raise ValueError("Please check noise model name")
         if gate_name == "I":
             return None
-        return (gate_pos, (gate_name))
+        return (gate_pos, (gate_name, error_rate))
     
     @staticmethod
     def bit_flip(error_rate: float):
         random_value = random.uniform(0, 1)
         gate_name = "I"
         if random_value < error_rate:
             gate_name = "x"
@@ -312,14 +318,29 @@
     def phase_flip(error_rate: float):
         random_value = random.uniform(0, 1)
         gate_name = "I"
         if random_value < error_rate:
             gate_name = "z"
         return gate_name
 
+    @staticmethod
+    def phase_damp(error_rate: float):
+        random_value = random.uniform(0, 1)
+        gate_name = "damp_I"
+        if random_value < error_rate:
+            gate_name = "pd"
+        return gate_name
+
+    @staticmethod
+    def amplitude_damp(error_rate: float):
+        random_value = random.uniform(0, 1)
+        gate_name = "damp_I"
+        if random_value < error_rate:
+            gate_name = "ad"
+        return gate_name
     
     def random_circuit(self, num_qubits, num_gates: Union[int, list]):
         """
         生成随机线路
         :param num_qubits:
         :param num_gates: 门数量，列表表示单比特，多比特门数量
         :return:
```

### Comparing `tgqSim-0.1.2/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.3/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.1.2/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.3/tgqSim.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.1.2
+Version: 0.1.3
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

