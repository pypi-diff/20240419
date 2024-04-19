# Comparing `tmp/tgqSim-0.0.9.tar.gz` & `tmp/tgqSim-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgqSim-0.0.9.tar", last modified: Mon Mar 25 06:51:22 2024, max compression
+gzip compressed data, was "tgqSim-0.1.0.tar", last modified: Fri Apr 19 06:00:22 2024, max compression
```

## Comparing `tgqSim-0.0.9.tar` & `tgqSim-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 06:51:22.139247 tgqSim-0.0.9/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2024-03-25 06:51:20.000000 tgqSim-0.0.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-03-25 06:51:20.000000 tgqSim-0.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      752 2024-03-25 06:51:22.139247 tgqSim-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-25 06:51:20.000000 tgqSim-0.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 06:51:22.139247 tgqSim-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-25 06:51:21.000000 tgqSim-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 06:51:22.137247 tgqSim-0.0.9/tgqSim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 06:51:22.139247 tgqSim-0.0.9/tgqSim/GateSimulation/
--rw-rw-rw-   0 root         (0) root         (0)     3793 2024-03-25 06:51:20.000000 tgqSim-0.0.9/tgqSim/GateSimulation/DoubleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-03-25 06:51:20.000000 tgqSim-0.0.9/tgqSim/GateSimulation/SingleGate.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-03-25 06:51:20.000000 tgqSim-0.0.9/tgqSim/GateSimulation/TripleGate.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 06:51:20.000000 tgqSim-0.0.9/tgqSim/GateSimulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13264 2024-03-25 06:51:20.000000 tgqSim-0.0.9/tgqSim/QuantumCircuit.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-03-25 06:51:21.000000 tgqSim-0.0.9/tgqSim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18468 2024-03-25 06:51:20.000000 tgqSim-0.0.9/tgqSim/draw_circuit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 06:51:22.138247 tgqSim-0.0.9/tgqSim.egg-info/
--rw-r--r--   0 root         (0) root         (0)      752 2024-03-25 06:51:22.000000 tgqSim-0.0.9/tgqSim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      402 2024-03-25 06:51:22.000000 tgqSim-0.0.9/tgqSim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 06:51:22.000000 tgqSim-0.0.9/tgqSim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-03-25 06:51:22.000000 tgqSim-0.0.9/tgqSim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-25 06:51:22.000000 tgqSim-0.0.9/tgqSim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.816327 tgqSim-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-04-19 06:00:21.000000 tgqSim-0.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-19 06:00:21.000000 tgqSim-0.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-19 06:00:22.816327 tgqSim-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-19 06:00:21.000000 tgqSim-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 06:00:22.816327 tgqSim-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-19 06:00:22.000000 tgqSim-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.813327 tgqSim-0.1.0/tgqSim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.815327 tgqSim-0.1.0/tgqSim/GateSimulation/
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/DoubleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/SingleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/TripleGate.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/GateSimulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16505 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/QuantumCircuit.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/draw_circuit_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.815327 tgqSim-0.1.0/tgqSim/lib/
+-rw-rw-rw-   0 root         (0) root         (0)    67288 2024-04-19 06:00:21.000000 tgqSim-0.1.0/tgqSim/lib/tgq_simulator.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 06:00:22.814327 tgqSim-0.1.0/tgqSim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-19 06:00:22.000000 tgqSim-0.1.0/tgqSim.egg-info/top_level.txt
```

### Comparing `tgqSim-0.0.9/LICENSE` & `tgqSim-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tgqSim-0.0.9/PKG-INFO` & `tgqSim-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.0.9
+Version: 0.1.0
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `tgqSim-0.0.9/setup.py` & `tgqSim-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='tgqSim',
-    version='0.0.9',
+    version='0.1.0',
     description='TGQ量子模拟器',  # 包描述
     long_description="Python for quantum simulation http://www.tiangongqs.com",  # 详细描述
     long_description_content_type='text/markdown',
     author='tiangongqs',  # 作者姓名
     license='MIT',  # 许可证
     package=find_packages(),
     include_package_data=True,
     packages=["tgqSim", "tgqSim.GateSimulation"],
     install_requires=[
         'numpy>=1.24.3',
         'numba>=0.58.1',
         'matplotlib>=3.7.1',
+        'GPUtil>=1.4.0'
     ],
     classifiers=[
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
```

