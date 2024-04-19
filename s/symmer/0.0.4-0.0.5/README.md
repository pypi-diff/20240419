# Comparing `tmp/symmer-0.0.4.tar.gz` & `tmp/symmer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symmer-0.0.4.tar", max compression
+gzip compressed data, was "symmer-0.0.5.tar", max compression
```

## Comparing `symmer-0.0.4.tar` & `symmer-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,36 @@
--rw-r--r--   0        0        0     1085 2023-08-17 21:14:44.558201 symmer-0.0.4/LICENSE
--rw-r--r--   0        0        0      732 2023-09-06 20:55:40.410718 symmer-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-08-18 13:46:47.636712 symmer-0.0.4/symmer/.DS_Store
--rw-r--r--   0        0        0      176 2023-08-17 21:14:44.576688 symmer-0.0.4/symmer/.idea/.gitignore
--rw-r--r--   0        0        0      697 2023-08-17 21:14:44.576916 symmer-0.0.4/symmer/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-08-17 21:14:44.577056 symmer-0.0.4/symmer/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      194 2023-08-17 21:14:44.581224 symmer-0.0.4/symmer/.idea/misc.xml
--rw-r--r--   0        0        0      264 2023-08-17 21:14:44.581519 symmer-0.0.4/symmer/.idea/modules.xml
--rw-r--r--   0        0        0      483 2023-08-17 21:14:44.581778 symmer-0.0.4/symmer/.idea/symmer.iml
--rw-r--r--   0        0        0      183 2023-08-17 21:14:44.582016 symmer-0.0.4/symmer/.idea/vcs.xml
--rw-r--r--   0        0        0      170 2023-08-17 21:14:44.582290 symmer-0.0.4/symmer/__init__.py
--rw-r--r--   0        0        0      117 2023-08-17 21:14:44.582646 symmer-0.0.4/symmer/approximate/__init__.py
--rw-r--r--   0        0        0    11289 2023-08-17 21:14:44.582978 symmer-0.0.4/symmer/approximate/tensor_network.py
--rw-r--r--   0        0        0     6237 2023-08-17 21:14:44.583359 symmer-0.0.4/symmer/command_line.py
--rw-r--r--   0        0        0      256 2023-08-17 21:14:44.583866 symmer-0.0.4/symmer/evolution/__init__.py
--rw-r--r--   0        0        0     9244 2023-08-17 21:14:44.584258 symmer-0.0.4/symmer/evolution/decomposition.py
--rw-r--r--   0        0        0     1543 2023-08-17 21:14:44.584538 symmer-0.0.4/symmer/evolution/exponentiation.py
--rw-r--r--   0        0        0     6387 2023-08-17 21:14:44.584737 symmer-0.0.4/symmer/evolution/gate_library.py
--rw-r--r--   0        0        0    21116 2023-08-17 21:14:44.585125 symmer-0.0.4/symmer/evolution/variational_optimization.py
--rw-r--r--   0        0        0      202 2023-08-17 21:14:44.585496 symmer-0.0.4/symmer/operators/__init__.py
--rw-r--r--   0        0        0    19997 2023-09-06 18:56:47.361427 symmer-0.0.4/symmer/operators/anticommuting_op.py
--rw-r--r--   0        0        0   103667 2023-09-06 18:56:47.362781 symmer-0.0.4/symmer/operators/base.py
--rw-r--r--   0        0        0    16751 2023-08-22 20:33:49.642540 symmer-0.0.4/symmer/operators/independent_op.py
--rw-r--r--   0        0        0    42158 2023-09-06 18:56:47.363944 symmer-0.0.4/symmer/operators/noncontextual_op.py
--rw-r--r--   0        0        0    21864 2023-09-06 18:56:47.364863 symmer-0.0.4/symmer/operators/utils.py
--rw-r--r--   0        0        0      230 2023-08-17 21:14:44.588730 symmer-0.0.4/symmer/projection/__init__.py
--rw-r--r--   0        0        0     8053 2023-08-17 21:14:44.588938 symmer-0.0.4/symmer/projection/base.py
--rw-r--r--   0        0        0    18153 2023-08-22 20:33:49.645578 symmer-0.0.4/symmer/projection/contextual_subspace.py
--rw-r--r--   0        0        0     9367 2023-08-17 21:14:44.589525 symmer-0.0.4/symmer/projection/qubit_subspace_manager.py
--rw-r--r--   0        0        0     4433 2023-08-17 21:14:44.589786 symmer-0.0.4/symmer/projection/qubit_tapering.py
--rw-r--r--   0        0        0    14701 2023-08-22 20:33:49.646381 symmer-0.0.4/symmer/projection/utils.py
--rw-r--r--   0        0        0    16453 2023-09-06 20:55:40.412045 symmer-0.0.4/symmer/utils.py
--rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 symmer-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-13 22:23:59.000049 symmer-0.0.5/LICENSE
+-rw-r--r--   0        0        0      715 2024-04-19 17:14:30.601754 symmer-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-03-13 22:26:29.148531 symmer-0.0.5/symmer/.DS_Store
+-rw-r--r--   0        0        0      176 2024-03-13 19:03:28.769421 symmer-0.0.5/symmer/.idea/.gitignore
+-rw-r--r--   0        0        0      697 2024-03-13 19:03:28.769509 symmer-0.0.5/symmer/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2024-03-13 19:03:28.769564 symmer-0.0.5/symmer/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      194 2024-03-13 19:03:28.769619 symmer-0.0.5/symmer/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2024-03-13 19:03:28.769673 symmer-0.0.5/symmer/.idea/modules.xml
+-rw-r--r--   0        0        0      483 2024-03-13 19:03:28.769724 symmer-0.0.5/symmer/.idea/symmer.iml
+-rw-r--r--   0        0        0      183 2024-03-13 19:03:28.769771 symmer-0.0.5/symmer/.idea/vcs.xml
+-rw-r--r--   0        0        0      213 2024-03-13 19:03:28.769824 symmer-0.0.5/symmer/__init__.py
+-rw-r--r--   0        0        0      117 2024-03-13 19:03:28.769902 symmer-0.0.5/symmer/approximate/__init__.py
+-rw-r--r--   0        0        0    11289 2024-03-13 19:03:28.770007 symmer-0.0.5/symmer/approximate/tensor_network.py
+-rw-r--r--   0        0        0     6237 2024-03-13 19:03:28.770069 symmer-0.0.5/symmer/command_line.py
+-rw-r--r--   0        0        0      348 2024-03-13 19:03:28.770161 symmer-0.0.5/symmer/evolution/__init__.py
+-rw-r--r--   0        0        0     8638 2024-04-03 14:57:36.601798 symmer-0.0.5/symmer/evolution/circuit_symmerlator.py
+-rw-r--r--   0        0        0     8267 2024-03-13 19:03:28.770355 symmer-0.0.5/symmer/evolution/decomposition.py
+-rw-r--r--   0        0        0     1543 2024-03-13 19:03:28.770423 symmer-0.0.5/symmer/evolution/exponentiation.py
+-rw-r--r--   0        0        0     7027 2024-03-13 19:03:28.770482 symmer-0.0.5/symmer/evolution/gate_library.py
+-rw-r--r--   0        0        0     2976 2024-03-13 19:03:28.770540 symmer-0.0.5/symmer/evolution/utils.py
+-rw-r--r--   0        0        0    20786 2024-04-03 14:57:36.602058 symmer-0.0.5/symmer/evolution/variational_optimization.py
+-rw-r--r--   0        0        0      202 2024-03-13 19:03:28.771064 symmer-0.0.5/symmer/operators/__init__.py
+-rw-r--r--   0        0        0    18663 2024-03-13 19:03:28.771172 symmer-0.0.5/symmer/operators/anticommuting_op.py
+-rw-r--r--   0        0        0   103971 2024-03-18 14:06:58.576214 symmer-0.0.5/symmer/operators/base.py
+-rw-r--r--   0        0        0    16301 2024-03-13 19:03:28.771856 symmer-0.0.5/symmer/operators/independent_op.py
+-rw-r--r--   0        0        0    36398 2024-03-13 21:27:40.833354 symmer-0.0.5/symmer/operators/noncontextual_op.py
+-rw-r--r--   0        0        0    23149 2024-03-18 14:22:32.602447 symmer-0.0.5/symmer/operators/utils.py
+-rw-r--r--   0        0        0     4083 2024-03-13 19:03:28.772477 symmer-0.0.5/symmer/process_handler.py
+-rw-r--r--   0        0        0      229 2024-03-13 19:03:28.772563 symmer-0.0.5/symmer/projection/__init__.py
+-rw-r--r--   0        0        0     8052 2024-04-19 16:49:19.755415 symmer-0.0.5/symmer/projection/base.py
+-rw-r--r--   0        0        0    16851 2024-04-19 16:49:19.755565 symmer-0.0.5/symmer/projection/contextual_subspace.py
+-rw-r--r--   0        0        0     9357 2024-04-19 16:49:19.755730 symmer-0.0.5/symmer/projection/qubit_subspace_manager.py
+-rw-r--r--   0        0        0     4656 2024-04-19 16:49:19.755857 symmer-0.0.5/symmer/projection/qubit_tapering.py
+-rw-r--r--   0        0        0    14701 2024-03-13 19:03:28.773196 symmer-0.0.5/symmer/projection/utils.py
+-rw-r--r--   0        0        0    15923 2024-03-13 19:03:28.773288 symmer-0.0.5/symmer/utils.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 symmer-0.0.5/PKG-INFO
```

### Comparing `symmer-0.0.4/LICENSE` & `symmer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `symmer-0.0.4/symmer/.idea/inspectionProfiles/Project_Default.xml` & `symmer-0.0.5/symmer/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `symmer-0.0.4/symmer/approximate/tensor_network.py` & `symmer-0.0.5/symmer/approximate/tensor_network.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.4/symmer/command_line.py` & `symmer-0.0.5/symmer/command_line.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.4/symmer/evolution/decomposition.py` & `symmer-0.0.5/symmer/evolution/decomposition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import reduce
 from typing import Dict, List, Union
 from symmer.operators import PauliwordOp, QuantumState
 from symmer.evolution.gate_library import *
 from qiskit.circuit import QuantumCircuit, ParameterVector
-import networkx as nx
+from networkx import Graph, draw_spring
+from collections import Counter
 import warnings
 warnings.filterwarnings("ignore", category=DeprecationWarning) 
 
 ##############################################
 # Decompose any QASM file into a PauliwordOp #
 ##############################################
 
@@ -195,32 +196,8 @@
         qc.barrier()
 
     for i in basis_change_indices['Y_indices']:
         qc.s(qiskit_ordering(i))
     for i in basis_change_indices['X_indices']:
         qc.h(qiskit_ordering(i))
         
-    return qc
-
-def get_CNOT_connectivity_graph(evolution_obj: Union[PauliwordOp, QuantumCircuit], print_graph=False):
-    """ 
-    Get the graph whoss edges denote nonlocal interaction between two qubits.
-    This is useful for device-aware ansatz construction to ensure the circuit connectiviy
-    may be accomodated by the topology of the target quantum processor. 
-
-    Args:
-        evolution_obj (Union[PauliwordOp, QuantumCircuit]): Evolution Object
-        print_graph (bool): If True, the graph is drawn. By default, it's set to False.
-    """
-    if isinstance(evolution_obj, PauliwordOp):
-        qc = PauliwordOp_to_QuantumCircuit(evolution_obj)
-    else:
-        assert isinstance(evolution_obj, QuantumCircuit)
-        qc = evolution_obj
-    nodes = [q.index for q in qc.qregs[0]]
-    edges = [[q.index for q in step[1]] for step in qc.data if step[0].name!='barrier' and len(step[1])>1]
-    G = nx.Graph()
-    G.add_nodes_from(nodes)
-    G.add_edges_from(edges)
-    if print_graph:
-        nx.draw_kamada_kawai(G)
-    return G
+    return qc
```

### Comparing `symmer-0.0.4/symmer/evolution/exponentiation.py` & `symmer-0.0.5/symmer/evolution/exponentiation.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.4/symmer/evolution/gate_library.py` & `symmer-0.0.5/symmer/evolution/gate_library.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,14 +107,30 @@
 
     Returns:
         PauliwordOp representing the Controlled-X (CX) gate applied to the specified control and target qubits in a system of 'n_qubits' qubits.
     """
     _Had = Had(n_qubits, target)
     return _Had * CZ(n_qubits, control, target) * _Had
 
+def CY(n_qubits:int, control:int, target:int) -> PauliwordOp:
+    """ 
+    Controlled Y gate
+
+    Args:
+        n_qubits (int): Number of qubits.
+        control (int): Qubit index at which will act as a control qubit.
+        target (int): Qubit index at which the operation 'X' has to be applied if the control qubit is in |1> state.
+
+    Returns:
+        PauliwordOp representing the Controlled-X (CX) gate applied to the specified control and target qubits in a system of 'n_qubits' qubits.
+    """
+    _Had = Had(n_qubits, target)
+    _S   = S(n_qubits, target)
+    return _S * _Had * CZ(n_qubits, control, target) * _Had * _S.dagger
+
 def RX(n_qubits:int, index:int, angle:float) -> PauliwordOp:
     """ 
     Rotation-X gate
 
     Args:
         n_qubits (int): Number of qubits.
         index (int): Qubit index at which the operation 'RX' has to be applied.
```

### Comparing `symmer-0.0.4/symmer/evolution/variational_optimization.py` & `symmer-0.0.5/symmer/evolution/variational_optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from cached_property import cached_property
-from qiskit.opflow import CircuitStateFn
+from qiskit.quantum_info import Statevector
 from qiskit import QuantumCircuit
-from symmer import QuantumState, PauliwordOp
+from symmer import process, QuantumState, PauliwordOp
 from symmer.operators.utils import (
     symplectic_to_string, safe_PauliwordOp_to_dict, safe_QuantumState_to_dict
 )
-from symmer.evolution import PauliwordOp_to_QuantumCircuit, get_CNOT_connectivity_graph
+from symmer.evolution import PauliwordOp_to_QuantumCircuit, get_CNOT_connectivity_graph, topology_match_score
 from networkx.algorithms.cycles import cycle_basis
 from scipy.optimize import minimize
 from copy import deepcopy
 import numpy as np
-import multiprocessing as mp
 from typing import *
 
 class VQE_Driver:
     """
     expectation value method one of the following choices:
         - symbolic_direct: uses symmer to compute <psi|H|psi> directly using the QuantumState class
         - symbolic_projector: computes expval by projecting onto +-1 eigenspaces of observable terms
@@ -80,15 +79,15 @@
             - Array (np.array) of the QuantumCircuit (for sparse/dense array methods).
             - Quantum State (QuantumState) representation of the QuantumCircuit (for symbolic methods).
             - Rotations of the form [(generator, angle)] for the observable_rotation expectation_eval method.
         """
         if self.expectation_eval == 'observable_rotation':
             return list(zip(evolution_obj, -2*x))
         else:
-            state = CircuitStateFn(evolution_obj.bind_parameters(x))
+            state = Statevector(evolution_obj.bind_parameters(x))
             if self.expectation_eval == 'dense_array':
                 return state.to_matrix().reshape([-1,1])
             elif self.expectation_eval == 'sparse_array':
                 return state.to_spmatrix().reshape([-1,1])
             elif self.expectation_eval.find('symbolic') != -1:
                 return QuantumState.from_array(state.to_matrix().reshape([-1,1]))
         
@@ -160,19 +159,19 @@
         Args:
             x (np.array): Parameter vector
         
         Returns:
             Ansatz parameter gradient (np.array)
         """
         if self.expectation_eval.find('projector') == -1:
-            with mp.Pool(mp.cpu_count()) as pool:
-                grad_vec = pool.starmap(
-                    self.partial_derivative, 
-                    [(x, i) for i in range(self.circuit.num_parameters)]
-                )
+            @process.parallelize
+            def f(index, param):
+                return self.partial_derivative(param,index)
+            grad_vec = f(range(self.circuit.num_parameters), x)
+
         else:
             grad_vec = [self.partial_derivative(x, i) for i in range(self.circuit.num_parameters)]
         
         return np.asarray(grad_vec)
     
     def run(self, x0:np.array=None, **kwargs):
         """ 
