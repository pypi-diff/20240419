# Comparing `tmp/nz_seqtech-0.2.4.tar.gz` & `tmp/nz_seqtech-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nz_seqtech-0.2.4.tar", last modified: Sat Nov 11 12:51:23 2023, max compression
+gzip compressed data, was "nz_seqtech-0.2.7.tar", last modified: Fri Apr 19 09:02:14 2024, max compression
```

## Comparing `nz_seqtech-0.2.4.tar` & `nz_seqtech-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 12:51:23.492410 nz_seqtech-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-11-11 12:51:23.488410 nz_seqtech-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 12:51:23.488410 nz_seqtech-0.2.4/nz_seqtech/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/nz_seqtech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20097 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/nz_seqtech/classical_ml_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/nz_seqtech/classical_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/nz_seqtech/quantum_dna_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/nz_seqtech/quantum_ml_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-11 12:51:23.488410 nz_seqtech-0.2.4/nz_seqtech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-11-11 12:51:23.000000 nz_seqtech-0.2.4/nz_seqtech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-11-11 12:51:23.000000 nz_seqtech-0.2.4/nz_seqtech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-11 12:51:23.000000 nz_seqtech-0.2.4/nz_seqtech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-11 12:51:23.000000 nz_seqtech-0.2.4/nz_seqtech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-11 12:51:23.000000 nz_seqtech-0.2.4/nz_seqtech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-11 12:51:23.492410 nz_seqtech-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-11-11 12:51:05.000000 nz_seqtech-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:14.374693 nz_seqtech-0.2.7/nz_seqtech/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20097 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/classical_ml_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/classical_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15119 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/quantum_dna_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/quantum_ml_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/nz_seqtech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/setup.py
```

### Comparing `nz_seqtech-0.2.4/LICENSE` & `nz_seqtech-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.4/PKG-INFO` & `nz_seqtech-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nz_seqtech
-Version: 0.2.4
+Version: 0.2.7
 Summary: A library for DNA sequence encoding in quantum machine learning
 Home-page: https://nz-seqtech.com/
 Author: Nouhaila Innan and Muhammad Al-Zafar Khan
 Author-email: nouhaila.innan@zaiku.com, muhammad.khan@zaikugroup.com
 License: Apache
 Project-URL: Documentation, https://nz-seqtech.readthedocs.io/
 Description-Content-Type: text/markdown
```

### Comparing `nz_seqtech-0.2.4/README.md` & `nz_seqtech-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.4/nz_seqtech/__init__.py` & `nz_seqtech-0.2.7/nz_seqtech/__init__.py`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.4/nz_seqtech/classical_ml_models.py` & `nz_seqtech-0.2.7/nz_seqtech/classical_ml_models.py`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.4/nz_seqtech/quantum_dna_encoding.py` & `nz_seqtech-0.2.7/nz_seqtech/quantum_dna_encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,42 +35,43 @@
     # Convert the DNA sequence to uppercase
     dna_seq = dna_seq.upper()
 
     # Check if the DNA sequence is valid
     if not is_valid_dna_seq(dna_seq):
         print("Error: This is not a valid DNA sequence. Please provide a valid DNA sequence.")
         return None
-    dna_seq = dna_seq.upper()
+    
+    # Define encoding for bases
+    encoding_dict = {'A': '00', 'C': '01', 'G': '10', 'T': '11'}
+    
+    # Calculate the number of qubits needed
     n = len(dna_seq)
-    qc = QuantumCircuit(n)
-
-    def encode_bases(base_pair):
-        # Define an encoding scheme for pairs of bases
-        encoding_dict = {
-            'AA': '00', 'AC': '01', 'AG': '10', 'AT': '11',
-            'CA': '00', 'CC': '01', 'CG': '10', 'CT': '11',
-            'GA': '00', 'GC': '01', 'GG': '10', 'GT': '11',
-            'TA': '00', 'TC': '01', 'TG': '10', 'TT': '11'
-        }
-        return encoding_dict[base_pair]
-
-    for i in range(0, n, 2):
-        if i + 1 < n:
-            base_pair = dna_seq[i] + dna_seq[i + 1]
-            encoded_bits = encode_bases(base_pair)
-
-            if encoded_bits[0] == '1':
-                qc.x(i)
-            if encoded_bits[1] == '1':
-                qc.x(i + 1)
-            qc.h([i, i + 1])
+    num_qubits = int(np.ceil(np.log2(n)))
 
-            theta = 2 * np.arcsin(1 / np.sqrt(4))
-            qc.rz(theta, [i, i + 1])
+    # Create the quantum circuit
+    qc = QuantumCircuit(num_qubits)
 