### Comparing `tgqSim-0.0.9/tgqSim/GateSimulation/DoubleGate.py` & `tgqSim-0.1.0/tgqSim/GateSimulation/DoubleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.0.9/tgqSim/GateSimulation/SingleGate.py` & `tgqSim-0.1.0/tgqSim/GateSimulation/SingleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.0.9/tgqSim/GateSimulation/TripleGate.py` & `tgqSim-0.1.0/tgqSim/GateSimulation/TripleGate.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.0.9/tgqSim/QuantumCircuit.py` & `tgqSim-0.1.0/tgqSim/QuantumCircuit.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,34 @@
 """
 @author: Yuchen He
 @contact: heyuchen@tgqs.net
 @version: 1.0.1
 @file: QuantumCircuit.py
 @time: 2024/1/16 17:16
 """
-from tgqSim.GateSimulation import SingleGate, DoubleGate, TripleGate
+from GateSimulation import SingleGate, DoubleGate, TripleGate
 from typing import Union
-import random
+import random, os, ctypes
 import numpy as np
-import tgqSim.draw_circuit_tools as tools
+import draw_circuit_tools as tools
 import matplotlib.pyplot as plt
+import GPUtil
 # from numba import njit, prange
 
+class Float2(ctypes.Structure):
+    _fields_ = [("x", ctypes.c_float),
+                ("y", ctypes.c_float)]
+
+class GateInfo(ctypes.Structure):
+    _fields_ = [
+        ("gateName", ctypes.c_char_p),
+        ("actionPos", ctypes.POINTER(ctypes.c_int)),
+        ("theta", ctypes.c_float)
+    ]
+
 
 class Qubit:
     def __init__(self, name=None, idx=None, pos=None):
         self.label = 'p' if not name else name
         self.name = f'p_{idx+100}' if not name else f"{name}_{idx}"
         self.pos = pos + idx
         self.idx = idx
@@ -48,14 +60,16 @@
         self.qbit_register = {}
         self.base_single_gate = ['h', 'x', 'y', 'z', 'rx', 'ry', 'rz', 'u3', 's', 'sdg', 't', 'tdg']
         self.base_double_gate = ['cx', 'swap', 'iswap', 'cz', 'cp', 'rxx', 'ryy', 'rzz']
         self.base_triple_gate = ['ccx', 'cswap']
         self.width = 0
         self.state = []
         self.circuit_diag = []
+        self.isgpu = False
+        self.deviceid = []
 
     def add_qubits(self, number: int, name: str = 'p'):
         """
         添加量子比特
         :param number: 比特数量
         :param name: 比特名称
         :return:
@@ -106,40 +120,89 @@
         添加三比特门序列
         :param gate_pos:
         :param gate_info:
         :return:
         """
         self.circuit_diag.append([(gate_info[0].upper(), gate_pos[2], gate_pos[0], gate_pos[1])])
         return self.gate_list.append((gate_pos, gate_info))
+    
+    def setdevice(self, deviceList: Union[int, list]):
+        gpus = GPUtil.getGPUs()
+        gpuidList = [gpu.id for gpu in gpus]
+        if isinstance(deviceList, int):
+            deviceList = [deviceList]
+        for deviceid in deviceList:
+            if deviceid not in gpuidList:
+                raise ValueError("设置设备ID不存在")
+        self.isgpu = True
+        self.deviceid = deviceList
+    
+    def _run_with_device(self):
+        # 未测试
+        dll_path = os.path.abspath('./lib/tgq_simulator.so')
+        lib = ctypes.CDLL(dll_path)
+        lib.execute_circuit.argtypes = [
+            ctypes.POINTER(Float2),
+            ctypes.POINTER(GateInfo),
+            ctypes.c_int,
+            ctypes.c_int,
+            ctypes.c_int
+        ]
+        gateInfo = []
+        for (gate_pos, gate_info) in self.gate_list:
+            if isinstance(gate_pos, int):
+                length = 2
+                gate_pos = [gate_pos]
+            elif isinstance(gate_pos, list):
+                length = len(gate_pos) + 1
+            else:
+                raise TypeError("Type of gate_pos must be int or list")
+            gate_obj = GateInfo()
+            actionPos = gate_pos + [-1]
+            gate_obj.actionPos = (ctypes.c_int * length)(*actionPos)
+            if len(gate_info) > 0:
+                gate_obj.gateName = gate_info[0].encode(encoding='utf-8')
+            if len(gate_info) > 1:
+                gate_obj.theta = gate_info[1]
+            gateInfo.append(gate_obj)
+        gateInfoCData = (GateInfo * len(gateInfo))(*gateInfo)
+        initial_state = [Float2(1.0, 0.0) if i == 0 else Float2(0.0, 0.0) for i in range(2 ** self.width)]
+        psi = (Float2 * len(initial_state))(*initial_state)
+        lib.execute_circuit(psi, gateInfoCData, len(gateInfo), self.width, self.deviceid[0])
+        for i, ele in enumerate(psi):
+            self.state[i] = ele.x + 1j * ele.y
 
     def run_statevector(self):
         """
         根据线路的门序列计算末态的量子态
         :return:
         """
         self.state = [1 if a == 0 else 0 for a in range(2**self.width)]