@@ -229,27 +228,29 @@
     variant of ADAPT-VQE (https://doi.org/10.1038/s41467-019-10988-2) that takes 
     its excitation pool as Pauli operators (mapped via some transformation such 
     as Jordan-Wigner) instead of the originating fermionic operators.
 
     Attributes:
         derivative_eval (str): Method which is to be used to calculate the operator pool derivatives.
         TETRIS (bool): If True, TETRIS-ADAPT-VQE is performed. By default it is set to False.
-        linearity_biased (bool): If True, linearity-biased-ADAPT-VQE is performed. By default it is set to True.
-        bias (float): Bias value used in linearity-biased-ADAPT-VQE. It's default value is 1/3.
+        topology_aware (bool): If True, Hardware-Aware ADAPT-VQE is performed. By default it is set to True.
+        topology_bias (float): Bias value used in Hardware-Aware ADAPT-VQE. It's default value is 1.
     """
     # method by which to calculate the operator pool derivatives, either
     # commutators: compute the commutator of the observable with each pool element
     # param_shift: use the parameter shift rule, requiring two expectation values per derivative
     derivative_eval = 'commutators'
     # we have alost implemented TETRIS-ADAPT-VQE as per https://doi.org/10.48550/arXiv.2209.10562
     # that aims to reduce circuit-depth in the ADAPT routine by adding multiple excitation terms
     # per cycle that are supported on distinct qubit positions.
     TETRIS = False
-    linearity_biased = True
-    bias = 1/3
+    topology_aware = True
+    topology_bias = 1
+    topology = None
+    subgraph_match_depth = 3
     
     def __init__(self,
         observable: PauliwordOp,
         excitation_pool: PauliwordOp = None,
         ref_state: QuantumState = None
         ) -> None:
         """
@@ -274,17 +275,19 @@
     def commutators(self) -> List[PauliwordOp]:
         """ 
         List of commutators [H, P] where P is some operator pool element.
 
         Returns:
             List of commutators [H, P]
         """
-        with mp.Pool(mp.cpu_count()) as pool:
-            commutators = pool.map(self.observable.commutator, self.excitation_pool)
-        return list(map(lambda x:x*1j, commutators))
+        @process.parallelize
+        def f(P, obs):
+            return obs.commutator(P)*1j
+        commutators = f(self.excitation_pool, self.observable)
+        return commutators
         
     def _derivative_from_commutators(self, index: int) -> float:
         """ 
         Calculate derivative using the commutator method.
 
         Args:
             index (int): Index
@@ -328,51 +331,47 @@
                 self.current_state = self.get_state(self.adapt_operator, self.opt_parameters)
             else:
                 circuit_temp = PauliwordOp_to_QuantumCircuit(
                     PwordOp=self.adapt_operator, ref_state=self.ref_state, bind_params=False)
                 self.current_state = self.get_state(circuit_temp, self.opt_parameters)
             if self.expectation_eval in ['sparse_array', 'symbolic_direct', 'observable_rotation']:
                 # the commutator method may be parallelized since the state is constant
-                with mp.Pool(mp.cpu_count()) as pool:
-                    gradient = pool.map(self._derivative_from_commutators, range(self.excitation_pool.n_terms))
+                @process.parallelize
+                def f(index, obs):
+                    return obs._derivative_from_commutators(index)
+                gradient = f(range(self.excitation_pool.n_terms), self)
             else:
                 # ... unless using symbolic_projector since this is multiprocessed
                 gradient = list(map(self._derivative_from_commutators, range(self.excitation_pool.n_terms)))
         
         elif self.derivative_eval == 'param_shift':
-            # not parallelizable due the CircuitStateFn already using multiprocessing! 
+            # not parallelizable due the Statevector already using multiprocessing! 
             gradient = list(map(self._derivative_from_param_shift, range(self.excitation_pool.n_terms)))
         
         else:
             raise ValueError('Unrecognised derivative_eval method')
         
         return np.asarray(gradient)
     
     def pool_score(self):
         """ 
-        Score the operator pool with respect to gradients and circuit linearity.
+        Score the operator pool with respect to gradients and topology likeness.
         """
         scores = abs(self.pool_gradient())
 
-        if self.linearity_biased:
-            # linearity-biased-ADAPT-VQE favours circuits with linear qubit connectivity
-            linearity_scores = []
+        if self.topology_aware:
+            assert self.topology is not None, 'No hardware topology specified'
+            # Hardware-Aware ADAPT-VQE favours circuits that match the target topology closely
+            topology_scores = []
             for index in range(self.excitation_pool.n_terms):
                 adapt_op_temp = self.adapt_operator.append(self.excitation_pool[index])
-                circuit_temp = PauliwordOp_to_QuantumCircuit(
-                    PwordOp=adapt_op_temp, ref_state=self.ref_state, bind_params=False)
-                connectivity = get_CNOT_connectivity_graph(circuit_temp)
-                # the presence of cycles in the CNOT connectivity graph is penalised in the score
-                # linear circuits result in a linearity of 1, hence their score is not affected here.
-                linearity_scores.append(
-                    (
-                        circuit_temp.num_qubits - len([a for b in cycle_basis(connectivity) for a in b])*self.bias
-                    ) / circuit_temp.num_qubits
+                topology_scores.append(
+                    topology_match_score(adapt_op_temp, self.topology, max_depth=self.subgraph_match_depth)
                 )
-            scores *= np.array(linearity_scores)
+            scores *= np.power(np.array(topology_scores), self.topology_bias)
         
         return scores
         
     def append_to_adapt_operator(self, excitations_to_append: List[PauliwordOp]):
         """ 
         Append the input term(s) to the expanding adapt_operator.
         """
```

### Comparing `symmer-0.0.4/symmer/operators/anticommuting_op.py` & `symmer-0.0.5/symmer/operators/anticommuting_op.py`

 * *Files 14% similar despite different names*

```diff
@@ -163,62 +163,82 @@
         Returns:
             Ps (PauliwordOp): Pauli operator of term reduced too
             rotations (PauliwordOp): rotations to perform unitary partitioning
             gamma_l (float): normalization constant of clique (anticommuting operator)
             AC_op (AntiCommutingOp): normalized clique - i.e. self == gamma_l * AC_op
         """
         assert up_method in ['LCU', 'seq_rot'], f'unknown unitary partitioning method: {up_method}'
-        AC_op = self.copy()
+
+        if s_index is None:
+            s_index = self.get_least_dense_term_index()
+
+        if np.isclose(self.coeff_vec[s_index], 0):
+            # need to correct for s_index having zero coeff...
+            s_index = np.argmax(abs(self.coeff_vec))
+            warnings.warn(f's indexed term has zero coeff, s_index set to {s_index} so that nonzero operator is rotated onto')
+       
+        s_index = int(s_index)
+        BsPs    = self[s_index]
+
+        # NOTE: term to reduce to is at the top of sym matrix i.e. s_index of ZERO now!
+        no_BsPs = (self - BsPs).cleanup()
+        if (len(no_BsPs.coeff_vec)==1 and no_BsPs.coeff_vec[0]==0):
+            AC_op = BsPs
+        else:
+            AC_op = BsPs.append(no_BsPs)
 
         if AC_op.n_terms == 1:
-            rotations = None
+            rotations = []
             gamma_l = np.linalg.norm(AC_op.coeff_vec)
             AC_op.coeff_vec = AC_op.coeff_vec / gamma_l
-            Ps = PauliwordOp(AC_op.symp_matrix, [1])
-            return Ps, rotations, gamma_l, AC_op
+            Ps = AC_op
+            return Ps, rotations, gamma_l, self.multiply_by_constant(1/gamma_l)
 
         else:
 
             assert np.isclose(np.sum(AC_op.coeff_vec.imag), 0), 'cannot apply unitary partitioning to operator with complex coeffs'
 
             gamma_l = np.linalg.norm(AC_op.coeff_vec)
             AC_op.coeff_vec = AC_op.coeff_vec / gamma_l
 
-            if s_index is None:
-                s_index = self.get_least_dense_term_index()
-
-            if s_index!=0:
-                # re-order so s term is ALWAYS at top of symplectic matrix and thus is index as 0!
-                ### assert s_index <= AC_op.n_terms-1, 's_index out of range'
-                AC_op.coeff_vec[[0, s_index]] = AC_op.coeff_vec[[s_index, 0]]
-                AC_op.symp_matrix[[0, s_index]] = AC_op.symp_matrix[[s_index, 0]]
-                AC_op = AntiCommutingOp(AC_op.symp_matrix, AC_op.coeff_vec) # need to reinit otherwise Z and X blocks wrong
-
-            # assert not np.isclose(AC_op.coeff_vec[0], 0), f's_index cannot have zero coefficent: {AC_op.coeff_vec[0]}'
-            if np.isclose(AC_op[0].coeff_vec, 0):
-                # need to correct for s_index having zero coeff... then need to swap to nonzero index
-                non_zero_index = np.argmax(abs(AC_op.coeff_vec))
-                AC_op.coeff_vec[[0, non_zero_index]] = AC_op.coeff_vec[[non_zero_index, 0]]
-                AC_op.symp_matrix[[0, non_zero_index]] = AC_op.symp_matrix[[non_zero_index, 0]]
-
             if up_method=='seq_rot':
                 if len(self.X_sk_rotations)!=0:
                     self.X_sk_rotations = []
                 Ps = self._recursive_seq_rotations(AC_op)
                 rotations = self.X_sk_rotations
             elif up_method=='LCU':
                 if self.R_LCU is not None:
                     self.R_LCU = None
 
                 Ps = self.generate_LCU_operator(AC_op)
-                rotations = self.R_LCU
+                rotations = LCU_as_seq_rot(self.R_LCU)
             else:
                 raise ValueError(f'unknown unitary partitioning method: {up_method}!')
 
-            return Ps, rotations, gamma_l, AC_op
+            return Ps, rotations, gamma_l, self.multiply_by_constant(1/gamma_l)
+        
+    def multiply_by_constant(self, constant: float) -> "AntiCommutingOp":
+        """ Return AntiCommutingOp under constant multiplication
+        """
+        AC_op_copy = self.copy()
+        AC_op_copy.coeff_vec *= constant
+        return AC_op_copy
+    
+    @classmethod
+    def random(cls, n_qubits: int, n_terms: Union[None, int]=None, apply_clifford=True) -> "AntiCommutingOp":
+        """
+        generate a random real coefficient anticommuting op
+
+        """
+        from symmer.utils import random_anitcomm_2n_1_PauliwordOp
+        if n_terms is None:
+            n_terms = 2*n_qubits+1
+
+        assert n_terms<= 2*n_qubits+1, f'cannot have {n_terms} Pops on {n_qubits} qubits'
+        return cls.from_PauliwordOp( random_anitcomm_2n_1_PauliwordOp(n_qubits, apply_clifford=apply_clifford)[:n_terms])
 
     def generate_LCU_operator(self, AC_op) -> PauliwordOp:
         """
         Given the normalized anticommuting operator object, function takes current symp ordering and
         finds the linear combination of unitaries (LCU) (https://arxiv.org/pdf/1908.08067.pdf) to reduce the operator
         to a single Pauli operator in the operator.
 
@@ -231,139 +251,105 @@
                            least dense Pauli operator in AC operator.
             check_reduction (bool): flag to check reduction by applying LCU on original operator.
 
         Returns:
             R_LCU (PauliwordOp): PauliwordOp that is a linear combination of unitaries
             P_s (PauliwordOp): single PauliwordOp that has been reduced too.
         """
-        # need to remove zero coeff terms
-        AC_op_cpy = AC_op.copy()
-        before_cleanup = AC_op_cpy.n_terms
-        AC_op = AC_op_cpy[np.where(abs(AC_op.coeff_vec)>1e-15)[0]]
-        post_cleanup = AC_op.n_terms
-        # AC_op = AC_op.cleanup(zero_threshold=1e-15)  ## cleanup re-orders which is BAD for s_index
-
-
-        if (before_cleanup>1 and post_cleanup==1):
-            if AC_op.coeff_vec[0]<0:
-                # need to fix neg sign (use Pauli multiplication)
-
-                # as s index defaults to 0, take the next term (in CS-VQE this will commute with symmetries)!
-                if np.isclose(AC_op_cpy[0].coeff_vec, 0):
-                    # need to correct for s_index having zero coeff... then need to swap to nonzero index
-                    non_zero_index = np.argmax(abs(AC_op_cpy.coeff_vec))
-
-                    AC_op_cpy.coeff_vec[[0, non_zero_index]] = AC_op_cpy.coeff_vec[[non_zero_index, 0]]
-                    AC_op_cpy.symp_matrix[[0, non_zero_index]] = AC_op_cpy.symp_matrix[[non_zero_index, 0]]
-
-
-                sign_correction = PauliwordOp(AC_op_cpy.symp_matrix[1],[1])
-
-                self.R_LCU = sign_correction
-                Ps_LCU = PauliwordOp(AC_op.symp_matrix, [1])
-            else:
-                self.R_LCU = PauliwordOp.from_list(['I'*AC_op.n_qubits])
-                Ps_LCU = PauliwordOp(AC_op.symp_matrix, AC_op.coeff_vec)
-        else:
-            s_index=0
-
-            # note gamma_l norm applied on init!
-            Ps_LCU = PauliwordOp(AC_op.symp_matrix[s_index], [1])
-            βs = AC_op.coeff_vec[s_index]
-
-            #  ∑ β_k 𝑃_k  ... note this doesn't contain 𝛽_s 𝑃_s
-            no_βsPs = AC_op - (Ps_LCU.multiply_by_constant(βs))
-
-            # Ω_𝑙 ∑ 𝛿_k 𝑃_k  ... renormalized!
-            omega_l = np.linalg.norm(no_βsPs.coeff_vec)
-            no_βsPs.coeff_vec = no_βsPs.coeff_vec / omega_l
-
-            phi_n_1 = np.arccos(βs)
-            # require sin(𝜙_{𝑛−1}) to be positive...
-            if (phi_n_1 > np.pi):
-                phi_n_1 = 2 * np.pi - phi_n_1
-
-            alpha = phi_n_1
-            I_term = 'I' * Ps_LCU.n_qubits
-            self.R_LCU = PauliwordOp.from_dictionary({I_term: np.cos(alpha / 2)})
-
-            sin_term = -np.sin(alpha / 2)
-
-            for dkPk in no_βsPs:
-                dk_PkPs = dkPk * Ps_LCU
-                self.R_LCU += dk_PkPs.multiply_by_constant(sin_term)
+        ## s_index is ensured to be in zero position in unitary_partitioning method! 
+        ## if using function without this method need to ensure term to rotate onto is the zeroth index of AC_op!
+        s_index=0
+
+        # note gamma_l norm applied on init!
+        Ps_LCU = PauliwordOp(AC_op.symp_matrix[s_index], [1])
+        βs = AC_op.coeff_vec[s_index]
+
+        #  ∑ β_k 𝑃_k  ... note this doesn't contain 𝛽_s 𝑃_s
+        no_βsPs = AC_op - (Ps_LCU.multiply_by_constant(βs))
+
+        # Ω_𝑙 ∑ 𝛿_k 𝑃_k  ... renormalized!
+        omega_l = np.linalg.norm(no_βsPs.coeff_vec)
+        no_βsPs.coeff_vec = no_βsPs.coeff_vec / omega_l
+
+        phi_n_1 = np.arccos(βs)
+        # require sin(𝜙_{𝑛−1}) to be positive...
+        if (phi_n_1 > np.pi):
+            phi_n_1 = 2 * np.pi - phi_n_1
+
+        alpha = phi_n_1
+        I_term = 'I' * Ps_LCU.n_qubits
+        self.R_LCU = PauliwordOp.from_dictionary({I_term: np.cos(alpha / 2)})
+
+        sin_term = -np.sin(alpha / 2)
+
+        for dkPk in no_βsPs:
+            dk_PkPs = dkPk * Ps_LCU
+            self.R_LCU += dk_PkPs.multiply_by_constant(sin_term)
 
         return Ps_LCU
 
-def LCU_as_seq_rot(AC_op: PauliwordOp, include_global_phase_correction=False):
+def LCU_as_seq_rot(R_LCU: PauliwordOp) -> List[Tuple[PauliwordOp, float]]:
     """
     Convert a unitary composed of a
     See equations 18 and 19 of https://arxiv.org/pdf/1907.09040.pdf
-    Note global phase fix is not necessary
+
+    number of rotations is 2*(R_LCU.n_terms-1), which can at most be 4*n_qubits
 
     Args:
-        AC_op (PauliwordOp): unitary composed as a linear combination of anticommuting Pauli operators (excluding identity)
-        include_global_phase_correction (optional): whether to fix global phase to matrix input operator matrix exactly
+        R_LCU (PauliwordOp): unitary composed as a normalized linear combination of imaginary anticommuting Pauli operators (excluding identity)
     Returns:
         expon_p_terms (list): list of rotations generated by Pauli operators to implement AC_op unitary
 
     ** Example use **
 
     from symmer.utils import random_anitcomm_2n_1_PauliwordOp
     from symmer.operators import AntiCommutingOp
     from symmer.evolution.exponentiation import exponentiate_single_Pop
-    from functools import reduce
+    from symmer.utils import product_list
 
     nq = 3 # change (do not make too large as has exp checking cost)
 
     AC_2n1 = random_anitcomm_2n_1_PauliwordOp(nq)
     AC_op = AntiCommutingOp.from_PauliwordOp(AC_2n1)
     Ps_LCU, rotations_LCU, gamma_l, AC_normed = AC_op.unitary_partitioning(s_index=0, up_method= 'LCU')
-    exp_terms = LCU_as_seq_rot(rotations_LCU, include_global_phase_correction=True)
-    print(AC_normed.perform_rotations(exp_terms) == Ps_LCU)
+    print(AC_normed.perform_rotations(rotations_LCU) == Ps_LCU)
 
-    # needs global phase correction here!
-    ## This is expensive operation!
-    check = reduce(lambda a,b: a*b, [exponentiate_single_Pop(x.multiply_by_constant(1j*y/2)) for x, y in exp_terms])
-    print(check == rotations_LCU)
+    ## expensive check to see if operation is identical! should NOT do this when using
+    a2 = product_list([exponentiate_single_Pop(P.multiply_by_constant(1j*angle/2)) for P, angle in rotations_LCU])
+    print(AC_op.R_LCU == a2)
     """
-
-    assert AC_op.n_terms > 1, 'AC_op must have more than 1 term'
-    assert np.isclose(np.linalg.norm(AC_op.coeff_vec), 1), 'AC_op must be l2 normalized'
+    if isinstance(R_LCU, list) and len(R_LCU)==0:
+        # case where there are no rotations
+        return list()
+    
+    assert R_LCU.n_terms > 1, 'AC_op must have more than 1 term'
+    assert np.isclose(np.linalg.norm(R_LCU.coeff_vec), 1), 'AC_op must be l2 normalized'
 
     expon_p_terms = []
 
-    # IF imaginary components the this makes real (but need phase correction later!)
-    coeff_vec = AC_op.coeff_vec.real + AC_op.coeff_vec.imag
-    for k, c_k in enumerate(coeff_vec):
-        P_k = AC_op[k]
+    # # IF imaginary components the this makes real (but need phase correction later!)
+    coeff_vec = R_LCU.coeff_vec.real + R_LCU.coeff_vec.imag
+
+    # for k, c_k in enumerate(coeff_vec):
+    #     P_k = R_LCU[k]
+    #     theta_k = np.arcsin(c_k / np.linalg.norm(coeff_vec[:(k + 1)]))
+    #     P_k.coeff_vec[0] = 1
+    #     expon_p_terms.append(tuple((P_k, theta_k)))
+    # ## phase correction - change angle by -pi in first rotation!
+    # expon_p_terms[0] = (expon_p_terms[0][0], expon_p_terms[0][1]-np.pi)
+
+    for k in range(1, R_LCU.n_terms):
+        P_k = R_LCU[k]
+        c_k = coeff_vec[k]
         theta_k = np.arcsin(c_k / np.linalg.norm(coeff_vec[:(k + 1)]))
         P_k.coeff_vec[0] = 1
         expon_p_terms.append(tuple((P_k, theta_k)))
 
     expon_p_terms = [*expon_p_terms, *expon_p_terms[::-1]]
-
-    ### check
-    # from symmer.evolution.exponentiation import exponentiate_single_Pop
-    # terms = [exponentiate_single_Pop(op.multiply_by_constant(1j*angle/2)) for op,angle in expon_p_terms]
-    # final_op = reduce(lambda x,y: x*y, terms) * PauliwordOp.from_dictionary({'I'*AC_op.n_qubits: -1j})
-    # assert AC_op == final_op
-
-    # in circuit this would be done with Z * Y * X gate series:
-    # global phase correction (not necessary)
-    ## phase_correction = PauliwordOp.from_dictionary({'I'*AC_op.n_qubits: -1j})
-
-    if include_global_phase_correction:
-        ## multiply by -1j Identity term!
-        phase_rot = (PauliwordOp.from_dictionary({'I' * AC_op.n_qubits: 1}), -np.pi)
-        expon_p_terms.append(phase_rot)
-
-        # check1 = reduce(lambda a,b: a*b, [exponentiate_single_Pop(x.multiply_by_constant(1j*y/2)) for x, y in expon_p_terms])
-        # assert check1 == AC_op
-
+    
     return expon_p_terms
 
 # from symmer.operators.utils import mul_symplectic
 # def conjugate_Pop_with_R(Pop:PauliwordOp,
 #                         R: PauliwordOp) -> PauliwordOp:
 #     """
 #     For a defined linear combination of pauli operators : R = ∑_{𝑖} ci Pi ... (note each P self-adjoint!)
```

### Comparing `symmer-0.0.4/symmer/operators/base.py` & `symmer-0.0.5/symmer/operators/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-import os
-import quimb
-from symmer.operators.utils import *
-import ray
+import warnings
 import numpy as np
 import pandas as pd
 import networkx as nx
+import matplotlib.pyplot as plt
+from symmer import process
+from symmer.operators.utils import (
+    matmul_GF2, random_symplectic_matrix, string_to_symplectic, QubitOperator_to_dict, SparsePauliOp_to_dict,
+    symplectic_to_string, cref_binary, check_independent, check_jordan_independent, symplectic_cleanup,
+    check_adjmat_noncontextual, symplectic_to_openfermion, binary_array_to_int, count1_in_int_bitstring
+)
 from tqdm.auto import tqdm
 from copy import deepcopy
 from functools import reduce
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Dict, Tuple
 from numbers import Number
-import multiprocessing as mp
 from cached_property import cached_property
+from scipy.stats import unitary_group
 from scipy.sparse import csr_matrix, csc_matrix, coo_matrix, dok_matrix
-from symmer.operators.utils import _cref_binary
-
 from openfermion import QubitOperator, count_qubits
-import matplotlib.pyplot as plt
-from qiskit.opflow import PauliSumOp as ibm_PauliSumOp
-from scipy.stats import unitary_group
-import warnings
+from qiskit.quantum_info import SparsePauliOp
 warnings.simplefilter('always', UserWarning)
 
 from numba.core.errors import NumbaDeprecationWarning, NumbaPendingDeprecationWarning
 warnings.simplefilter('ignore', category=NumbaDeprecationWarning)
 warnings.simplefilter('ignore', category=NumbaPendingDeprecationWarning)
 
 class PauliwordOp:
@@ -64,14 +63,20 @@
         assert len(self.symp_matrix.shape) == 2, 'symplectic matrix must be 2 dimensional only'
         self.n_qubits = self.symp_matrix.shape[1]//2
         self.coeff_vec = np.asarray(coeff_vec, dtype=complex)
         self.n_terms = self.symp_matrix.shape[0]
         assert(self.n_terms==len(self.coeff_vec)), 'coeff list and Pauliwords not same length'
         self.X_block = self.symp_matrix[:, :self.n_qubits]
         self.Z_block = self.symp_matrix[:, self.n_qubits:]
+
+    def set_processing_method(self, method):
+        """ Set the method to use when running parallelizable processes. 
+        Valid options are: mp, ray, single_thread.
+        """
+        process.method = method
         
     @classmethod
     def random(cls, 
             n_qubits: int, 
             n_terms:  int, 
             diagonal: bool = False, 
             complex_coeffs: bool = True,
@@ -189,27 +194,27 @@
         operator_dict = QubitOperator_to_dict(
             openfermion_op, n_qubits
         )
         return cls.from_dictionary(operator_dict)
 
     @classmethod
     def from_qiskit(cls,
-            qiskit_op: ibm_PauliSumOp
+            qiskit_op: SparsePauliOp
         ) -> "PauliwordOp":
         """ 
-        Initialize a PauliwordOp from Qiskit's PauliSumOp representation.
+        Initialize a PauliwordOp from Qiskit's SparsePauliOp representation.
 
         Args:
-            qiskit_op (ibm_PauliSumOp): The PauliSumOp to initialize from.
+            qiskit_op (SparsePauliOp): The SparsePauliOp to initialize from.
 
         Returns:
             PauliwordOp: A new PauliwordOp object.
         """
-        assert(isinstance(qiskit_op, ibm_PauliSumOp)), 'Must supply a PauliSumOp'
-        operator_dict = PauliSumOp_to_dict(
+        assert(isinstance(qiskit_op, SparsePauliOp)), 'Must supply a SparsePauliOp'
+        operator_dict = SparsePauliOp_to_dict(
             qiskit_op
         )
         return cls.from_dictionary(operator_dict)
 
     @classmethod
     def empty(cls, 
             n_qubits: int
@@ -452,14 +457,16 @@
             key (str, optional): The sorting order. Options are 'increasing' and 'decreasing'. Defaults to 'decreasing'.
 
         Returns:
             PauliwordOp: A new PauliwordOp object with sorted terms.    
         """
         if by == 'magnitude':
             sort_order = np.argsort(-abs(self.coeff_vec))
+        elif by == 'lex':
+            sort_order = np.lexsort(self.symp_matrix.T)
         elif by == 'weight':
             sort_order = np.argsort(-np.sum(self.symp_matrix.astype(int), axis=1))
         elif by == 'support':
             pos_terms_occur = np.logical_or(self.symp_matrix[:, :self.n_qubits], self.symp_matrix[:, self.n_qubits:])
             symp_matrix_view = np.ascontiguousarray(pos_terms_occur).view(
                 np.dtype((np.void, pos_terms_occur.dtype.itemsize * pos_terms_occur.shape[1]))
             )
@@ -635,16 +642,16 @@
 
         Args:
             Pword (PauliwordOp): The PauliwordOp object to compare with.
 
         Returns:
             bool: True if the two PauliwordOp objects are equal, False otherwise.
         """
-        check_1 = self.cleanup()
-        check_2 = Pword.cleanup()
+        check_1 = self.cleanup().sort('lex')
+        check_2 = Pword.cleanup().sort('lex')
         if check_1.n_qubits != check_2.n_qubits:
             raise ValueError('Operators defined over differing numbers of qubits.')
         elif check_1.n_terms != check_2.n_terms:
             return False
         else:
             return (not np.sum(np.logical_xor(check_1.symp_matrix, check_2.symp_matrix)) and
                          np.allclose(check_1.coeff_vec, check_2.coeff_vec))
@@ -745,101 +752,70 @@
             const (complex): The complex constant to multiply by.
 
         Returns:
             PauliwordOp: The result of multiplying the PauliwordOp by the constant.
         """
         return PauliwordOp(self.symp_matrix, self.coeff_vec*const)
 
-    def _mul_symplectic(self, 
-            symp_vec: np.array, 
-            coeff: complex, 
-            Y_count_in: np.array
-        ) -> Tuple[np.array, np.array]:
-        """ 
-        Performs Pauli multiplication with phases at the level of the symplectic 
-        matrices to avoid superfluous PauliwordOp initializations. The phase compensation 
-        is implemented as per https://doi.org/10.1103/PhysRevA.68.042318.
-
-        Args:
-            symp_vec (np.array): The symplectic vector representing the Pauli operator to be multiplied with.
-            coeff (complex): The complex coefficient of the Pauli operator.
-            Y_count_in (np.array): The Y-counts of the input Pauli operator.
-
-        Returns:
-            Tuple[np.array, np.array]: The resulting symplectic vector and coefficient vector after multiplication.
-        """
-        # phaseless multiplication is binary addition in symplectic representation
-        phaseless_prod = np.bitwise_xor(self.symp_matrix, symp_vec)
-        # phase is determined by Y counts plus additional sign flip
-        Y_count_out = np.sum(np.bitwise_and(*np.hsplit(phaseless_prod,2)), axis=1)
-        sign_change = (-1) ** (
-            np.sum(np.bitwise_and(self.X_block, np.hsplit(symp_vec,2)[1]), axis=1) % 2
-        ) # mod 2 as only care about parity
-        # final phase modification
-        phase_mod = sign_change * (1j) ** ((3*Y_count_in + Y_count_out) % 4) # mod 4 as roots of unity
-        coeff_vec = phase_mod * self.coeff_vec * coeff
-        return phaseless_prod, coeff_vec
-
     def _multiply_by_operator(self, 
             PwordOp: Union["PauliwordOp", "QuantumState", complex],
             zero_threshold: float = 1e-15
         ) -> "PauliwordOp":
         """ 
         Right-multiplication of this PauliwordOp by another PauliwordOp or QuantumState ket.
 
+        Performs Pauli multiplication with phases at the level of the symplectic 
+        matrices to avoid superfluous PauliwordOp initializations. The phase compensation 
+        is implemented as per https://doi.org/10.1103/PhysRevA.68.042318.
+
         Args:
             PwordOp (Union["PauliwordOp", "QuantumState", complex]): The operator or ket to multiply by.
             zero_threshold (float): The threshold below which coefficients are considered negligible.
 
         Returns:
             PauliwordOp: The resulting PauliwordOp after multiplication.
         """
         assert (self.n_qubits == PwordOp.n_qubits), 'PauliwordOps defined for different number of qubits'
-
-        if PwordOp.n_terms == 1:
-            # no cleanup if multiplying by a single term (faster)
-            symp_stack, coeff_stack = self._mul_symplectic(
-                symp_vec=PwordOp.symp_matrix, 
-                coeff=PwordOp.coeff_vec, 
-                Y_count_in=self.Y_count+PwordOp.Y_count
-            )
-            pauli_mult_out = PauliwordOp(symp_stack, coeff_stack)
-        else:
-            # multiplication is performed at the symplectic level, before being stacked and cleaned
-            symp_stack, coeff_stack = zip(
-                *[self._mul_symplectic(symp_vec=symp_vec, coeff=coeff, Y_count_in=self.Y_count+Y_count) 
-                for symp_vec, coeff, Y_count in zip(PwordOp.symp_matrix, PwordOp.coeff_vec, PwordOp.Y_count)]
+        Q_symp_matrix = PwordOp.symp_matrix.reshape([PwordOp.n_terms, 1, 2*PwordOp.n_qubits])
+        termwise_phaseless_prod = self.symp_matrix ^ Q_symp_matrix
+        Y_count_in  = self.Y_count + PwordOp.Y_count.reshape(-1,1)
+        Y_count_out = np.sum(termwise_phaseless_prod[:,:,:PwordOp.n_qubits] & termwise_phaseless_prod[:,:,PwordOp.n_qubits:], axis=2)
+        sign_change = (-1) ** (np.sum(self.X_block & Q_symp_matrix[:,:,PwordOp.n_qubits:], axis=2) % 2)
+        phase_mod = sign_change * (1j) ** ((3*Y_count_in + Y_count_out) % 4)
+        return PauliwordOp(
+            *symplectic_cleanup(
+                termwise_phaseless_prod.reshape(-1,2*self.n_qubits), 
+                (phase_mod * np.outer(self.coeff_vec, PwordOp.coeff_vec).T).reshape(-1), zero_threshold=zero_threshold
             )
-            pauli_mult_out = PauliwordOp(
-                *symplectic_cleanup(
-                    np.vstack(symp_stack), np.hstack(coeff_stack), zero_threshold=zero_threshold
-                )
-            )
-        return pauli_mult_out
+        )
     
     def expval(self, psi: "QuantumState") -> complex:
         """ 
         Efficient (linear) expectation value calculation using projectors
         See single_term_expval function below for further details.
 
         Args:
             psi (QuantumState): The quantum state for which to calculate the expectation value.
 
         Returns:
             complex: The expectation value.
         """
-        if self.n_terms > 1:
-            # parallelize if number of terms greater than one
-            psi_ray_store = ray.put(psi)
-            expvals = np.array(ray.get(
-                [single_term_expval.remote(P, psi_ray_store) for P in self]))
+        if self.n_terms > psi.n_terms and psi.n_terms > 10:
+            return (psi.dagger * self * psi).real
         else:
-            expvals = np.array(single_term_expval(self, psi))
+            if self.n_terms > 1:
+                @process.parallelize
+                def f(P, psi):
+                    return single_term_expval(P, psi)
 
-        return np.sum(expvals * self.coeff_vec)
+                expvals = np.array(f(self, psi))
+            else:
+                expvals = np.array(single_term_expval(self, psi))
+
+            return np.sum(expvals * self.coeff_vec).real
 
     def __mul__(self, 
             mul_obj: Union["PauliwordOp", "QuantumState", complex],
             zero_threshold: float = 1e-15
         ) -> "PauliwordOp":
         """ 
         Right-multiplication of this PauliwordOp by another PauliwordOp or QuantumState ket.
@@ -935,15 +911,15 @@
                 start=0
             if stop is None:
                 stop=self.n_terms
             mask = np.arange(start, stop, key.step)
         elif isinstance(key, (list, np.ndarray)):
             mask = np.asarray(key)
         else:
-            raise ValueError('Unrecognised input, must be an integer, slice, list or np.array')
+            raise ValueError(f'Unrecognised input {type(key)}, must be an integer, slice, list or np.array')
         
         symp_items = self.symp_matrix[mask]
         coeff_items = self.coeff_vec[mask]
         return PauliwordOp(symp_items, coeff_items)
 
     def __iter__(self):
         """ 
@@ -980,16 +956,18 @@
         ### sparse code
         # adjacency_matrix = (
         #             csr_matrix(self.symp_matrix.astype(int)) @ csr_matrix(np.hstack((PwordOp.Z_block, PwordOp.X_block)).astype(int)).T)
         # adjacency_matrix.data = ((adjacency_matrix.data % 2) != 0)
         # return np.logical_not(adjacency_matrix.toarray())
 
         ### dense code
-        Omega_PwordOp_symp = np.hstack((PwordOp.Z_block,  PwordOp.X_block)).astype(int)
-        return (self.symp_matrix @ Omega_PwordOp_symp.T) % 2 == 0
+        # Omega_PwordOp_symp = np.hstack((PwordOp.Z_block,  PwordOp.X_block)).astype(int)
+        # return (self.symp_matrix @ Omega_PwordOp_symp.T) % 2 == 0
+        
+        return ~matmul_GF2(self.symp_matrix, np.hstack((PwordOp.Z_block,  PwordOp.X_block)).T)
 
     def anticommutes_termwise(self,
             PwordOp: "PauliwordOp"
         ) -> np.array:
         """
         Args:
             PwordOp (PauliwordOp): The PauliwordOp to check for term-wise anticommutation.
@@ -1061,16 +1039,17 @@
 
         Args:
             PwordOp (PauliwordOp): The PauliwordOp to check for commutation.
 
         Returns:
             bool: True if all terms commute, False otherwise.
         """
-        return self.commutator(PwordOp).n_terms == 0
-    
+        commutator = self.commutator(PwordOp).cleanup()
+        return (commutator.n_terms == 0 or np.all(commutator.coeff_vec[0] == 0))
+        
     @cached_property
     def adjacency_matrix(self) -> np.array:
         """ 
         Checks which terms of self commute within itself.
 
         Returns:
             np.array: Adjacency matrix.
@@ -1087,65 +1066,30 @@
         """
         return self.qubitwise_commutes_termwise(self)
 
     @cached_property
     def is_noncontextual(self) -> bool:
         """ 
         Returns True if the operator is noncontextual, False if contextual
-        Scales as O(N^2), compared with the O(N^3) algorithm of https://doi.org/10.1103/PhysRevLett.123.200501
+        Scales as O(M^2), compared with the O(M^3) algorithm of https://doi.org/10.1103/PhysRevLett.123.200501
+        where M is the number of terms in the operator.
         Constructing the adjacency matrix is by far the most expensive part - very fast once that has been built.
 
         Returns:
             bool: True if the operator is noncontextual, False if contextual.
         """
         if self.n_terms < 4:
+            # all operators with 3 or less P are noncontextual
             return True
-
-        to_reduce = np.vstack([np.hstack([self.Z_block, self.X_block]), np.eye(2 * self.n_qubits, dtype=bool)])
-        cref_matrix = _cref_binary(to_reduce)
-        Z2_symp = cref_matrix[self.n_terms:, np.all(~cref_matrix[:self.n_terms], axis=0)].T
-        Z2_terms = PauliwordOp(Z2_symp, np.ones(Z2_symp.shape[0]))
-
-        if Z2_terms.n_terms < 1:
-            remaining = self.cleanup()
-            if remaining.n_terms > 2 * remaining.n_qubits + 1:
-                # no symmetry component, therefore operator must be made up of pairwise
-                # anticommuting pauli operators to be noncontextual. This can have a max size of 2n+1, if larger cannot
-                # be noncontextual
-                return False
-            else:
-                # for remaining to be noncontextual must be disjoint union of cliques
-                # we can test for this below
-                adj_matrix_view = np.ascontiguousarray(remaining.adjacency_matrix).view(
-                    np.dtype((np.void, remaining.adjacency_matrix.dtype.itemsize * remaining.adjacency_matrix.shape[1]))
-                )
-                re_order_indices = np.argsort(adj_matrix_view.ravel())
-                # sort the adj matrix and vector of coefficients accordingly
-                sorted_terms = remaining.adjacency_matrix[re_order_indices]
-                # unique terms are those with non-zero entries in the adjacent row difference array
-                diff_adjacent = np.diff(sorted_terms, axis=0)
-                mask_unique_terms = np.append(True, np.any(diff_adjacent, axis=1))
-                clique_mask = sorted_terms[mask_unique_terms]
-
-                # check for overlap (array of ones == no overlap)
-                return np.all(np.sum(clique_mask, axis=0) == 1)
-        else:
-
-            _, mask = self.generator_reconstruction(Z2_terms)
-            missing = self[~mask]
-
-            from symmer.utils import get_generators_including_xz_products
-            gens_xyz = get_generators_including_xz_products(missing)
-            gens = missing.generators
-            return check_adjmat_noncontextual(gens.adjacency_matrix) or check_adjmat_noncontextual(gens_xyz.adjacency_matrix)
-
+        return check_adjmat_noncontextual(self.adjacency_matrix)
 
     def _rotate_by_single_Pword(self,
             Pword: "PauliwordOp", 
-            angle: float = None
+            angle: float = None,
+            threshold: float = 1e-18
         ) -> "PauliwordOp":
         """ 
         Let R(t) = e^{i t/2 Q} = cos(t/2)*I + i*sin(t/2)*Q, then one of the following can occur:
         R(t) P R^\dag(t) = P when [P,Q] = 0
         R(t) P R^\dag(t) = cos(t) P + sin(t) (-iPQ) when {P,Q} = 0
 
         This operation is Clifford when t=pi/2, since cos(pi/2) P - sin(pi/2) iPQ = -iPQ.
@@ -1153,18 +1097,25 @@
         
         <!> Please note the definition of the angle in R(t)...
             different implementations could be out by a factor of 2!
 
         Args:
             Pword (PauliwordOp): The Pauliword to rotate by.
             angle (float): The rotation angle in radians. If None, a Clifford rotation (angle=pi/2) is assumed.
-
+            threshold (float): Angle threshold for Clifford rotation (precision to which the angle is a multiple of pi/2)
         Returns:
             PauliwordOp: The rotated operator.
         """
+        if angle is None: # for legacy compatibility
+            angle = np.pi/2
+
+        if angle.imag != 0:
+            warnings.warn('Complex component in angle: this will be ignored.')
+        angle = angle.real
+
         assert(Pword.n_terms==1), 'Only rotation by single Pauliword allowed here'
         if Pword.coeff_vec[0] != 1:
             # non-1 coefficients will affect the sign and angle in the exponent of R(t)
             # imaginary coefficients result in non-unitary R(t)
             Pword_copy = Pword.copy()
             Pword_copy.coeff_vec[0] = 1
             warnings.warn(f'Pword coefficient {Pword.coeff_vec[0]: .8f} has been set to 1')
@@ -1176,23 +1127,33 @@
             # if Pword commutes with self then the rotation has identity action
             return self
         else:
             # note ~commute_vec == not commutes, this indexes the anticommuting terms
             commute_self = PauliwordOp(self.symp_matrix[commute_vec], self.coeff_vec[commute_vec])
             anticom_self = PauliwordOp(self.symp_matrix[~commute_vec], self.coeff_vec[~commute_vec])
 
-            if angle is None:
-                # assumes pi/2 rotation so Clifford
-                anticom_part = (anticom_self*Pword_copy).multiply_by_constant(-1j)
+            multiple = angle * 2 / np.pi
+            int_part = round(multiple)
+            if abs(int_part - multiple)<=threshold:
+                if int_part % 2 == 0:
+                    # no rotation for angle congruent to 0 or pi disregarding sign, fixed in next line
+                    anticom_part = anticom_self
+                else:
+                    # rotation of -pi/2 disregarding sign, fixed in next line
+                    anticom_part = (anticom_self*Pword_copy).multiply_by_constant(-1j)
+                if int_part in [2,3]:
+                    anticom_part = anticom_part.multiply_by_constant(-1)
                 # if rotation is Clifford cannot produce duplicate terms so cleanup not necessary
                 return PauliwordOp(
                     np.vstack([anticom_part.symp_matrix, commute_self.symp_matrix]), 
                     np.hstack([anticom_part.coeff_vec, commute_self.coeff_vec])
                 )
             else:
+                if abs(angle)>1e6:
+                    warnings.warn('Large angle can lead to precision errors: recommend using high-precision math library such as mpmath or redefine angle in range [-pi, pi]')
                 # if angle is specified, performs non-Clifford rotation
                 anticom_part = (anticom_self.multiply_by_constant(np.cos(angle)) + 
                                 (anticom_self*Pword_copy).multiply_by_constant(-1j*np.sin(angle)))
                 return commute_self + anticom_part
                 
     def perform_rotations(self, 
             rotations: List[Tuple["PauliwordOp", float]]
@@ -1208,46 +1169,62 @@
             rotations (List[Tuple[PauliwordOp, float]]): A list of tuples, where each tuple contains a Pauliword
                 to rotate by and the rotation angle in radians. If no angle is given, a Clifford rotation (angle=pi/2) is assumed.
 
         Returns:
             PauliwordOp: The operator after performing the rotations.
         """
         op_copy = self.copy()
-        for pauli_rotation, angle in rotations:
-            op_copy = op_copy._rotate_by_single_Pword(pauli_rotation, angle).cleanup()
-        return op_copy
+        if rotations == []:
+            return op_copy.cleanup()
+        else:
+            for pauli_rotation, angle in rotations:
+                op_copy = op_copy._rotate_by_single_Pword(pauli_rotation, angle).cleanup()
+            return op_copy
 
     def tensor(self, right_op: "PauliwordOp") -> "PauliwordOp":
         """ 
         Tensor current Pauli operator with another on the right (cannot interlace currently).
 
         Args:
             right_op (PauliwordOp): The Pauli operator to tensor with.
 
         Returns:
             PauliwordOp: The resulting Pauli operator after the tensor product.
         """
-        identity_block_right = np.zeros([right_op.n_terms, self.n_qubits]).astype(int)
-        identity_block_left  = np.zeros([self.n_terms,  right_op.n_qubits]).astype(int)
+        identity_block_right = np.zeros([right_op.n_terms, self.n_qubits], dtype=bool)#.astype(int)
+        identity_block_left  = np.zeros([self.n_terms,  right_op.n_qubits], dtype=bool)#.astype(int)
         padded_left_symp = np.hstack([self.X_block, identity_block_left, self.Z_block, identity_block_left])
         padded_right_symp = np.hstack([identity_block_right, right_op.X_block, identity_block_right, right_op.Z_block])
         left_factor = PauliwordOp(padded_left_symp, self.coeff_vec)
         right_factor = PauliwordOp(padded_right_symp, right_op.coeff_vec)
         return left_factor * right_factor
 
     def get_graph(self, 
-            edge_relation = 'C'
+            edge_relation: Optional[str]='C',
+             label_nodes: Optional[bool]=False
         ) -> nx.graph:
-        """ 
-        Build a graph based on edge relation C (commuting), 
-        AC (anticommuting) or QWC (qubitwise commuting).
+        """
+        Build a graph based on edge relation C (commuting), AC (anticommuting) or QWC (qubitwise commuting).
+        Note if label_nodes set to True then node names are pauli operators.
+
+        To draw:
+        import networkx as nx
+        H = PauliwordOp.random(3, 10)
+        graph = H.get_graph(edge_relation='C', label_nodes=True)
+        nx.draw(graph,
+                with_labels = True,
+                alpha=0.75,
+                node_color="skyblue",
+                width=0.1,
+                node_size=750
+        )
 
         Args:
             edge_relation (str): The edge relation to consider. Options are 'C' for commuting, 'AC' for anticommuting, and 'QWC' for qubitwise commuting. Defaults to 'C'.
-
+            label_nodes (bool): flag to label nodes of graph
         Returns:
             nx.Graph: The graph representing the edge relation.
         """
         # build the adjacency matrix for the chosen edge relation
         if edge_relation == 'AC':
             adjmat = ~self.adjacency_matrix.copy()
         elif edge_relation == 'C':
@@ -1255,14 +1232,20 @@
         elif edge_relation == 'QWC':
             adjmat = self.adjacency_matrix_qwc.copy()
         else:
             raise TypeError('Unrecognised edge relation, must be one of C (commuting), AC (anticommuting) or QWC (qubitwise commuting).')
         np.fill_diagonal(adjmat,False) # avoids self-adjacency
         # convert to a networkx graph and perform colouring on complement
         graph = nx.from_numpy_array(adjmat)
+
+        if label_nodes:
+            node_list = np.apply_along_axis(symplectic_to_string, 1, self.symp_matrix).tolist()
+            mapping = dict(zip(range(len(node_list)), node_list))
+            graph = nx.relabel_nodes(graph, mapping)
+
         return graph
 
     def largest_clique(self,
             edge_relation='C'
         ) -> "PauliwordOp":
         """ 
         Return the largest clique w.r.t. the specified edge relation.
@@ -1389,36 +1372,32 @@
 
     @cached_property
     def to_openfermion(self) -> QubitOperator:
         """ 
         Convert to OpenFermion Pauli operator representation.
 
         Returns:
-            QubitOperator: The QubitOperator representation of the PauliwordOp.
+            open_f (QubitOperator): The QubitOperator representation of the PauliwordOp.
         """
-        pauli_terms = []
-        for symp_vec, coeff in zip(self.symp_matrix, self.coeff_vec):
-            pauli_terms.append(
-                QubitOperator(' '.join([Pi+str(i) for i,Pi in enumerate(symplectic_to_string(symp_vec)) if Pi!='I']),
-                coeff)
-            )
-        if len(pauli_terms) == 1:
-            return pauli_terms[0]
-        else:
-            return sum(pauli_terms)
+        open_f = QubitOperator()
+        for P_sym, coeff in zip(self.symp_matrix, self.coeff_vec):
+            open_f+=symplectic_to_openfermion(P_sym, coeff)
+        return open_f
 
     @cached_property
-    def to_qiskit(self) -> ibm_PauliSumOp:
+    def to_qiskit(self) -> SparsePauliOp:
         """ 
         Convert to Qiskit Pauli operator representation.
 
         Returns:
             PauliSumOp: The PauliSumOp representation of the PauliwordOp.
         """
-        return ibm_PauliSumOp.from_list(self.to_dictionary.items())
+        Pstr_list = np.apply_along_axis(symplectic_to_string, 1, self.symp_matrix).tolist()
+
+        return SparsePauliOp(Pstr_list, coeffs=self.coeff_vec.tolist())
 
     @cached_property
     def to_dictionary(self) -> Dict[str, complex]:
         """
         Method for converting the operator from the symplectic representation 
         to a dictionary of the form {P_string:coeff, ...}
 
@@ -1489,15 +1468,15 @@
             from symmer.utils import get_sparse_matrix_large_pauliwordop
             sparse_matrix = get_sparse_matrix_large_pauliwordop(self)
             return sparse_matrix
         else:
             x_int = binary_array_to_int(self.X_block).reshape(-1, 1)
             z_int = binary_array_to_int(self.Z_block).reshape(-1, 1)
 
-            Y_number = np.sum(np.bitwise_and(self.X_block, self.Z_block).astype(int), axis=1)
+            Y_number = np.sum(np.bitwise_and(self.X_block, self.Z_block), axis=1)
             global_phase = (-1j) ** Y_number
 
             dimension = 2 ** self.n_qubits
             row_ind = np.repeat(np.arange(dimension).reshape(1, -1), self.X_block.shape[0], axis=0)
             col_ind = np.bitwise_xor(row_ind, x_int)
 
             row_inds_and_Zint = np.bitwise_and(row_ind, z_int)
@@ -2013,14 +1992,53 @@
             shape = (2**self.n_qubits, 1), 
             dtype=np.complex128
         )
         if self.vec_type == 'bra':
             # conjugate has already taken place, just need to make into row vector
             sparse_Qstate= sparse_Qstate.reshape([1,-1])
         return sparse_Qstate
+    
+    @cached_property
+    def to_dense_matrix(self):
+        """
+        Returns:
+            dense_Qstate (ndarray): dense matrix representation of the statevector
+        """
+        return self.to_sparse_matrix.toarray()
+    
+    def partial_trace_over_qubits(self, qubits: List[int] = []) -> np.ndarray:
+        """
+        Perform a partial trace over the specified qubit positions, 
+        yielding the reduced density matrix of the remaining subsystem.
+
+        Args:
+            qubits (List[int]): qubit indicies to trace over
+
+        Returns:
+            rho_reduced (ndarray): Reduced density matrix over the remaining subsystem
+        """
+        rho_reduced = self.to_dense_matrix.reshape([2]*self.n_qubits)
+        rho_reduced = np.tensordot(rho_reduced, rho_reduced.conj(), axes=(qubits, qubits))
+        d = int(np.sqrt(np.product(rho_reduced.shape)))
+        return rho_reduced.reshape(d, d)
+
+    def get_rdm(self, qubits: List[int] = []) -> np.ndarray:
+        """
+        Return the reduced density matrix of the specified qubit positions, 
+        corresponding with a partial trace over the complementary qubit indices
+        
+        Args:
+            qubits (List[int]): qubit indicies to preserve
+
+        Returns:
+            rho_reduced (ndarray): Reduced density matrix over the chosen subsystem
+        """
+        trace_over_indices = list(set(range(self.n_qubits)).difference(set(qubits)))
+        rho_reduced = self.partial_trace_over_qubits(trace_over_indices)
+        return rho_reduced
 
     def _is_normalized(self) -> bool:
         """
         Check if state is normalized.
 
         Returns:
             bool: True or False depending on if state is normalized.
@@ -2395,24 +2413,15 @@
 
     if return_operator:
         ij_operator = PauliwordOp(ij_symp_matrix, coeffs)
         return ij_operator
     else:
         return ij_symp_matrix, coeffs
 
-@ray.remote(num_cpus=os.cpu_count(),
-            runtime_env={
-                "env_vars": {
-                    "NUMBA_NUM_THREADS": os.getenv("NUMBA_NUM_THREADS"),
-                    # "OMP_NUM_THREADS": str(os.cpu_count()),
-                    "OMP_NUM_THREADS": os.getenv("NUMBA_NUM_THREADS"),
-                    "NUMEXPR_MAX_THREADS": str(os.cpu_count())
-                }
-            }
-            )
+
 def single_term_expval(P_op: PauliwordOp, psi: QuantumState) -> float:
     """ 
     Expectation value calculation for a single Pauli operator given a QuantumState psi
 
     Scales linearly in the number of basis states of psi, versus the quadratic cost of
     evaluating <psi|P|psi> directly, taking into consideration all of the cross-terms.
```

### Comparing `symmer-0.0.4/symmer/operators/independent_op.py` & `symmer-0.0.5/symmer/operators/independent_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
-from typing import Dict, List, Tuple, Union
 import warnings
-import multiprocessing as mp
+from typing import Dict, List, Tuple, Union
+from symmer import process
 from symmer.operators.utils import _rref_binary, _cref_binary, check_independent
 from symmer.operators import PauliwordOp, QuantumState, symplectic_to_string, single_term_expval
-import ray
 
 class IndependentOp(PauliwordOp):
     """ 
     Special case of PauliwordOp, in which the operator terms must
     by algebraically independent, with all coefficients set to integers +/-1.
 
     - stabilizer_rotations
@@ -134,15 +133,15 @@
         else:
             # if any of the stabilizers are not mutually commuting, take the largest commuting subset
             if S.n_terms < 10 or largest_clique:
                 # expensive clique cover finding optimal commuting subset
                 S_commuting = S.largest_clique(edge_relation='C')    
             else:
                 # greedy graph-colouring approach when symmetry basis is large
-                S_commuting = S.clique_cover(edge_relation='C')[0]
+                S_commuting = S.clique_cover(edge_relation='C', strategy='independent_set')[0]
                 warnings.warn('Greedy method may identify non-optimal commuting symmetry terms; might be able to taper again.')
             
             return cls(S_commuting.symp_matrix, np.ones(S_commuting.n_terms, dtype=complex))
 
     def _check_stab(self) -> None:
         """ 
         Checks the stabilizer coefficients are +/-1
@@ -288,25 +287,15 @@
              threshold (float): Threshold Value for  expectation value. It's default value is 0.5
         """
         if not isinstance(ref_state, QuantumState):
             ref_state = QuantumState(ref_state)
         assert ref_state._is_normalized(), 'Reference state is not normalized.'
         
         ### update the stabilizers assignments in parallel
-        # with mp.Pool(mp.cpu_count()) as pool:
-        #     self.coeff_vec = np.array(
-        #         list(pool.starmap(assign_value, [(S, ref_state, threshold) for S in self]))
-        #     )
-        ref_state_ray_store = ray.put(ref_state)
-        self.coeff_vec = np.array(ray.get(
-                        [single_term_expval.remote(S, ref_state_ray_store) for S in self]))
-        # set anything below threshold to be zero
-        self.coeff_vec[np.abs(self.coeff_vec)<threshold] = 0
-        self.coeff_vec = np.sign(self.coeff_vec)
-        
+        self.coeff_vec = np.array(assign_value(self, ref_state))
         # raise a warning if any stabilizers are assigned a zero value
         if np.any(self.coeff_vec==0):
             S_zero = self[self.coeff_vec==0]; S_zero.coeff_vec[:]=1
             S_zero = list(S_zero.to_dictionary.keys())
             warnings.warn(f'The stabilizers {S_zero} were assigned zero values - bad reference state.')
         
     def rotate_onto_single_qubit_paulis(self) -> "IndependentOp":
@@ -362,26 +351,27 @@
         Makes a PauliwordOp instance iterable.
 
         Returns:
             Iterator of PauliwordOp instance.
         """
         return iter([self[i] for i in range(self.n_terms)])
 
-
-def assign_value(S: PauliwordOp, ref_state: QuantumState, threshold: float) -> int:
+@process.parallelize
+def assign_value(S: PauliwordOp, ref_state: QuantumState) -> int:
     """
     Measure expectation value of stabilizer on input reference state.
     Args: 
         S (PauliwordOp): Stabilizer.
         ref_state (QuantumState): Reference State.
         threshold (float): Threshold Value of expectation value.
 
     Returns:
         Expectation Value (int) of stabilizer on input reference state.
     """
+    threshold = 0.5
     expval = single_term_expval(S, ref_state)
     # if this expval exceeds some predefined threshold then assign the corresponding 
     # ±1 eigenvalue. Otherwise, return 0 as insufficient evidence to fix the value.
     if abs(expval) > threshold:
         return int(np.sign(expval))
     else:
         return 0
```

### Comparing `symmer-0.0.4/symmer/operators/noncontextual_op.py` & `symmer-0.0.5/symmer/operators/noncontextual_op.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import warnings
-import os
 import itertools
 import numpy as np
 import networkx as nx
-import multiprocessing as mp
-import qubovert as qv
 from cached_property import cached_property
 from time import time
 from functools import reduce
 from typing import Optional, Union, Tuple, List
 from matplotlib import pyplot as plt
-from scipy.optimize import differential_evolution, shgo
+from scipy.optimize import shgo
 from symmer.operators import PauliwordOp, IndependentOp, AntiCommutingOp, QuantumState
 from symmer.operators.utils import binomial_coefficient, perform_noncontextual_sweep
-import ray
 from symmer.utils import random_anitcomm_2n_1_PauliwordOp
+from symmer import process
 
 class NoncontextualOp(PauliwordOp):
     """ 
     Class for representing noncontextual Hamiltonians
 
     Noncontextual Hamiltonians are precisely those whose terms may be reconstructed 
     under the Jordan product (AB = {A, B}/2) from a generating set of the form 
@@ -248,99 +245,114 @@
         assert generators.is_noncontextual, 'Generating set is contextual.'
         if use_jordan_product:
             _, noncontextual_terms_mask = H.jordan_generator_reconstruction(generators)
         else:
             _, noncontextual_terms_mask = H.generator_reconstruction(generators, override_independence_check=True)
 
         return cls.from_PauliwordOp(H[noncontextual_terms_mask])
-
+    
     @classmethod
     def random(cls,
             n_qubits: int,
             n_cliques:Optional[int]=3,
             complex_coeffs:Optional[bool]=False,
             n_commuting_terms:Optional[int]=None,
+            apply_clifford: Optional[bool] = True,
         ) -> "NoncontextualOp":
         """
         Generate a random Noncontextual operator with normally distributed coefficients.
         Note to maximise size choose number of n_cliques to be 3 (and for 2<= n_cliques <= 5 the operator
         will be larger than only using commuting generators).
+
         WARNING: this function can generates an exponentially large Hamiltonian unless n_terms set.
-        size when NOT set is: n_cliques * [ 2**(n_qubits -  int(np.ceil((n_cliques - 1) / 2))) ]
+        size when NOT set is: n_cliques * [ 2**(n_qubits -  int(np.ceil((n_cliques - 1) / 2))) ] + n_commuting_terms
 
-        Note: The number of terms in output will be: n_cliques*n_commuting_terms
+        Note: The number of terms in output will be: n_cliques*n_commuting_terms + n_commuting_terms
+              apart from when n_commuting_terms=0 in which case = n_cliques
 
         Args:
             n_qubits (int): Number of qubits noncontextual operator defined on
             n_cliques (int): Number of cliques representives in operator
             complex_coeffs (bool): Whether to generate complex coefficients (default: True).
             n_commuting_terms (int): Optional int for number of commuting terms. if not set then it will be: 2**(n_qubits -  int(np.ceil((n_cliques - 1) / 2))) (i.e. exponentially large)
-
+            apply_clifford (bool): Whether to apply clifford before output (to get rid of structure used to build Hnc)
         Returns:
             NoncontextualOp: A random NoncontextualOp object.
         """
-        assert n_cliques > 1, 'number of cliques must be set to 2 or more (cannot have one anticommuting term)'
+        assert n_cliques > 1 or n_cliques == 0, 'number of cliques must be zero or set to 2 or more (cannot have one anticommuting term)'
         n_clique_qubits = int(np.ceil((n_cliques - 1) / 2))
-        assert n_clique_qubits <= n_qubits, 'cannot have {n_cliques} anticommuting cliques on {n_qubits} qubits'
+        assert n_clique_qubits <= n_qubits, f'cannot have {n_cliques} anticommuting cliques on {n_qubits} qubits'
 
         remaining_qubits = n_qubits - n_clique_qubits
 
         if n_commuting_terms:
-            assert n_commuting_terms<= 2**remaining_qubits, f'cannot have {n_commuting_terms} commuting operators on {remaining_qubits} qubits'
+            assert n_commuting_terms <= 2 ** remaining_qubits, f'cannot have {n_commuting_terms} commuting operators on {remaining_qubits} qubits'
+        elif n_qubits == n_clique_qubits:
+            n_commuting_terms = 0
 
-        if remaining_qubits>=1:
-            if n_commuting_terms==None:
+        if remaining_qubits >= 1:
+            if n_commuting_terms == None:
                 n_commuting_terms = 2 ** (remaining_qubits)
                 XZ_block = (((np.arange(n_commuting_terms)[:, None] & (1 << np.arange(2 * remaining_qubits))[
-                                                                            ::-1])) > 0).astype(bool)
+                                                                      ::-1])) > 0).astype(bool)
+            elif n_commuting_terms == 0:
+                XZ_block = np.zeros(2 * remaining_qubits, dtype=bool).reshape([1, -1])
             else:
