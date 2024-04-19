# Comparing `tmp/qualesim-quantumsim-1.0.0.tar.gz` & `tmp/qualesim-quantumsim-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quantumsim-1.0.0.tar", last modified: Fri Mar 29 08:16:25 2024, max compression
+gzip compressed data, was "qualesim-quantumsim-1.0.1.tar", last modified: Fri Apr 19 03:20:49 2024, max compression
```

## Comparing `qualesim-quantumsim-1.0.0.tar` & `qualesim-quantumsim-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:16:25.845497 qualesim-quantumsim-1.0.0/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-07-04 13:48:17.000000 qualesim-quantumsim-1.0.0/LICENSE
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-03-29 08:16:25.845497 qualesim-quantumsim-1.0.0/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       81 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.0/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:16:25.845497 qualesim-quantumsim-1.0.0/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:16:25.845497 qualesim-quantumsim-1.0.0/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.0/data/bin/dqcsbequantumsim
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:16:25.845497 qualesim-quantumsim-1.0.0/qualesim_quantumsim/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        2 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim/__init__.py
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9727 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim/backend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7614 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim/qubit.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:16:25.845497 qualesim-quantumsim-1.0.0/qualesim_quantumsim.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-03-29 08:16:25.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      390 2024-03-29 08:16:25.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-03-29 08:16:25.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       22 2024-03-29 08:16:25.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       20 2024-03-29 08:16:25.000000 qualesim-quantumsim-1.0.0/qualesim_quantumsim.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-03-29 08:16:25.845497 qualesim-quantumsim-1.0.0/setup.cfg
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.0/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:20:49.035721 qualesim-quantumsim-1.0.1/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-07-04 13:48:17.000000 qualesim-quantumsim-1.0.1/LICENSE
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-04-19 03:20:49.031721 qualesim-quantumsim-1.0.1/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       81 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.1/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:20:49.031721 qualesim-quantumsim-1.0.1/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:20:49.031721 qualesim-quantumsim-1.0.1/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.1/data/bin/dqcsbequantumsim
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:20:49.031721 qualesim-quantumsim-1.0.1/qualesim_quantumsim/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        2 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim/__init__.py
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      113 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11498 2024-04-19 03:10:17.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim/backend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7614 2024-03-29 08:05:06.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim/qubit.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:20:49.031721 qualesim-quantumsim-1.0.1/qualesim_quantumsim.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      686 2024-04-19 03:20:48.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      390 2024-04-19 03:20:49.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-19 03:20:48.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       22 2024-04-19 03:20:48.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       20 2024-04-19 03:20:48.000000 qualesim-quantumsim-1.0.1/qualesim_quantumsim.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-19 03:20:49.035721 qualesim-quantumsim-1.0.1/setup.cfg
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1113 2024-04-18 09:06:26.000000 qualesim-quantumsim-1.0.1/setup.py
```

### Comparing `qualesim-quantumsim-1.0.0/LICENSE` & `qualesim-quantumsim-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quantumsim-1.0.0/PKG-INFO` & `qualesim-quantumsim-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quantumsim
-Version: 1.0.0
+Version: 1.0.1
 Summary: QuaLeSim backend for QuantumSim.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quantumsim.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: QuaLeSim quantumsim
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quantumsim-1.0.0/qualesim_quantumsim/backend.py` & `qualesim-quantumsim-1.0.1/qualesim_quantumsim/backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from qualesim.plugin import *
 from qualesim.common import *
 from qualesim_quantumsim.qubit import Qubit
 import struct
 import numpy as np
-
+from quantumsim.dm_np import DensityNP
 # import copy
 
 
 @plugin("QuantumSim interface for QuaLeSim", "Dingdong Liu", "0.0.1")
 class QuantumSimInterface(Backend):
     # QuantumSim's SparseDM object doesn't support adding or removing qubits.
     # However, any qubits that haven't been entangled yet are purely classical.
@@ -142,17 +142,19 @@
             basis[3].real - basis[3].imag * 1j,
         ]
 
         # Perform the measurements.
         measurements = []
         msg = dict()
         msmt = []
-        state_res_before = self._dm_to_vec(self.sdm.full_dm)
+        state_res_before = self._dm_to_vec(self.sdm.full_dm.to_array())
+        st = dict()
         res_l = []
         for qubit_ref in qubit_refs:
+            st[qubit_ref] = self._partial_trace(self.sdm.full_dm, qubit_ref - 1)
             self.handle_unitary_gate([qubit_ref], basis_hermetian, None)
             qubit: Qubit = self.qubits[qubit_ref]
             qubit.apply_pending_error()
             if qubit.qs_ref is not None:
                 p0, p1 = qubit.qsi.sdm.peak_measurement(qubit.qs_ref)
                 trace = p0 + p1
                 p0 /= trace
@@ -167,37 +169,46 @@
                 else:
                     p = p0
             msg[qubit_ref] = (qubit.classical, p)
             self.cls_dict[qubit_ref] = qubit.classical
             res_l.append(qubit.classical)
         msmt.append(res_l)
 