+    # Encode each base of the DNA sequence
+    for i in range(n):
+        base = dna_seq[i]
+        encoded_bits = encoding_dict[base]
+        
+        # Encode each bit of the base
+        for j in range(len(encoded_bits)):
+            if encoded_bits[j] == '1':
+                qc.x(j)
+        
+        # Apply a Hadamard gate to each qubit
+        for j in range(len(encoded_bits)):
+            qc.h(j)
+        
+        # Rotate qubits based on the encoded bits
+        theta = 2 * np.arcsin(1 / np.sqrt(4))
+        qc.rz(theta, list(range(len(encoded_bits))))
+        
     return qc
 #####################################################################################
 #####################################################################################
 def cosine_encoding(dna_seq):
     """
     Encodes a DNA sequence into a quantum state using cosine encoding.
```

### Comparing `nz_seqtech-0.2.4/nz_seqtech/quantum_ml_models.py` & `nz_seqtech-0.2.7/nz_seqtech/quantum_ml_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import pandas as pd
-from sklearn.preprocessing import LabelEncoder
 import numpy as np
 from sklearn.model_selection import train_test_split
-from sklearn.metrics import classification_report
+from sklearn.metrics import classification_report, accuracy_score, confusion_matrix, ConfusionMatrixDisplay
 from qiskit import Aer, QuantumCircuit
-from qiskit.circuit.library import ZZFeatureMap, RealAmplitudes, ZFeatureMap
-import qiskit_algorithms
-from qiskit.algorithms.optimizers import COBYLA
-from qiskit.primitives import Sampler
-from matplotlib import pyplot as plt
-from IPython.display import clear_output
+from qiskit.circuit.library import ZZFeatureMap, RealAmplitudes, ZFeatureMap, PauliFeatureMap
+from qiskit.utils import QuantumInstance, algorithm_globals
 from qiskit_machine_learning.algorithms.classifiers import NeuralNetworkClassifier
 from qiskit_machine_learning.neural_networks import TwoLayerQNN
-from qiskit.utils import algorithm_globals
+from qiskit.algorithms.optimizers import COBYLA, SPSA
+from matplotlib import pyplot as plt
+from IPython.display import clear_output
 import time
 import warnings
 warnings.simplefilter('ignore')
-def suggested_dataset_QNN(random_state=1):
+def suggested_dataset_QNN(random_state=1, num_inputs=2, num_samples=100):
     """
     Generate a suggested dataset for Quantum Neural Networks (QNN).
 
     This function creates a synthetic dataset for binary classification suitable for training Quantum Neural Networks.
     It generates random input samples and assigns binary labels based on the sum of input features.
 
     Parameters:
@@ -28,19 +25,16 @@
 
     Returns:
     tuple: A tuple containing:
         - X (numpy.ndarray): Input data of shape (num_samples, num_inputs), where each row represents a sample
           with `num_inputs` features.
         - y (numpy.ndarray): Binary labels corresponding to the input data, in {-1, +1} format.
     """
-    num_inputs = 2
-    num_samples = 100
     X = 2 * algorithm_globals.random.random([num_samples, num_inputs]) - 1
-    y01 = 1 * (np.sum(X, axis=1) >= 0)  # in { 0,  1}
-    y = 2 * y01 - 1  # in {-1, +1}
+    y = 1 * (np.sum(X, axis=1) >= 0)  # Labels in {0, 1}
     return X, y
 def load_dataset_qnn(X=None, y=None, suggested_data=False, test_size=0.25, random_state=1):
     """
     Load or generate a dataset for Quantum Neural Networks (QNN) training.
 
     This function allows loading a user-provided dataset or generating a suggested synthetic dataset
     for binary classification suitable for training Quantum Neural Networks.
@@ -76,15 +70,16 @@
 
     if len(X.shape) != 2 or len(y.shape) != 1:
         print("The provided data does not have the appropriate format.")
         return None, None
 
     return X, y
 
-def QNN(X=None, y=None, suggested_data=False, test_size=0.25, random_state=1):
+def QNN(X=None, y=None, suggested_data=False, test_size=0.25, random_state=1, 
+        num_iterations=60, feature_map_type='ZZFeatureMap', optimizer_type='COBYLA', print_circuit=False):
     """
     Train a Quantum Neural Network (QNN) classifier using the provided or suggested dataset.
 
     This function utilizes a Quantum Neural Network (QNN) to train a binary classifier. It can either use a
     user-provided dataset or generate a suggested synthetic dataset for training.
 
     Parameters:
@@ -102,51 +97,58 @@
     Note:
     If `suggested_data` is True, the function generates or loads a suggested dataset using the `load_dataset_qnn` function.
     If `suggested_data` is False and `X` and `y` are provided, the function checks the validity of the input data and
     proceeds with training the QNN classifier. If there are issues with the provided data, the function prints an error
     message and returns None.
     """
     if suggested_data:
-        X, y = load_dataset_qnn(suggested_data=True)
-        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
-    else:
-        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
-
-    if X_train is None or y_train is None:
-        print("Data loading failed.")
-        return None
+        X, y = suggested_dataset_QNN(random_state)
+    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
 