-                # randomly chooise Z bitstrings in symp matrix:
-                indices = np.unique(np.random.random_integers(0,
-                                                              high=2**remaining_qubits-1,
-                                                              size=10*n_commuting_terms))
-                while len(indices) < n_commuting_terms:
-                    indices = np.unique(np.append(indices,
-                                                  np.unique(np.random.random_integers(0,
-                                                                                      high=2 ** remaining_qubits - 1,
-                                                                                      size=10*n_commuting_terms)))
-                                        )
+                indices = np.random.choice(np.arange(0, 2 ** remaining_qubits),
+                                    size=n_commuting_terms, 
+                                    replace=False)
+                # # randomly chooise Z bitstrings in symp matrix:
+                # indices = np.unique(np.random.random_integers(0,
+                #                                               high=2 ** remaining_qubits - 1,
+                #                                               size=10 * n_commuting_terms))
+                # while len(indices) < n_commuting_terms:
+                #     indices = np.unique(np.append(indices,
+                #                                   np.unique(np.random.random_integers(0,
+                #                                                                       high=2 ** remaining_qubits - 1,
+                #                                                                       size=10 * n_commuting_terms)))
+                #                         )
 
                 indices = indices[:n_commuting_terms]
                 XZ_block = (((indices[:, None] & (1 << np.arange(2 * remaining_qubits))[
-                                                                        ::-1])) > 0).astype(bool)
+                                                 ::-1])) > 0).astype(bool)
 
         if n_cliques == 0:
             H_nc = PauliwordOp(XZ_block, np.ones(XZ_block.shape[0]))