-        state_res_after = self._dm_to_vec(self.sdm.full_dm)
         if measure_mod == "measureforres":
             state_res = str([self.cls_dict, state_res_before])
+            for qubit_ref in qubit_refs:
+                measurements.append(
+                    Measurement(
+                        qubit_ref,
+                        msg[qubit_ref][0],
+                        struct.pack("<d", msg[qubit_ref][1]),
+                        probability=msg[qubit_ref][1],
+                        state_vector=state_res,
+                        one_shot=msmt,
+                    )
+                )
+                self.handle_unitary_gate([qubit_ref], basis, None)
         else:
-            state_res = str([self.cls_dict, state_res_after])
-        for qubit_ref in qubit_refs:
-            measurements.append(
-                Measurement(
-                    qubit_ref,
-                    msg[qubit_ref][0],
-                    struct.pack("<d", msg[qubit_ref][1]),
-                    probability=msg[qubit_ref][1],
-                    state_vector=state_res,
-                    state_vector_be=str([self.cls_dict, state_res_before]),
-                    one_shot=msmt,
+            for qubit_ref in qubit_refs:
+                state_res = str([self.cls_dict, st[qubit_ref]])
+                measurements.append(
+                    Measurement(
+                        qubit_ref,
+                        msg[qubit_ref][0],
+                        struct.pack("<d", msg[qubit_ref][1]),
+                        probability=msg[qubit_ref][1],
+                        state_vector=state_res,
+                        one_shot=msmt,
+                    )
                 )
-            )
-            self.handle_unitary_gate([qubit_ref], basis, None)
+                self.handle_unitary_gate([qubit_ref], basis, None)
         return measurements
 
-    def _dm_to_vec(self, full_dm):
+    def _dm_to_vec(self, dm_array):
         """Method turning a pure state density matrix into state vector."""
-        dm_array = full_dm.to_array()
         num_col = dm_array.shape[1]  # Number of columns
         # The target state vector got from normalizing the column with the largest norm.
         # Mathematically, a colunm with non-zero norm is enough, but in real computer *some almost zero number is not zero*.
         # Thus, we choose the-largest-norm column to get away from that situation.
         state_vec = None
         cur_max_norm = 0
         for i in range(0, num_col):
@@ -205,14 +216,40 @@
             # This norm is just the norm of the current col's common (one-of-amplitude)* factor
             norm = np.linalg.norm(col_vec)
             if norm > cur_max_norm:
                 state_vec = col_vec / norm
                 cur_max_norm = norm
         return list(state_vec)
 
+    def _partial_trace(self, full_dm, qubits_ref):
+        """Method for partial trace of a density matrix."""
+        dm_array = full_dm.to_array()
+        num_qubits = int(np.log2(dm_array.shape[0]))  # Total number of qubits
+        qubits_to_trace = [i for i in range(num_qubits) if i != qubits_ref]
+        num_qubits_to_trace = len(qubits_to_trace)  # Number of qubits to trace out
+
+        # Compute the dimensions of the reduced density matrix
+        reduced_dm_dim = 2**(num_qubits - num_qubits_to_trace)
+
+        # Initialize the reduced density matrix
+        reduced_dm = np.zeros((reduced_dm_dim, reduced_dm_dim), dtype=np.complex128)
+
+        # Compute the indices of the qubits to keep
+        qubits_to_keep = sorted(set(range(num_qubits)) - set(qubits_to_trace))
+
+        # Iterate over all elements of the full density matrix
+        for i in range(2**num_qubits):
+            # Compute the indices of the corresponding element in the reduced density matrix
+            reduced_dm_index = tuple(np.array([i >> q & 1 for q in qubits_to_keep]))
+
+            # Update the corresponding element in the reduced density matrix
+            reduced_dm[reduced_dm_index] += dm_array[i, i]
+        return self._dm_to_vec(reduced_dm)
+
+
     def handle_prepare_gate(self, qubit_refs, basis, _arb):
         measurements = []
         for qubit_ref in qubit_refs:
             self.qubits[qubit_ref].prep()
             self.handle_unitary_gate([qubit_ref], basis, None)
         return measurements
```

### Comparing `qualesim-quantumsim-1.0.0/qualesim_quantumsim/qubit.py` & `qualesim-quantumsim-1.0.1/qualesim_quantumsim/qubit.py`

 * *Files identical despite different names*

### Comparing `qualesim-quantumsim-1.0.0/qualesim_quantumsim.egg-info/PKG-INFO` & `qualesim-quantumsim-1.0.1/qualesim_quantumsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quantumsim
-Version: 1.0.0
+Version: 1.0.1
 Summary: QuaLeSim backend for QuantumSim.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quantumsim.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: QuaLeSim quantumsim
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quantumsim-1.0.0/setup.py` & `qualesim-quantumsim-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quantumsim",
-    version="1.0.0",
+    version="1.0.1",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim backend for QuantumSim.",
     license="GPLv3",
     keywords="QuaLeSim quantumsim",
     url="https://gitee.com/hpcl_quanta/dqcsim-quantumsim.git",
     long_description=read("README.md"),
```