-    if len(X_train.shape) != 2 or len(y_train.shape) != 1:
-        print("The provided data does not have the appropriate format.")
-        return None
+    # Callback function for plotting
     objective_func_vals = []
     def callback_graph(weights, obj_func_eval):
         clear_output(wait=True)
         objective_func_vals.append(obj_func_eval)
-        plt.title("Live loss curve")
+        plt.plot(objective_func_vals, color='red')
+        plt.title("Objective Function Value Over Iterations")
         plt.xlabel("Iteration")
-        plt.ylabel("Loss value")
-        plt.plot(range(len(objective_func_vals)), objective_func_vals,color='red')
+        plt.ylabel("Objective Function Value")
         plt.show()
+
+    # Feature map and ansatz selection
+    feature_map = ZZFeatureMap(feature_dimension=X.shape[1], reps=2) if feature_map_type == 'ZZFeatureMap' \
+        else ZFeatureMap(feature_dimension=X.shape[1], reps=2) if feature_map_type == 'ZFeatureMap' \
+        else PauliFeatureMap(feature_dimension=X.shape[1], reps=2)
+    ansatz = RealAmplitudes(X.shape[1], reps=2)
+
+    # Quantum circuit composition
     qc = QuantumCircuit(X.shape[1])
-    feature_map = ZZFeatureMap(X.shape[1],reps=4)
-    ansatz = RealAmplitudes(X.shape[1])
     qc.compose(feature_map, inplace=True)
     qc.compose(ansatz, inplace=True)
-    estimator_qnn = TwoLayerQNN(
-        feature_map=feature_map,
-        ansatz=ansatz,
-        quantum_instance=Aer.get_backend('statevector_simulator'),
-    )
-    estimator_classifier = NeuralNetworkClassifier(
-        estimator_qnn, optimizer=COBYLA(maxiter=200), callback=callback_graph
-    )
-    start = time.time()
+
+    # Estimator and classifier setup
+    optimizer = COBYLA(maxiter=num_iterations) if optimizer_type == 'COBYLA' else SPSA(maxiter=num_iterations)
+    estimator_qnn = TwoLayerQNN(feature_map=feature_map, ansatz=ansatz,
+                                quantum_instance=Aer.get_backend('statevector_simulator'))
+    estimator_classifier = NeuralNetworkClassifier(estimator_qnn, optimizer=optimizer, callback=callback_graph)
+
+    # Model training
+    start_time = time.time()
     estimator_classifier.fit(X_train, y_train)
-    elapsed = time.time() - start
-    y_pred_test = estimator_classifier.predict(X_test)  
-    test_score_qnn = np.mean(y_pred_test == y_test)
-    #training_time_str = "The training time: {:.2f} s".format(elapsed)
-    test_score_qnn = np.mean(y_pred_test == y_test)
-    report = classification_report(y_test, y_pred_test)
-    x=print("Classification Report:\n", report)  # Print the classification report
-    return x
+    training_time = time.time() - start_time
+
+    # Predictions and evaluation
+    y_pred_test = estimator_classifier.predict(X_test)
+    accuracy = accuracy_score(y_test, y_pred_test)
+    cm = confusion_matrix(y_test, y_pred_test, labels=[0, 1])
+    disp = ConfusionMatrixDisplay(confusion_matrix=cm, display_labels=[0, 1])
+    if print_circuit:
+        print(qc.draw()) 
+    # Reporting
+    print(f"Training time: {training_time:.2f} seconds")
+    print(f"Accuracy: {accuracy:.2f}")
+    print("Classification Report:")
+    print(classification_report(y_test, y_pred_test, labels=[0, 1]))
+    disp.plot(cmap=plt.cm.Blues)
+    plt.title('Confusion Matrix')
+    plt.show()
```

### Comparing `nz_seqtech-0.2.4/nz_seqtech.egg-info/PKG-INFO` & `nz_seqtech-0.2.7/nz_seqtech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nz-seqtech
-Version: 0.2.4
+Name: nz_seqtech
+Version: 0.2.7
 Summary: A library for DNA sequence encoding in quantum machine learning
 Home-page: https://nz-seqtech.com/
 Author: Nouhaila Innan and Muhammad Al-Zafar Khan
 Author-email: nouhaila.innan@zaiku.com, muhammad.khan@zaikugroup.com
 License: Apache
 Project-URL: Documentation, https://nz-seqtech.readthedocs.io/
 Description-Content-Type: text/markdown
```

### Comparing `nz_seqtech-0.2.4/setup.py` & `nz_seqtech-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #with open("README.md", 'r', encoding='utf-8') as f:
     #long_description = f.read()
 with open("README.md") as readme:
     long_description = readme.read()    
     
 setup(
     name='nz_seqtech',
-    version='0.2.4',
+    version='0.2.7',
     license='Apache',
     description='A library for DNA sequence encoding in quantum machine learning',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url ='https://nz-seqtech.com/',
     author='Nouhaila Innan and Muhammad Al-Zafar Khan',
     author_email='nouhaila.innan@zaiku.com, muhammad.khan@zaikugroup.com',
```