-
         else:
             AC = random_anitcomm_2n_1_PauliwordOp(n_clique_qubits,
                                                   apply_clifford=True)[:n_cliques]
             AC.coeff_vec = np.ones_like(AC.coeff_vec)
             if remaining_qubits >= 1:
                 diag_H = PauliwordOp(XZ_block, np.ones(XZ_block.shape[0]))
             else:
                 diag_H = PauliwordOp.from_list(['I' * remaining_qubits])
 
             AC_full = PauliwordOp.from_list(['I' * remaining_qubits]).tensor(AC)
+
             H_sym = diag_H.tensor(PauliwordOp.from_list(['I' * n_clique_qubits]))
-            H_nc = AC_full * H_sym
-            assert AC.n_terms * n_commuting_terms == H_nc.n_terms, 'operator not largest it can be'
+            if n_commuting_terms > 0:
+                H_nc = AC_full * H_sym + H_sym
+                assert n_commuting_terms*n_cliques + n_commuting_terms == H_nc.n_terms, 'operator not largest it can be'
+            else:
+                H_nc = AC_full * H_sym + H_sym
+                assert AC.n_terms + 1 == H_nc.n_terms, 'operator not largest it can be'
 
         coeff_vec = np.random.randn(H_nc.n_terms).astype(complex)
         if complex_coeffs:
             coeff_vec += 1j * np.random.randn(H_nc.n_terms)
 