-        for (gate_pos, gate_info) in self.gate_list:
-            gate_type = gate_info[0]
-            angle = tuple(gate_info[1:])
-            if gate_type in self.base_single_gate:
-                self.state = SingleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
-
-            elif gate_type in self.base_double_gate:
-                set_gate_pos = set(gate_pos)
-                if len(set_gate_pos) != len(gate_pos):
-                    raise SimulationError(f"Gate position cannot be the same: {gate_pos[0]}, {gate_pos[1]}")
-                self.state = DoubleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
-            elif gate_type in self.base_triple_gate:
-                set_gate_pos = set(gate_pos)
-                if len(set_gate_pos) != len(gate_pos):
-                    raise SimulationError(f"Gate position cannot be the same: "
-                                          f"{gate_pos[0]}, {gate_pos[1]} and {gate_pos[2]}")
-                self.state = TripleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
-            else:
-                raise SimulationError(f"Unkown gate type: {gate_type}")
+        if not self.isgpu:
+            for (gate_pos, gate_info) in self.gate_list:
+                gate_type = gate_info[0]
+                angle = tuple(gate_info[1:])
+                if gate_type in self.base_single_gate:
+                    self.state = SingleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
+
+                elif gate_type in self.base_double_gate:
+                    set_gate_pos = set(gate_pos)
+                    if len(set_gate_pos) != len(gate_pos):
+                        raise SimulationError(f"Gate position cannot be the same: {gate_pos[0]}, {gate_pos[1]}")
+                    self.state = DoubleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
+                elif gate_type in self.base_triple_gate:
+                    set_gate_pos = set(gate_pos)
+                    if len(set_gate_pos) != len(gate_pos):
+                        raise SimulationError(f"Gate position cannot be the same: "
+                                            f"{gate_pos[0]}, {gate_pos[1]} and {gate_pos[2]}")
+                    self.state = TripleGate.ActOn_State(self.state, self.width, gate_type, gate_pos, *angle)
+                else:
+                    raise SimulationError(f"Unkown gate type: {gate_type}")
+        else:
+            self._run_with_device()
     
     def random_circuit(self, num_qubits, num_gates: Union[int, list]):
         """
         生成随机线路
         :param num_qubits:
         :param num_gates: 门数量，列表表示单比特，多比特门数量
         :return:
@@ -327,7 +390,35 @@
         cumulate = 0
         sample = np.random.uniform(0,1, size=shots)
         for key in distribution.keys():
             new_cumulate = cumulate + distribution[key]
             result[key] = sum((cumulate<=sample) & (sample<new_cumulate))
             cumulate = new_cumulate
         return result
+
+
+
+# 下面这段代码仅限测试使用，不会参与实际工程
+if __name__ == '__main__':
+    nQubits = 9
+    qc = QuantumCircuit()
+    qc.add_qubits(nQubits, name='qft')
+    for i in range(nQubits):
+        if nQubits - 2 == i:
+            qc.x(i)
+        else:
+            qc.h(i)
+    for i in range(nQubits - 1, -1, -1):
+        for j in range(i, -1, -1):
+            if j == i:
+                qc.h(j)
+            else:
+                qc.cp(control_qubit=j, target_qubit=i, theta=np.pi / (2 ** (i - j)))
+    qc.x(0)
+    for i in range(0, nQubits // 2):
+        qc.swap(qubit_1=i, qubit_2=nQubits - 1 - i)
+    qc.run_statevector()
+    print(qc.state)
+    print(len(qc.state))
+    measure_pos = sorted([1, 0, 2], reverse=True)
+    print(qc.measure(measure_bits_list=measure_pos))
+    # qc.show_quantum_circuit()
```

### Comparing `tgqSim-0.0.9/tgqSim/draw_circuit_tools.py` & `tgqSim-0.1.0/tgqSim/draw_circuit_tools.py`

 * *Files identical despite different names*

### Comparing `tgqSim-0.0.9/tgqSim.egg-info/PKG-INFO` & `tgqSim-0.1.0/tgqSim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgqSim
-Version: 0.0.9
+Version: 0.1.0
 Summary: TGQ量子模拟器
 Home-page: UNKNOWN
 Author: tiangongqs
 License: MIT
 Keywords: tgq,cetc,quantum,simulator
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