-        # apply clifford rotations to get rid of some of generation structure
-        U_cliff_rotations = []
-        for _ in range(n_qubits * 5):
-            P_rand = PauliwordOp.random(H_nc.n_qubits, n_terms=1)
-            P_rand.coeff_vec = [1]
-            U_cliff_rotations.append((P_rand, None))
+        if apply_clifford:
+            # apply clifford rotations to get rid of some of generation structure
+            U_cliff_rotations = []
+            for _ in range(n_qubits * 5):
+                P_rand = PauliwordOp.random(H_nc.n_qubits, n_terms=1)
+                P_rand.coeff_vec = [1]
+                U_cliff_rotations.append((P_rand, (np.pi/2)*np.random.choice([1,3])))
 
-        H_nc = H_nc.perform_rotations(U_cliff_rotations)
+            H_nc = H_nc.perform_rotations(U_cliff_rotations)
 
         return cls(H_nc.symp_matrix, coeff_vec)
 
     @classmethod
     def _from_stabilizers_noncontextual_op(cls, 
             H:PauliwordOp, stabilizers: IndependentOp, use_jordan_product=False
         ) -> "NoncontextualOp":
@@ -403,15 +415,27 @@
         nx.draw(G, pos, edge_color=colors, width=weights, 
                 node_color=node_colour, node_size=node_size, ax=axis)
 
     def noncontextual_generators(self) -> None:
         """ 
         Find an independent generating set for the noncontextual operator.
         """
-        Z2_symmerties = IndependentOp.symmetry_generators(self, commuting_override=True)
+
+        # get Z2 symmetries (may anticommute among themselves)
+        Z2_general = IndependentOp.symmetry_generators(self, commuting_override=True)
+        _, Z2_mask = self.generator_reconstruction(Z2_general)
+        Z2_symmerties = self[Z2_mask].generators
+
+        # then build remaining operator (should be disjoint union of AC cliques now!)
+        _, successful_mask = self.generator_reconstruction(Z2_symmerties)
+        remaining = self[~successful_mask]
+
+        # then build remaining operator (should be disjoint union of AC cliques now as passed NC check!)
+        _, successful_mask = self.generator_reconstruction(Z2_symmerties)
+        remaining = self[~successful_mask]
 
         if not np.all(Z2_symmerties.commutes_termwise(Z2_symmerties)):
             # need to account for Z2_symmerties not commuting with themselves
             sym_gens = self.generators
             # z2_mask = np.sum(sym_gens.adjacency_matrix, axis=1) == sym_gens.n_terms
             z2_mask = np.sum(sym_gens.commutes_termwise(sym_gens), axis=1) == sym_gens.n_terms
 
@@ -501,45 +525,14 @@
             noncon_generators[inds], # index the relevant noncontextual generating elements
             PauliwordOp.from_list(['I'*self.n_qubits]) # initialise product with identity
         ).coeff_vec[0].real
 
         self.pauli_mult_signs = np.array(
             list(map(multiply_indices,jordan_recon_matrix.astype(bool)))
         ).astype(int)
-        
-    def symmetrized_operator(self, expansion_order=1):
-        """ 
-        Get the symmetrized noncontextual operator S_0 - sqrt(S_1^2 + .. S_M^2).
-        In the infinite limit of expansion_order the ground state of this operator
-        will coincide exactly with the true noncontextual operator. This is used
-        for xUSO solver since this reformulation of the Hamiltonian is polynomial.
-
-        Args:
-            expansion_order (int): Expansion order. By default, it is set to 1.
-
-        Returns:
-            Symmetrized noncontextual operator.
-        """
-        Si_list = [self.decomposed['symmetry']]
-        for i in range(self.n_cliques):
-            Ci = self.decomposed[i][0]; Ci.coeff_vec[0]=1
-            Si = Ci*self.decomposed[i]
-            Si_list.append(Si)
-
-        S = sum([Si**2 for Si in Si_list[1:]])
-        norm = np.linalg.norm(S.coeff_vec, ord=1)
-        S *= (1/norm)
-        I = PauliwordOp.from_list(['I'*self.n_qubits])
-        terms = [
-            (I-S)**n * (-1)**n * binomial_coefficient(.5, n) 
-            for n in range(expansion_order+1)
-        ] # power series expansion of the oeprator root
-        S_root = sum(terms) * np.sqrt(norm)
-        
-        return Si_list[0] - S_root
 
     def get_symmetry_contributions(self, nu: np.array) -> float:
         """
         """
         nu = np.asarray(nu)
         coeff_mod =  (
             # coefficient vector whose signs we are modifying:
@@ -549,20 +542,20 @@
             # sign flips from nu assignment:
             (-1)**np.count_nonzero(np.logical_and(self.G_indices==1, nu == -1), axis=1)
         )
         s0 = np.sum(coeff_mod[self.mask_S0]).real
         si = np.array([np.sum(coeff_mod[mask]).real for mask in self.mask_Ci])
         return s0, si
 
-    def get_energy(self, nu: np.array) -> float:
-        """
+    def get_energy(self, nu: np.array, AC_ev: int = -1) -> float:
+        """ 
         The classical objective function that encodes the noncontextual energies.
         """
         s0, si = self.get_symmetry_contributions(nu)
-        return s0 - np.linalg.norm(si)
+        return s0 + AC_ev * np.linalg.norm(si, ord=2)
     
     def update_clique_representative_operator(self, clique_index:int = None) -> List[Tuple[PauliwordOp, float]]:
         _, si = self.get_symmetry_contributions(self.symmetry_generators.coeff_vec)
         self.clique_operator.coeff_vec = si
         if clique_index is None:
             clique_index = 0
         (
@@ -570,151 +563,108 @@
             self.unitary_partitioning_rotations, 
             self.clique_normalization,
             self.clique_operator
         ) = self.clique_operator.unitary_partitioning(up_method=self.up_method, s_index=clique_index)
         
     def solve(self, 
             strategy: str = 'brute_force', 
-            ref_state: np.array = None, 
-            num_anneals:int = 1_000,
-            expansion_order:int = 1
+            ref_state: np.array = None
         ) -> None:
         """ 
         Minimize the classical objective function, yielding the noncontextual 
         ground state. This updates the coefficients of the clique representative 
         operator C(r) and symmetry generators G with the optimal configuration.
 
-        Note: Most QUSO functions/methods work faster than their PUSO counterparts.
-
         Args:
-            strategy (str): Optimization strategy. By default it is set to 'brute_force'. It can be 'brute_force', 'binary_relaxation', 'brute_force_PUSO', 'brute_force_QUSO', 'annealing_PUSO', or 'annealing_QUSO'.
-            ref_state (np.array): Reference State.
-            num_anneals (int): Number of simulated anneals to do.
+            strategy (str): Optimization strategy. By default it is set to 'brute_force'. It can be 'brute_force' or 'binary_relaxation'.
+            ref_state (np.array): Reference State
             expansion_order (int): Expansion order. By default, it is set to 1.
         """
         if ref_state is not None:
             # update the symmetry generator G coefficients w.r.t. the reference state
             self.symmetry_generators.update_sector(ref_state)
             ev_assignment = self.symmetry_generators.coeff_vec
             fixed_ev_mask = ev_assignment!=0
             fixed_eigvals = (ev_assignment[fixed_ev_mask]).astype(int)
             NC_solver = NoncontextualSolver(self, fixed_ev_mask, fixed_eigvals)
             # any remaining unfixed symmetry generators are solved via other means:
         else:
             NC_solver = NoncontextualSolver(self)
 
-        NC_solver.num_anneals = num_anneals
-        NC_solver.expansion_order = expansion_order
-
         if strategy=='brute_force':
             self.energy, nu = NC_solver.energy_via_brute_force()
-
         elif strategy=='binary_relaxation':
             self.energy, nu = NC_solver.energy_via_relaxation()
-        
         else:
-            #### qubovert strategies below this point ####
-            # PUSO = Polynomial unconstrained spin Optimization
-            # QUSO: Quadratic Unconstrained Spin Optimization
-            if strategy == 'brute_force_PUSO':
-                NC_solver.method = 'brute_force'
-                NC_solver.x = 'P'   
-            elif strategy == 'brute_force_QUSO':  
-                NC_solver.method = 'brute_force'
-                NC_solver.x = 'Q'
-            elif strategy == 'annealing_PUSO':
-                NC_solver.method = 'annealing'
-                NC_solver.x = 'P'
-            elif strategy == 'annealing_QUSO':
-                NC_solver.method = 'annealing'
-                NC_solver.x = 'Q'
-            else:
-                raise ValueError(f'Unknown optimization strategy: {strategy}')
-        
-            self.energy, nu = NC_solver.energy_xUSO()
-
+            raise ValueError(f'Unknown optimization strategy: {strategy}')
+    
         # optimize the clique operator coefficients
         self.symmetry_generators.coeff_vec = nu.astype(int)
         if self.n_cliques > 0:
             self.update_clique_representative_operator()
 
-    def noncon_state(self, UP_method:Optional[str]= 'LCU') -> Tuple[QuantumState, np.array]:
+    def noncon_state(self, UP_method = 'LCU') -> Tuple[QuantumState, np.array]:
         """
         Method to generate noncontextual state for current symmetry generators assignments. Note by default
         UP_method is set to LCU as this avoids generating exponentially large states (which seq_rot can do!)
 
         Args:
             UP_method: string of unitary partitioning approach.
 
         Returns:
             state (QuantumState): noncontextual ground state
             nu_assignment (np.array): vector (nu) of expectation value assignments for noncontexutal symmetry generators
 
         """
         nu_assignment = self.symmetry_generators.coeff_vec.copy()
-
         ## update clique coeffs from nu assignment!
         _, si = self.get_symmetry_contributions(nu_assignment)
         self.clique_operator.coeff_vec = si
-
         assert UP_method in ['LCU', 'seq_rot']
-
         if UP_method == 'LCU':
-            Ps, rotations_LCU, gamma_l, AC_normed = self.clique_operator.unitary_partitioning(s_index=0,
-                                                                                                  up_method='LCU')
+            rotations_LCU = self.clique_operator.R_LCU
+            Ps, rotations_LCU, gamma_l, AC_normed = self.clique_operator.unitary_partitioning(s_index=0,up_method='LCU')
         else:
-            Ps, rotations_SEQ, gamma_l, AC_normed = self.clique_operator.unitary_partitioning(s_index=0,
-                                                                                   up_method='seq_rot')
-
+            Ps, rotations_SEQ, gamma_l, AC_normed = self.clique_operator.unitary_partitioning(s_index=0,up_method='seq_rot')
         # choose negative value for clique operator (to minimize energy)
         Ps.coeff_vec[0] = -1
-
         ### to find ground state, need to map noncontextual stabilizers to single qubit Pauli Zs
         independent_stabilizers = self.symmetry_generators + Ps
-
         # rotate onto computational basis
         independent_stabilizers.target_sqp = 'Z'
-
         rotated_stabs = independent_stabilizers.rotate_onto_single_qubit_paulis()
         clifford_rots = independent_stabilizers.stabilizer_rotations
-
         ## get stabilizer state for the rotated stabilizers
-        Z_indices = np.sum(rotated_stabs.Z_block, axis=0)
-        Z_vals = np.sum(rotated_stabs.Z_block[:, Z_indices.astype(bool)] * rotated_stabs.coeff_vec, axis=1)
-        Z_indices[Z_indices.astype(bool)] = ((Z_vals - 1) * -0.5).astype(int)
-
-        state = QuantumState(Z_indices.reshape(1, -1))
-
+        nc_vec = np.zeros(self.n_qubits, dtype=int)
+        for val,row in zip(rotated_stabs.coeff_vec, rotated_stabs.Z_block):
+            assert np.count_nonzero(row) == 1
+            nc_vec[row] = (1-val)/2
+        state = QuantumState(nc_vec)
         ## undo clifford rotations
         from symmer.evolution.exponentiation import exponentiate_single_Pop
-        for op, _ in clifford_rots:
+        for op, _ in clifford_rots[::-1]:
             rot = exponentiate_single_Pop(op.multiply_by_constant(1j * np.pi / 4))
             state = rot.dagger * state
-
         ## undo unitary partitioning step
         if UP_method == 'LCU':
-            state = rotations_LCU.dagger * state
+            state = self.clique_operator.R_LCU.dagger * state
         else:
             for op, angle in rotations_SEQ[::-1]:
                 state = exponentiate_single_Pop(op.multiply_by_constant(1j * angle / 2)).dagger * state
-
         # TODO: could return clifford and UP rotations here too!
-        return state, nu_assignment    
+        return state, nu_assignment
+
 ###############################################################################
 ################### NONCONTEXTUAL SOLVERS BELOW ###############################
 ###############################################################################
 
 class NoncontextualSolver:
 
-    # xUSO settings
     method:str = 'brute_force'
-    x:str = 'P'
-    num_anneals:int = 1_000,
-    _nu = None,
-    expansion_order=1
+    _nu = None
 
     def __init__(
         self,
         NC_op: NoncontextualOp,
         fixed_ev_mask: np.array = None,
         fixed_eigvals: np.array = None
         ) -> None:
@@ -744,22 +694,15 @@
         else:
             search_size = 2**np.sum(~self.fixed_ev_mask)
             nu_list = np.ones([search_size, self.NC_op.symmetry_generators.n_terms], dtype=int)
             nu_list[:,self.fixed_ev_mask] = np.tile(self.fixed_eigvals, [search_size,1])
             nu_list[:,~self.fixed_ev_mask] = np.array(list(itertools.product([-1,1],repeat=np.sum(~self.fixed_ev_mask))))
         
         # # optimize over all discrete value assignments of nu in parallel
-        noncon_H = ray.put(self.NC_op)
-        tracker = np.array(ray.get(
-            [get_noncon_energy.remote(noncon_H, nu_vec) for nu_vec in nu_list]))
-
-        # with mp.Pool(mp.cpu_count()) as pool:
-        #     tracker = pool.map(self.NC_op.get_energy, nu_list)
-        
-        # find the lowest energy eigenvalue assignment from the full list
+        tracker = get_noncon_energy(nu_list, self.NC_op)
         full_search_results = zip(tracker, nu_list)
         energy, fixed_nu = min(full_search_results, key=lambda x:x[0])
 
         return energy, fixed_nu
 
     #################################################################
     ###################### BINARY RELAXATION ########################
@@ -782,116 +725,15 @@
             return nu
 
         optimizer_output = shgo(func=lambda angles:self.NC_op.get_energy(get_nu(angles)), bounds=nu_bounds)
         # if optimization was successful the optimal angles should consist of 0 and pi
         fix_nu = np.sign(np.array(get_nu(np.cos(optimizer_output['x'])))).astype(int)
         self.NC_op.symmetry_generators.coeff_vec = fix_nu 
         return optimizer_output['fun'], fix_nu
-    
-    #################################################################
-    ################ UNCONSTRAINED SPIN OPTIMIZATION ################
-    #################################################################    
-
-    def get_cost_func(self):
-        """ 
-        Define the unconstrained spin cost function.
-        """
-        symmetrized_operator = self.NC_op.symmetrized_operator(expansion_order=self.expansion_order)
-        G_indices, _ = symmetrized_operator.generator_reconstruction(self.NC_op.symmetry_generators)
-        # setup spin variables
-        fixed_indices = np.where(self.fixed_ev_mask)[0] # bool to indices
-        fixed_assignments = dict(zip(fixed_indices, self.fixed_eigvals))
-        q_vec_SPIN={}
-        for ind in range(self.NC_op.symmetry_generators.n_terms):
-            if ind in fixed_assignments.keys():
-                q_vec_SPIN[ind] = fixed_assignments[ind]
-            else:
-                q_vec_SPIN[ind] = qv.spin_var('x%d' % ind)
-
-        COST = 0
-        for P_index, term in enumerate(G_indices):
-            non_zero_inds = term.nonzero()[0]
-            # collect all the spin terms
-            G_term = 1
-            for i in non_zero_inds:
-                G_term *= q_vec_SPIN[i]
-
-            # cost function
-            COST += (
-                G_term * 
-                symmetrized_operator.coeff_vec[P_index].real
-                #self.NC_op.pauli_mult_signs[P_index]# * 
-                #r_part[P_index].real
-            )
-
-        return COST
 
-    def energy_xUSO(self) -> Tuple[float, np.array, np.array]:
-        """
-        Get energy via either: Polynomial unconstrained spin Optimization (x=P)
-                                    or
-                                Quadratic Unconstrained Spin Optimization  (x=Q)
-
-        via a brute force search over q_vector or via simulated annealing
-
-        Note in this method the r_vector is fixed upon input! (aka just does binary optimization)
-
-        Args:
-            NC_op (NoncontextualOp): Non-contextual operator
-            fixed_ev_mask (np.array): bool list of where eigenvalues in nu vector are fixed
-            fixed_eigvals (np.array): list of nu eigenvalues that are fixed
-            method (str): brute force or annealing optimization
-            x (str): Whether method is Polynomial or Quadratic optimization
-            num_anneals (optional): number of simulated anneals to do
 
-        Returns:
-            energy (float): noncontextual energy
-        """
-        assert self.x in ['P', 'Q']
-        assert self.method in ['brute_force', 'annealing']
-        
-        COST = self.get_cost_func()
-        
-        if np.all(self.fixed_ev_mask):
-            # if no degrees of freedom over nu vector, COST is a number
-            nu_vec = self.fixed_eigvals
-        else:
-            if self.x =='P':
-                spin_problem = COST.to_puso()
-            else:
-                spin_problem = COST.to_quso()
-
-            if self.method=='brute_force':
-                sol = spin_problem.solve_bruteforce()
-            elif self.method == 'annealing':
-                if self.x == 'P':
-                    puso_res = qv.sim.anneal_puso(spin_problem, num_anneals=self.num_anneals)
-                elif self.x == 'Q':
-                    puso_res= qv.sim.anneal_quso(spin_problem, num_anneals=self.num_anneals)
-                    assert COST.is_solution_valid(puso_res.best.state) is True
-                sol = puso_res.best.state
-
-            solution = COST.convert_solution(sol)
-            nu_vec = np.ones(self.NC_op.symmetry_generators.n_terms, dtype=int)
-            nu_vec[self.fixed_ev_mask] = self.fixed_eigvals
-            # must ensure the binary variables are correctly ordered in the solution:
-            nu_vec[~self.fixed_ev_mask] = np.array([solution[x_i] for x_i in sorted(COST.variables)])
-        
-        return self.NC_op.get_energy(nu_vec), nu_vec
-
-
-@ray.remote(num_cpus=os.cpu_count(),
-            runtime_env={
-                "env_vars": {
-                    "NUMBA_NUM_THREADS": os.getenv("NUMBA_NUM_THREADS"),
-                    # "OMP_NUM_THREADS": str(os.cpu_count()),
-                    "OMP_NUM_THREADS": os.getenv("NUMBA_NUM_THREADS"),
-                    "NUMEXPR_MAX_THREADS": str(os.cpu_count())
-                }
-            }
-            )
-def get_noncon_energy(noncon_H:NoncontextualOp, nu: np.array) -> float:
+@process.parallelize
+def get_noncon_energy(nu: np.array, noncon_H:NoncontextualOp) -> float:
     """
     The classical objective function that encodes the noncontextual energies.
     """
-    s0, si = noncon_H.get_symmetry_contributions(nu)
-    return s0 - np.linalg.norm(si)
+    return noncon_H.get_energy(nu)
```

### Comparing `symmer-0.0.4/symmer/operators/utils.py` & `symmer-0.0.5/symmer/operators/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,85 @@
 import numpy as np
 import scipy as sp
 from typing import Tuple, Dict
 from openfermion import QubitOperator
-from qiskit.opflow import PauliSumOp
+from qiskit.quantum_info import SparsePauliOp
+from qiskit._accelerate.sparse_pauli_op import unordered_unique
+import numba as nb
+
+def matmul_GF2(A: np.array, B: np.array) -> np.array:
+    """
+    Matrix multiplication mod2, i.e. (A@B)%2. 
+    
+    Note this calls one of two numba functions. First one uses numpy dot functionality, the second
+    does a manual multiplication over GF2 (that is safe for very large matrices)
+
+    Args:
+        A (np.array): boolean numpy array
+        B (np.array): boolean numpy array
+    Returns:
+        matrix multiplication mod 2
+
+    """
+    if max(*A.shape, *B.shape)<2147483648: # 2**31
+        return numba_dot_matmal_GF2(A,B)
+    else:
+        return numba_binary_matmal_GF2(A,B)
+
+@nb.njit(fastmath=True, parallel=True, cache=True)
+def numba_binary_matmal_GF2(A: np.array, B: np.array) -> np.array:
+    """
+    custom GF(2) multiplication using numba. i.e. C = (A@B) mod 2.
+    
+    Note function uses fact that multiplication over GF2 doesn't require sums for each matrix element in C
+    instead it uses and AND operation (same as elementwise multiplicaiton of row,col pairs) 
+    followed by XOR operation (same as taking sum of row,col multiplied pairs)
+    
+    Args:
+        A (np.array): numpy boolean array
+        B (np.array): numpy boolean array
+    Returns:
+        C (np.array): numpy boolean array of (A@B) mod 2
+    """
+    C = np.empty((A.shape[0], B.shape[1]), dtype=np.bool_)
+    for i in nb.prange(C.shape[0]):
+        for j in range(C.shape[1]):
+
+            ## logical version 1 (slower) 
+            # C[i, j] = bool(np.sum(np.logical_and(A[i, :], B[:, j]))%2)
+
+            # # logical version 2 (slower) 
+            # parity = False
+            # for bit in np.logical_and(A[i, :], B[:, j]):
+            #     parity^=bit
+            # C[i, j] = parity
+
+            ## faster loop
+            acc = False
+            for k in range(B.shape[0]):
+                acc ^= A[i, k] & B[k, j]
+            C[i, j] = acc
+    return C
+
+@nb.njit(fastmath=True, cache=True)
+def numba_dot_matmal_GF2(A, B):
+    """
+    Matrix multiplication mod2, i.e. (A@B)%2. Note this function expects boolean input!
+
+    Args:
+        A (np.array): boolean numpy array
+        B (np.array): boolean numpy array
+    Returns:
+        matrix multiplication mod 2
+
+    """
+    return np.asarray(np.dot(np.asarray(A, dtype = np.float64),
+                             np.asarray(B, dtype = np.float64)
+                             )%2, 
+                      dtype = np.bool_)
 
 def symplectic_to_string(symp_vec) -> str:
     """
     Returns string form of symplectic vector defined as (X | Z)
 
     Args:
         symp_vec (array): symplectic Pauliword array
@@ -29,14 +102,45 @@
     char_aray[X_loc] = 'X'
     char_aray[Z_loc] = 'Z'
 
     Pword_string = ''.join(char_aray)
 
     return Pword_string
 
+def symplectic_to_openfermion(symp_vec, coeff) -> str:
+    """Returns string form of symplectic vector defined as (X | Z).
+
+    Args:
+        symp_vec (array): symplectic Pauliword array
+
+    Returns:
+        Pword_string (str): String version of symplectic array
+    """
+    n_qubits = len(symp_vec) // 2
+
+    X_block = symp_vec[:n_qubits]
+    Z_block = symp_vec[n_qubits:]
+
+    Y_loc = np.logical_and(X_block, Z_block)
+    X_loc = np.logical_xor(Y_loc, X_block)
+    Z_loc = np.logical_xor(Y_loc, Z_block)
+
+    char_aray = np.array(list("I" * n_qubits), dtype=str)
+
+    char_aray[Y_loc] = "Y"
+    char_aray[X_loc] = "X"
+    char_aray[Z_loc] = "Z"
+
+    indices = np.array(range(n_qubits), dtype=str)
+    char_aray = np.char.add(char_aray, indices)[np.where(char_aray != "I")[0]]
+
+    Pword_string = " ".join(char_aray)
+
+    return QubitOperator(Pword_string, coeff)
+
 def string_to_symplectic(pauli_str, n_qubits):
     """
     Args:
         pauli_str (str): Pauli String to be converted to symplectic array
         n_qubits (int): Number of qubits
 
     Returns:
@@ -136,36 +240,46 @@
         symp_matrix (np.array): Symplectic matrix.
         coeff_vec (np.array): Coefficient Vector.
         zero_threshold (float): Zero Threshold Value. By default it is set to 'None'.
 
     Returns: 
         Reduced symplectic matrix and reduced coefficient vector.
     """
-    # order lexicographically using a fast void view implementation...
-    # this scales to large numbers of qubits more favourably than np.lexsort
-    symp_matrix_view = np.ascontiguousarray(symp_matrix).view(
-        np.dtype((np.void, symp_matrix.dtype.itemsize * symp_matrix.shape[1]))
-    )
-    re_order_indices = np.argsort(symp_matrix_view.ravel())
-    # sort the symplectic matrix and vector of coefficients accordingly
-    sorted_terms = symp_matrix[re_order_indices]
-    sorted_coeff = coeff_vec[re_order_indices]
-    # unique terms are those with non-zero entries in the adjacent row difference array
-    diff_adjacent = np.diff(sorted_terms, axis=0)
-    mask_unique_terms = np.append(True, np.any(diff_adjacent, axis=1))
-    reduced_symp_matrix = sorted_terms[mask_unique_terms]
-    # mask the term indices such that those which are skipped are summed under np.reduceat
-    summing_indices = np.arange(symp_matrix.shape[0])[mask_unique_terms]
-    reduced_coeff_vec = np.add.reduceat(sorted_coeff, summing_indices, axis=0)
-    # if a zero threshold is specified terms with sufficiently small coefficient will be dropped
+    # # order lexicographically using a fast void view implementation...
+    # # this scales to large numbers of qubits more favourably than np.lexsort
+    # symp_matrix_view = np.ascontiguousarray(symp_matrix).view(
+    #     np.dtype((np.void, symp_matrix.dtype.itemsize * symp_matrix.shape[1]))
+    # )
+    # re_order_indices = np.argsort(symp_matrix_view.ravel())
+    # # sort the symplectic matrix and vector of coefficients accordingly
+    # sorted_terms = symp_matrix[re_order_indices]
+    # sorted_coeff = coeff_vec[re_order_indices]
+    # # unique terms are those with non-zero entries in the adjacent row difference array
+    # diff_adjacent = np.diff(sorted_terms, axis=0)
+    # mask_unique_terms = np.append(True, np.any(diff_adjacent, axis=1))
+    # reduced_symp_matrix = sorted_terms[mask_unique_terms]
+    # # mask the term indices such that those which are skipped are summed under np.reduceat
+    # summing_indices = np.arange(symp_matrix.shape[0])[mask_unique_terms]
+    # reduced_coeff_vec = np.add.reduceat(sorted_coeff, summing_indices, axis=0)
+    # # if a zero threshold is specified terms with sufficiently small coefficient will be dropped
+    # if zero_threshold is not None:
+    #     mask_nonzero = abs(reduced_coeff_vec)>zero_threshold
+    #     reduced_symp_matrix = reduced_symp_matrix[mask_nonzero]
+    #     reduced_coeff_vec = reduced_coeff_vec[mask_nonzero]
+
+    # return reduced_symp_matrix, reduced_coeff_vec
+
+    unique_locations, inverse_map = unordered_unique(symp_matrix.astype('uint16'))
+    reduced_symp_matrix = symp_matrix[unique_locations]
+    reduced_coeff_vec = np.zeros(unique_locations.shape[0], dtype=complex)
+    np.add.at(reduced_coeff_vec, inverse_map, coeff_vec)
     if zero_threshold is not None:
         mask_nonzero = abs(reduced_coeff_vec)>zero_threshold
         reduced_symp_matrix = reduced_symp_matrix[mask_nonzero]
         reduced_coeff_vec = reduced_coeff_vec[mask_nonzero]
-
     return reduced_symp_matrix, reduced_coeff_vec
 
 def random_symplectic_matrix(n_qubits,n_terms, diagonal=False, density=0.3):
     """ 
     Generates a random binary matrix of dimension (n_terms) x (2*n_qubits)
     Specifying diagonal=True will set the left hand side (X_block) to all zeros
     """
@@ -265,28 +379,27 @@
         for i in t:
             letters[i[0]] = i[1]
         p_string = ''.join(letters)        
         op_dict[p_string] = term_dict[t]
          
     return op_dict
 
-def PauliSumOp_to_dict(op:PauliSumOp) -> dict:
+def SparsePauliOp_to_dict(op:SparsePauliOp) -> dict:
     """ 
     Qiskit
     
     Args:
-        op (PauliSumOp): Pauli Sum Operator
+        op (SparsePauliOp): Pauli Sum Operator
 
     Returns:
         Dictionary format of Pauli Sum Operator.
     """
     H_dict = {}
-    for P_term in op.to_pauli_op():
-        Pstr = P_term.primitive.to_label()
-        H_dict[Pstr] = P_term._coeff
+    for Pstr, coeff in op.to_list():
+        H_dict[Pstr] = coeff
     return H_dict
 
 def safe_PauliwordOp_to_dict(op) -> Dict[str, Tuple[float, float]]:
     """ 
     Stores the real and imaginary parts of the coefficient separately in a tuple.
 
     Args:
@@ -394,16 +507,20 @@
     
     Args:
         operators (PauliwordOp): Operators.
 
     Returns:
         Returns True, if input operators contains algebraically dependent terms.
     """
-    check_independent = _rref_binary(operators.symp_matrix)
-    return ~np.any(np.all(~check_independent, axis=1))
+    if operators.n_terms>2*operators.n_qubits:
+        # cannot have indp. set of Pauli operators of more than 2N terms
+        return False
+    else:
+        ind_check = _rref_binary(operators.symp_matrix)
+        return ~np.any(np.all(~ind_check, axis=1))
 
 def check_jordan_independent(operators):
     """ 
     Check if the input PauliwordOp contains algebraically dependent terms under jordan product
     (note input can be noncontextual, but contain dependent terms!)
 
     Args:
@@ -420,88 +537,36 @@
                      'IXII': (1+0j),
                      'XIIX': (1+0j)
                      }
     # clique =  [IIIZ, XIIX]
     # Z2     =  [IIZI, ZIIZ, IXII]
 
     """
-    # mask_symmetries = np.all(operators.adjacency_matrix, axis=1)
-    # Symmetries = operators[mask_symmetries]
-    # Anticommuting = operators[~mask_symmetries]
-    # return (
-    #     check_independent(Symmetries) & 
-    #     np.all(Anticommuting.adjacency_matrix == np.eye(Anticommuting.n_terms))
-    # )
-
-    # if operators.n_terms<= 2*operators.n_qubits+1:
-    #     # check if input is fully anticommuting
-    #     adj_mat = operators.adjacency_matrix
-    #     adj_mat[np.diag_indices_from(adj_mat)] = False
-    #     if np.all(~adj_mat):
-    #         return True
-
-    # Z2_gen_mask = np.sum(operators.commutes_termwise(operators), axis=1) == operators.n_terms
-    # Z2_terms = operators[Z2_gen_mask]
-    #
-    # # find terms not generated these Z2 symmerties
-    # _, z2_mask = operators.generator_reconstruction(Z2_terms, override_independence_check=True)
-    #
-    # ac_terms = operators[~z2_mask]
-    # if ac_terms.n_terms > 0:
-    #     decomposed = ac_terms.clique_cover(edge_relation='C')
-    #     clique_rep_list = [C.sort()[0] for C in decomposed.values()]
-    #     ac_op = sum(clique_rep_list).cleanup()
-    #     # if ac_op.n_terms>0:
-    #     #     assert (np.sum(ac_op.adjacency_matrix.astype(int)
-    #     #                    - np.eye(ac_op.adjacency_matrix.shape[0])) == 0), f'ac_op is not anticommuting: {ac_op}'
-    #     # del ac_op
-    #     if ac_op.n_terms > 0:
-    #         # check all operators anticommute
-    #         adj_mat = ac_op.adjacency_matrix
-    #         adj_mat[np.diag_indices_from(adj_mat)] = False
-    #         if not np.all(~adj_mat):
-    #             return False
-    #
-    #     Z2_from_cliques = sum((decomposed[n] - C_rep) * C_rep for n, C_rep in enumerate(clique_rep_list) if
-    #                           decomposed[n].n_terms > 1)
-    #     if Z2_from_cliques:
-    #         Z2_terms += Z2_from_cliques
-    #
-    #     if not np.all(Z2_terms.commutes_termwise(ac_op)):
-    #         return False
-    #
-    # return check_independent(Z2_terms)
-
-    # get fully commuting terms
-    z2_mask = np.sum(operators.commutes_termwise(operators), axis=1) == operators.n_terms
-    Z2_symm = operators[z2_mask]
-
-    _, missing_mask = operators.generator_reconstruction(Z2_symm, override_independence_check=True)
-    remaining = operators[~missing_mask]
-
-    if remaining.n_terms > 0:
-        # for remaining to be jordan independent remaining must be disjoint union of cliques
-        # we can test for this below
-
-        adj_matrix_view = np.ascontiguousarray(remaining.adjacency_matrix).view(
-            np.dtype((np.void, remaining.adjacency_matrix.dtype.itemsize * remaining.adjacency_matrix.shape[1]))
-        )
-        re_order_indices = np.argsort(adj_matrix_view.ravel())
-        # sort the adj matrix and vector of coefficients accordingly
-        sorted_terms = remaining.adjacency_matrix[re_order_indices]
-        # unique terms are those with non-zero entries in the adjacent row difference array
-        diff_adjacent = np.diff(sorted_terms, axis=0)
-        mask_unique_terms = np.append(True, np.any(diff_adjacent, axis=1))
-        clique_mask = sorted_terms[mask_unique_terms]
+    if operators.n_terms> 3*operators.n_qubits:
+        # cannot have a jordan indp. set larger than 3N
+        ## (e.g. only SINGLE X,Y,Z on every qubit position)
+        ## {XI, ZI, YI, IX, IY, IZ}
+        return False
+
+    # check if globally commuting subset of operators is independent
+    comm_mask = np.sum(operators.commutes_termwise(operators), axis=1) == operators.n_terms
+    comm_part = operators[comm_mask]
+    if not check_independent(comm_part):
+        # commuting subset is not independent
+        ## {YY, XX, ZZ} is example where this would fail! and is why we check here
+        ## as would pass test below
+        return False
+    
+    ## Final check over WHOLE operator to see if jordan indp. (not need to include commuting part! See unit test)
+    # do row reduction where Y terms treated seperately
+    Y_block = np.logical_and(operators.Z_block, operators.X_block)
+    XZY_block = np.hstack((np.logical_xor(operators.X_block, Y_block), np.hstack((np.logical_xor(operators.Z_block, Y_block), Y_block))))
+    ind_check = _rref_binary(XZY_block)
+    return ~np.any(np.all(~ind_check, axis=1))
 
-        # check for overlap (array of ones == no overlap)
-        return np.all(np.sum(clique_mask, axis=0) == 1)
-    else:
-        # operators is made up of pairwise commuting ops and thus must be jordan independent
-        return True
 
 def check_adjmat_noncontextual(adjmat) -> bool:
     """
     Check whether the input boolean square matrix has a noncontextual structure...
     ... see https://doi.org/10.1103/PhysRevLett.123.200501 for details.
 
     Args:
@@ -531,42 +596,28 @@
     Args:
         operator (PauliwordOp): Ordered operator.
 
     Returns:
         List of terms maintaining noncontextuality.
     """
 
-    # # initialize noncontextual operator with first element of input operator
-    # noncon_indices = np.array([0])
-    # adjmat = np.array([[True]], dtype=bool)
-    # for index, term in enumerate(operator[1:]):
-    #     # pad the adjacency matrix term-by-term - avoids full construction each time
-    #     adjmat_vector = np.append(term.commutes_termwise(operator[noncon_indices]), True)
-    #     adjmat_padded = np.pad(adjmat, pad_width=((0, 1), (0, 1)), mode='constant')
-    #     adjmat_padded[-1,:] = adjmat_vector; adjmat_padded[:,-1] = adjmat_vector
-    #     # check whether the adjacency matrix has a noncontextual structure
-    #     if check_adjmat_noncontextual(adjmat_padded):
-    #         noncon_indices = np.append(noncon_indices, index+1)
-    #         adjmat = adjmat_padded
-
-    # return operator[noncon_indices] 
-
-    ## new method uses generators to speed up sweep
-    from symmer.operators import PauliwordOp
-    mask = np.zeros(operator.n_terms, dtype=bool)
-
-    for ind in range(operator.n_terms):
-        mask[ind] = ~mask[ind]
-        running_op = PauliwordOp(operator.symp_matrix[mask],
-                                 np.ones(np.sum(mask)))
-
-        if not running_op.is_noncontextual:
-            mask[ind] = ~mask[ind]
+    # initialize noncontextual operator with first element of input operator
+    noncon_indices = np.array([0])
+    adjmat = np.array([[True]], dtype=bool)
+    for index, term in enumerate(operator[1:]):
+        # pad the adjacency matrix term-by-term - avoids full construction each time
+        adjmat_vector = np.append(term.commutes_termwise(operator[noncon_indices]), True)
+        adjmat_padded = np.pad(adjmat, pad_width=((0, 1), (0, 1)), mode='constant')
+        adjmat_padded[-1,:] = adjmat_vector; adjmat_padded[:,-1] = adjmat_vector
+        # check whether the adjacency matrix has a noncontextual structure
+        if check_adjmat_noncontextual(adjmat_padded):
+            noncon_indices = np.append(noncon_indices, index+1)
+            adjmat = adjmat_padded
 
-    return operator[mask]
+    return operator[noncon_indices] 
 
 def binary_array_to_int(bin_arr):
     """
     Function to convert an array composed of rows of binary into integers.
 
     Args:
         bin_arr(np.array): 2D numpy array of binary.
```

### Comparing `symmer-0.0.4/symmer/projection/base.py` & `symmer-0.0.5/symmer/projection/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from typing import List, Tuple, Union
 from symmer.operators import PauliwordOp, IndependentOp, QuantumState
 from symmer.evolution import trotter, Had
 from functools import reduce
 
-class S3_projection:
+class S3Projection:
     """ 
     Base class for enabling qubit reduction techniques derived from
     the Stabilizer SubSpace (S3) projection framework, such as tapering
     and Contextual-Subspace VQE. The methods defined herein serve the 
     following purposes:
 
     - _perform_projection
@@ -119,15 +119,15 @@
         else:
             op_rotated = operator
         
         self.rotated_flag = True
         # ...and finally perform the stabilizer subspace projection
         return self._perform_projection(operator=op_rotated)
     
-    def project_state(self, state: QuantumState) -> QuantumState:
+    def _project_state(self, state: QuantumState) -> QuantumState:
         """ 
         Project a state into the stabilizer subspace.
 
         Args:
             state (QuantumState): The state which has to be projected into the stabilizer subspace.
 
         Returns: 
@@ -141,15 +141,15 @@
                     self.stabilizers.rotate_onto_single_qubit_paulis().X_block & 
                     ~self.stabilizers.rotate_onto_single_qubit_paulis().Z_block,
                     axis=0
             )
                 )[0]
         ]
         # Projections onto the stabilizer subspace
-        #transformation_list += list(map(lambda x:(x**2 + x)*.5,self.stabilizers.rotate_onto_single_qubit_paulis()))
+        transformation_list += list(map(lambda x:(x**2 + x)*.5,self.stabilizers.rotate_onto_single_qubit_paulis()))
         # Rotations mapping stabilizers onto single-qubit Pauli operators
         transformation_list += list(map(lambda s:trotter(s[0]*(np.pi/4*1j)), self.stabilizers.stabilizer_rotations))
         # Product over the transformation list yields final transformation operator
         transformation = reduce(lambda x,y:x*y, transformation_list)
         # apply transformation to the reference state
         transformed_state = transformation * state
         # drop stabilized qubit positions and sum over potential duplicates
```

### Comparing `symmer-0.0.4/symmer/projection/contextual_subspace.py` & `symmer-0.0.5/symmer/projection/contextual_subspace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,78 @@
 import numpy as np
 from symmer.operators import PauliwordOp, IndependentOp, NoncontextualOp, QuantumState
 from symmer.projection.utils import (
     update_eigenvalues, StabilizerIdentification, ObservableBiasing, stabilizer_walk,
     # get_noncon_generators_from_commuting_stabilizers
 )
-from symmer.projection import S3_projection
+from symmer.projection import S3Projection
 from symmer.evolution import trotter
 from typing import List, Union, Optional
 
-class ContextualSubspace(S3_projection):
+class ContextualSubspace(S3Projection):
     """ 
     Class for performing contextual subspace methods as per https://quantum-journal.org/papers/q-2021-05-14-456/.
     Reduces the number of qubits in the problem while aiming to control the systematic error incurred along the way.
 
     This class handles the following:
     1. Identify a set of operators one wishes to enforce as stabilizers over the contextual subspace,
         one might think ofthese as 'pseudo-symmetries', as opposed to the true, physical symmetries of qubit tapering.
     2. Construct a noncontextual Hamiltoinian that respects the stabilizers selecting in (1),
         the NoncontextualOp class handles the decomposition into a generating set and classical optimization over the noncontextual objective function 
     NOTE: the order in which (1) and (2) are performed depends on the noncontextual strategy specified
     3. Apply unitary partitioning (either sequence of rotations or linear combination of unitaries) to collapse noncontextual cliques
     
-    The remaining steps are handled by the parent S3_projection class:
+    The remaining steps are handled by the parent S3Projection class:
     4. rotate each stabilizer onto a single-qubit Pauli operator, 
     5. drop the corresponding qubits from the Hamiltonian whilst
     6. fixing the +/-1 eigenvalues
     """
+    name = 'contextual_subspace' # for reference in QubitSubspaceManager
+
     def __init__(self,
             operator: PauliwordOp,
             noncontextual_strategy: str = 'diag',
             noncontextual_solver: str = 'brute_force',
-            num_anneals:Optional[int] = 1000,
             unitary_partitioning_method: str = 'seq_rot',
             reference_state: Union[np.array, QuantumState] = None,
-            noncontextual_operator: NoncontextualOp = None,
-            noncontextual_expansion_order: int = 1
+            noncontextual_operator: NoncontextualOp = None
         ):
         """
         When passing in a noncontextual_operator if noncontextual_strategy set to be 'solved' then noncontextual_solver will NOT be run.
 
         Args: 
             operator(PauliwordOp): Operator one wishes to enforce as stabilizers over the contextual subspace.
             noncontextual_strategy (str): Non-Contextual Strategy to be applied. Its default value is'diag'.
             noncontextual_solver (str): Non-contextual solver to be applied. Its default value is'brute_force'.
-            num_anneals (int): Number of simulated anneals to do. By default, it is set to 1000.
             unitary_partitioning_method (str): Unitary Partitioning Method to be applied. Its default value is'seq_rot'.
             reference_state (QuantumState): Reference State. By default, it is set to None.
-            noncontextual_operator (NoncontextualOp): Non-contextual Operator. By default, it is set to None.
-            noncontextual_expansion_order (int): Non-contextual Expansion Order. Its default value is 1.       
+            noncontextual_operator (NoncontextualOp): Non-contextual Operator. By default, it is set to None.    
         """
         # noncontextual startegy will have the form x_y, where x is the actual strategy
         # and y is some supplementary method indicating a sorting key such as magnitude
         if reference_state is None or isinstance(reference_state, QuantumState):
             self.ref_state = reference_state
         else:
             self.ref_state = QuantumState(reference_state)            
         extract_noncon_strat = noncontextual_strategy.split('_')
         self.nc_strategy = extract_noncon_strat[0]
         self.noncontextual_solver = noncontextual_solver
-        self.num_anneals = num_anneals
-        self.noncontextual_expansion_order = noncontextual_expansion_order
         self.unitary_partitioning_method = unitary_partitioning_method
 
         # With the exception of the StabilizeFirst noncontextual strategy, here we build
         # the noncontextual Hamiltonian in line with the specified strategy
         self.operator = operator
         if noncontextual_operator is None and self.nc_strategy != 'StabilizeFirst':
             self.noncontextual_operator = NoncontextualOp.from_hamiltonian(
                 operator, strategy=noncontextual_strategy
             )
-            # solve noncon problem
-            self._noncontextual_update()
-            noncontextual_strategy = 'solved'
         else:
             self.noncontextual_operator = noncontextual_operator
-        
-        ## case for StabilizeFirst when need to solve noncon problem
-        if not noncontextual_strategy == 'solved':
-            self._noncontextual_update()
+        self.unitary_partitioning_method = unitary_partitioning_method
+        self._noncontextual_update()
 
     def manual_stabilizers(self, S: Union[List[str], IndependentOp]) -> None:
         """ 
         Specify a set of operators to enforce manually.
 
         Args:
             S (IndependentOp): Set of Stablizers
@@ -150,20 +141,21 @@
         To be executed each time the noncontextual operator is updated.
         """
         if self.noncontextual_operator is not None:
             self.noncontextual_operator.up_method = self.unitary_partitioning_method
             self.contextual_operator = self.operator - self.noncontextual_operator
             if self.contextual_operator.n_terms == 0:
                 raise ValueError('The Hamiltonian is noncontextual, the contextual subspace is empty.')
-            self.noncontextual_operator.solve(
-                strategy=self.noncontextual_solver, 
-                ref_state=self.ref_state, 
-                num_anneals=self.num_anneals,
-                expansion_order=self.noncontextual_expansion_order
-            )
+            if self.nc_strategy != "solved":
+                self.noncontextual_operator.solve(
+                    strategy=self.noncontextual_solver, 
+                    ref_state=self.ref_state
+                )
+            else:
+                self.noncontextual_operator.update_clique_representative_operator()
             self.n_cliques = self.noncontextual_operator.n_cliques
         
     def _aux_operator_preserving_stabilizer_search(self,
             n_qubits: int,
             aux_operator: PauliwordOp,
             use_X_only: bool = True
         ) -> IndependentOp:
@@ -316,43 +308,34 @@
         """
         # if not supplied with an alternative operator for projection, use the internal operator 
         if operator_to_project is None:
             operator_to_project = self.operator.copy() 
         # if there are no stabilizers, return the input operator
         if self.stabilizers is None:
             return operator_to_project   
-        # instantiate the parent S3_projection class that handles the subspace projection
+        # instantiate the parent S3Projection class that handles the subspace projection
         super().__init__(self.stabilizers)
         self.S3_initialized = True
         # perform unitary partitioning
         if self.perform_unitary_partitioning:
-            # the rotation is implemented differently depending on the choice of LCU or seq_rot
-            if self.noncontextual_operator.up_method=='LCU':
-                # linear-combination-of-unitaries approach
-                rotated_op = (self.noncontextual_operator.unitary_partitioning_rotations * operator_to_project
-                        * self.noncontextual_operator.unitary_partitioning_rotations.dagger).cleanup()
-            elif self.noncontextual_operator.up_method=='seq_rot':
-                # sequence-of-rotations approach
-                rotated_op = operator_to_project.perform_rotations(self.noncontextual_operator.unitary_partitioning_rotations)
-            else:
-                raise ValueError('Unrecognised unitary partitioning rotation method, must be one of LCU or seq_rot.')
+            rotated_op = operator_to_project.perform_rotations(self.noncontextual_operator.unitary_partitioning_rotations)
         else:
             rotated_op = operator_to_project
         # finally, project the operator before returning
         cs_operator = self.perform_projection(rotated_op)
 
         if self.return_NC:
             assert cs_operator.n_qubits == 1, 'Projected operator consists of more than one qubit.'
             cs_operator = NoncontextualOp.from_PauliwordOp(cs_operator)
             cs_operator.solve()
             return cs_operator.energy
         else:
             return cs_operator
 
-    def project_state_onto_subspace(self, 
+    def project_state(self, 
             state_to_project: QuantumState = None
         ) -> QuantumState:
         """ 
         Project a QuantumState into the contextual subspace
 
         Args:
             state_to_project (QuantumState): Quantum State to be projected into the contextual subspace. By default, it is set to None.
@@ -367,16 +350,15 @@
         assert self.S3_initialized, 'Must first project an operator into the contextual subspace via the project_onto_subspace method'
         # can provide an auxiliary state to project, although not in general scalable
         if state_to_project is None:
             assert self.ref_state is not None, 'Must provide a state to project into the contextual subspace'
             state_to_project = self.ref_state
 
         if self.perform_unitary_partitioning:
-            # behaviour is different whether using the LCU or seq_rot UP methods
-            if self.noncontextual_operator.up_method == 'LCU':
-                rotation = self.noncontextual_operator.unitary_partitioning_rotations
-            elif self.noncontextual_operator.up_method == 'seq_rot':
+            if self.noncontextual_operator.unitary_partitioning_rotations == []:
+                rotation = PauliwordOp.from_list(['I'*self.operator.n_qubits])
+            else:
                 rotation_generator = sum([R*angle*.5*1j for R,angle in self.noncontextual_operator.unitary_partitioning_rotations])
                 rotation = trotter(rotation_generator)
-            return self.project_state(rotation * state_to_project)
+            return self._project_state(rotation * state_to_project)
         else:
-            return self.project_state(state_to_project)
+            return self._project_state(state_to_project)
```

### Comparing `symmer-0.0.4/symmer/projection/qubit_subspace_manager.py` & `symmer-0.0.5/symmer/projection/qubit_subspace_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,18 +196,17 @@
             operator (PauliwordOp): Projection of Quantum State.
         """
         assert self._projection_ready, 'Have not yet projected the Hamiltonian into the contextual subspace'
 
         if self._n_qubits < self.hamiltonian.n_qubits:
 
             if self.run_qubit_tapering:
-                state = self.QT.project_state(state)
-            
+                state = self.QT.project_state(state_to_project=state)
             if self.run_contextual_subspace:
-                state = self.CS.project_state_onto_subspace(state_to_project=state)
+                state = self.CS.project_state(state_to_project=state)
 
         return state
```

### Comparing `symmer-0.0.4/symmer/projection/qubit_tapering.py` & `symmer-0.0.5/symmer/projection/qubit_tapering.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import warnings
 
 import numpy as np
 from typing import List, Union
 from cached_property import cached_property
-from symmer.projection import S3_projection
+from symmer.projection import S3Projection
 from symmer.operators import PauliwordOp, IndependentOp, QuantumState
 
-class QubitTapering(S3_projection):
+class QubitTapering(S3Projection):
     """ 
     Class for performing qubit tapering as per https://arxiv.org/abs/1701.08213.
     Reduces the number of qubits in the problem whilst preserving its energy spectrum by:
 
     1. identifying a symmetry of the Hamiltonian,
     2. finding an independent basis therein,
     3. rotating each basis operator onto a single Pauli X, 
     4. dropping the corresponding qubits from the Hamiltonian whilst
     5. fixing the +/-1 eigenvalues
 
-    Steps 1-2 are handled in this class whereas we defer to the parent S3_projection for 3-5.
+    Steps 1-2 are handled in this class whereas we defer to the parent S3Projection for 3-5.
     """
+    name = 'qubit_tapering' # for reference in QubitSubspaceManager
+
     def __init__(self,
             operator: PauliwordOp, 
-            target_sqp: str = 'X'
+            target_sqp: str = 'Z'
         ) -> None:
         """ 
         Input the PauliwordOp we wish to taper.
         There is freedom over the choice of single-qubit Pauli operator we wish to rotate onto, 
         however this is set to X by default (in line with the original tapering paper).
 
         Args: 
@@ -53,15 +55,15 @@
             ref_state: Union[List[int], np.array]=None,
             sector: Union[List[int], np.array]=None,
             aux_operator: PauliwordOp = None
         ) -> PauliwordOp:
         """ 
         Finally, once the symmetry generators and sector have been identified, 
         we may perform a projection onto the corresponding stabilizer subspace via 
-        the parent S3_projection class.
+        the parent S3Projection class.
 
         This method allows one to input an auxiliary operator other than the internal
         operator itself to be tapered consistently with the identified symmetry. This is 
         especially useful when considering an Ansatz defined over the full system that 
         one wishes to restrict to the same stabilizer subspace as the Hamiltonian for 
         use in VQE, for example.
 
@@ -86,19 +88,24 @@
 
         # allow an auxiliary operator (e.g. an Ansatz) to be tapered
         if aux_operator is not None:
             operator_to_taper = aux_operator.copy()
         else:
             operator_to_taper = self.operator.copy()
 
-        # taper the operator via S3_projection.perform_projection
+        # taper the operator via S3Projection.perform_projection
         tapered_operator = self.perform_projection(
             operator=operator_to_taper,
             ref_state=ref_state,
             sector=sector
         )
 
         # if a reference state was supplied, project it into the stabilizer subspace
         if ref_state is not None:
             self.tapered_ref_state = self.project_state(ref_state)
 
         return tapered_operator
+    
+    def project_state(self, state_to_project: QuantumState) -> QuantumState:
+        """
+        """
+        return self._project_state(state_to_project)
```

### Comparing `symmer-0.0.4/symmer/projection/utils.py` & `symmer-0.0.5/symmer/projection/utils.py`

 * *Files identical despite different names*

### Comparing `symmer-0.0.4/symmer/utils.py` & `symmer-0.0.5/symmer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import scipy as sp
 from typing import List, Tuple, Union
 from functools import reduce
 import py3Dmol
 from scipy.sparse import csr_matrix
 from scipy.sparse import kron as sparse_kron
 from symmer.operators.utils import _rref_binary
-import multiprocessing as mp
 import ray
 import os
 # from psutil import cpu_count
 
 def exact_gs_energy(
         sparse_matrix, 
         initial_guess=None, 
@@ -72,14 +71,31 @@
                 )
                 expval_n_particle += Z_coeff * np.sum(sign * np.square(abs(psi.state_op.coeff_vec)))
             if np.round(expval_n_particle) == n_particles:
                 return evl, QuantumState.from_array(evc.reshape([-1,1]))
         # if a solution is not found within the first n_eig eigenvalues then error
         raise RuntimeError('No eigenvector of the correct particle number was identified - try increasing n_eigs.')
 
+def get_entanglement_entropy(psi: QuantumState, qubits: List[int]) -> float:
+    """
+    Get the Von Neumann entropy of the biprtition defined by the specified subsystem 
+    qubit indices and those remaining (i.e. those that will be subsequently traced out)
+
+    Args:
+        psi (QuantumState): the quantum state for which we wish to extract the entanglement entropy
+        qubits (List[int]): the qubit indices to project onto (the remaining qubits will be traced over)
+    
+    Returns:
+        entropy (float): the Von Neumann entropy of the reduced subsystem
+    """
+    reduced = psi.get_rdm(qubits)
+    eigvals, eigvecs = np.linalg.eig(reduced)
+    eigvals = eigvals[eigvals>0]
+    entropy = -np.sum(eigvals*np.log(eigvals)).real
+    return entropy
 
 def random_anitcomm_2n_1_PauliwordOp(n_qubits, complex_coeff=False, apply_clifford=True):
     """ 
     Generate a anticommuting PauliOperator of size 2n+1 on n qubits (max possible size)
     with normally distributed coefficients. Generates in structured way then uses Clifford rotation (default)
     to try and make more random (can stop this to allow FAST build, but inherenet structure
     will be present as operator is formed in specific way!)
@@ -121,18 +137,18 @@
         coeff_vec += 1j * np.random.randn(2 * n_qubits + 1).astype(complex)
 
     P_anticomm = PauliwordOp(ac_symp, coeff_vec)
 
     if apply_clifford:
         # apply clifford rotations to get rid of structure
         U_cliff_rotations = []
-        for _ in range(n_qubits + 5):
+        for _ in range(n_qubits * 5):
             P_rand = PauliwordOp.random(n_qubits, n_terms=1)
             P_rand.coeff_vec = [1]
-            U_cliff_rotations.append((P_rand, None))
+            U_cliff_rotations.append((P_rand, np.random.choice([np.pi/2, -np.pi/2])))
 
         P_anticomm = P_anticomm.perform_rotations(U_cliff_rotations)
 
     assert P_anticomm.n_terms == 2 * n_qubits + 1
 
     ## expensive check
     # anti_comm_check = P_anticomm.adjacency_matrix.astype(int) - np.eye(P_anticomm.adjacency_matrix.shape[0])
@@ -293,15 +309,15 @@
                 }
             }
             )
 def _get_sparse_matrix_large_pauliwordop(P_op: PauliwordOp) -> csr_matrix:
     """
     """
     nq = P_op.n_qubits
-    mat = PauliwordOp.empty(nq).to_sparse_matrix
+    mat = csr_matrix(([], ([],[])), shape=(2**nq,2**nq))
     for op in P_op:
         left_tensor = np.hstack((op.X_block[:, :nq // 2],
                                  op.Z_block[:, :nq // 2]))
         left_coeff = op.coeff_vec
 
         right_tensor = np.hstack((op.X_block[:, nq // 2:],
                                   op.Z_block[:, nq // 2:]))
@@ -396,43 +412,8 @@
     """
     Ps, rot, gamma_l, AC_normed = operator.unitary_partitioning(up_method='LCU')
 
     Ps_root = get_PauliwordOp_root(power, Ps)
 
     AC_root = (rot.dagger * Ps_root * rot).multiply_by_constant(gamma_l ** power)
 
-    return AC_root
-
-
-def get_generators_including_xz_products(operator: PauliwordOp) -> PauliwordOp:
-    """
-    Given an input operator perform similar process to finding generators (but do not use X,Z terms to generate Y terms)
-    i.e. the set can be dependent.
-
-    Args:
-        operator:
-
-    Returns:
-        PauliwordOp of generators build of X,Y,Z terms (note can have dependent terms!)
-
-    """
-    X_only = np.logical_and(operator.X_block, ~operator.Z_block)
-    Z_only = np.logical_and(~operator.X_block, operator.Z_block)
-    Y_only = np.logical_and(operator.Z_block, operator.X_block)
-
-    XZY_block = np.hstack((np.hstack((X_only, Z_only)), Y_only))
-
-    row_red_XYZ = _rref_binary(XZY_block)
-    non_zero_rows = row_red_XYZ[np.sum(row_red_XYZ, axis=1).astype(bool)]
-
-    X_new = non_zero_rows[:, :operator.X_block.shape[1]]
-    Z_new = non_zero_rows[:, operator.X_block.shape[1]:2 * operator.Z_block.shape[1]]
-    Y_new = non_zero_rows[:, 2 * operator.Z_block.shape[1]:]
-
-    sym_final = np.hstack((np.logical_or(X_new, Y_new),
-                           np.logical_or(Z_new, Y_new)))
-
-    # remove duplicates due to same X_new and Z_new positions
-    xyz_gens = PauliwordOp(sym_final, np.ones(sym_final.shape[0])).cleanup()
-    xyz_gens.coeff_vec = np.ones_like(xyz_gens.coeff_vec)
-
-    return xyz_gens
+    return AC_root
```

### Comparing `symmer-0.0.4/PKG-INFO` & `symmer-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: symmer
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 License: MIT
 Author: AlexisRalli
 Author-email: rallilex@hotmail.co.uk
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: black (>=22.1.0,<23.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: black (>=24.3.0,<25.0.0)
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: flake8 (>=4.0.1,<5.0.0)
-Requires-Dist: ipywidgets (>=8.1.0,<9.0.0)
 Requires-Dist: isort (>=5.10.1,<6.0.0)
 Requires-Dist: myst-nb (>=0.17.2,<0.18.0)
 Requires-Dist: ncon (>=1.0.0,<2.0.0)
-Requires-Dist: numba (==0.56)
-Requires-Dist: openfermion (>=1.3.0,<2.0.0)
+Requires-Dist: numba (==0.58.1)
+Requires-Dist: openfermion (>=1.6.1,<2.0.0)
 Requires-Dist: opt-einsum (>=3.3.0,<4.0.0)
-Requires-Dist: py3Dmol (>=1.8.0,<2.0.0)
+Requires-Dist: py3dmol (>=2.0.4,<3.0.0)
 Requires-Dist: pydocstyle (>=6.1.1,<7.0.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
-Requires-Dist: qiskit (>=0.44.0,<0.45.0)
-Requires-Dist: qubovert (>=1.2.5,<2.0.0)
-Requires-Dist: quimb (>=1.5.1,<2.0.0)
-Requires-Dist: ray (>=2.6.3,<3.0.0)
+Requires-Dist: qiskit (==0.46)
+Requires-Dist: quimb (>=1.7.3,<2.0.0)
+Requires-Dist: ray (==2.10)
+Requires-Dist: scipy (==1.9.3)
 Requires-Dist: sphinx-copybutton (>=0.5.2,<0.6.0)
 Requires-Dist: sphinx-design (>=0.5.0,<0.6.0)
+Requires-Dist: urllib3 (==1.26.6)
```

