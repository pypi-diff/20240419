# Comparing `tmp/breastcancermlpmodel-0.0.30.tar.gz` & `tmp/breastcancermlpmodel-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breastcancermlpmodel-0.0.30.tar", last modified: Fri Apr 19 19:24:26 2024, max compression
+gzip compressed data, was "breastcancermlpmodel-0.0.31.tar", last modified: Fri Apr 19 19:34:04 2024, max compression
```

## Comparing `breastcancermlpmodel-0.0.30.tar` & `breastcancermlpmodel-0.0.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 19:24:26.876987 breastcancermlpmodel-0.0.30/
-drwxrwxrwx   0        0        0        0 2024-04-19 19:24:26.873787 breastcancermlpmodel-0.0.30/BreastCancerMLPModel.egg-info/
--rw-rw-rw-   0        0        0     3874 2024-04-19 19:24:26.000000 breastcancermlpmodel-0.0.30/BreastCancerMLPModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-19 19:24:26.000000 breastcancermlpmodel-0.0.30/BreastCancerMLPModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 19:24:26.000000 breastcancermlpmodel-0.0.30/BreastCancerMLPModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-19 19:24:26.000000 breastcancermlpmodel-0.0.30/BreastCancerMLPModel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-19 19:24:26.000000 breastcancermlpmodel-0.0.30/BreastCancerMLPModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3874 2024-04-19 19:24:26.874786 breastcancermlpmodel-0.0.30/PKG-INFO
--rw-rw-rw-   0        0        0     3061 2024-04-19 18:09:35.000000 breastcancermlpmodel-0.0.30/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 19:24:26.860282 breastcancermlpmodel-0.0.30/mlp_breast_cancer_diagnosis/
--rw-rw-rw-   0        0        0        0 2024-04-19 17:47:39.000000 breastcancermlpmodel-0.0.30/mlp_breast_cancer_diagnosis/__init__.py
--rw-rw-rw-   0        0        0     7451 2024-04-19 19:15:50.000000 breastcancermlpmodel-0.0.30/mlp_breast_cancer_diagnosis/mlp_model.py
--rw-rw-rw-   0        0        0       42 2024-04-19 19:24:26.876987 breastcancermlpmodel-0.0.30/setup.cfg
--rw-rw-rw-   0        0        0     1727 2024-04-19 19:24:08.000000 breastcancermlpmodel-0.0.30/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 19:24:26.871122 breastcancermlpmodel-0.0.30/tests/
--rw-rw-rw-   0        0        0     2205 2024-04-19 19:14:26.000000 breastcancermlpmodel-0.0.30/tests/test_mlp_model.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:34:04.362318 breastcancermlpmodel-0.0.31/
+drwxrwxrwx   0        0        0        0 2024-04-19 19:34:04.338011 breastcancermlpmodel-0.0.31/BreastCancerMLPModel/
+-rw-rw-rw-   0        0        0     7548 2024-04-19 19:32:46.000000 breastcancermlpmodel-0.0.31/BreastCancerMLPModel/BreastCancerMLPModel.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 17:47:39.000000 breastcancermlpmodel-0.0.31/BreastCancerMLPModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:34:04.360463 breastcancermlpmodel-0.0.31/BreastCancerMLPModel.egg-info/
+-rw-rw-rw-   0        0        0    10212 2024-04-19 19:34:03.000000 breastcancermlpmodel-0.0.31/BreastCancerMLPModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-04-19 19:34:04.000000 breastcancermlpmodel-0.0.31/BreastCancerMLPModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 19:34:03.000000 breastcancermlpmodel-0.0.31/BreastCancerMLPModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-19 19:34:03.000000 breastcancermlpmodel-0.0.31/BreastCancerMLPModel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-19 19:34:04.000000 breastcancermlpmodel-0.0.31/BreastCancerMLPModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10212 2024-04-19 19:34:04.362318 breastcancermlpmodel-0.0.31/PKG-INFO
+-rw-rw-rw-   0        0        0     9399 2024-04-19 19:26:43.000000 breastcancermlpmodel-0.0.31/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 19:34:04.362318 breastcancermlpmodel-0.0.31/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2024-04-19 19:33:16.000000 breastcancermlpmodel-0.0.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 19:34:04.357463 breastcancermlpmodel-0.0.31/tests/
+-rw-rw-rw-   0        0        0     2209 2024-04-19 19:29:40.000000 breastcancermlpmodel-0.0.31/tests/test_mlp_model.py
```

### Comparing `breastcancermlpmodel-0.0.30/mlp_breast_cancer_diagnosis/mlp_model.py` & `breastcancermlpmodel-0.0.31/BreastCancerMLPModel/BreastCancerMLPModel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 from sklearn.neural_network import MLPClassifier
 from sklearn.preprocessing import StandardScaler
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
-import numpy as np
-
-from sklearn.datasets import load_breast_cancer
-from sklearn.model_selection import train_test_split
-from sklearn.neural_network import MLPClassifier
-from sklearn.preprocessing import StandardScaler
 from sklearn.metrics import accuracy_score, confusion_matrix
 import numpy as np
 
 class BreastCancerMLPModel:
     def __init__(self):
         """
         Initialize the BreastCancerMLPModel.
@@ -68,30 +62,35 @@
         X = breast_cancer.data
         y = breast_cancer.target
 
         # Split the dataset into training and test sets
         X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 
         # Scale features
-        # Scale the features to ensure they are on the same scale
         X_train_scaled = self.scaler.fit_transform(X_train)
         X_test_scaled = self.scaler.transform(X_test)
 
         # Train the model
         self.model.fit(X_train_scaled, y_train)
 
         # Evaluate the model
-        train_accuracy = self.model.score(X_train_scaled, y_train)
-        test_accuracy = self.model.score(X_test_scaled, y_test)
+        train_accuracy = accuracy_score(y_train, self.model.predict(X_train_scaled))
+        test_accuracy = accuracy_score(y_test, self.model.predict(X_test_scaled))
         
         # Print results
         print("Model trained successfully.")
         print("Train Accuracy:", train_accuracy)
         print("Test Accuracy:", test_accuracy)
 
+        # Calculate and print confusion matrix
+        train_conf_matrix = confusion_matrix(y_train, self.model.predict(X_train_scaled))
+        test_conf_matrix = confusion_matrix(y_test, self.model.predict(X_test_scaled))
+        print("Train Confusion Matrix:\n", train_conf_matrix)
+        print("Test Confusion Matrix:\n", test_conf_matrix)
+
     def predict(self, data):
         """
         Make predictions for the input data.
 
         This method takes labeled input data, parses it to extract features, scales the
         features using the StandardScaler object, and then uses the trained MLPClassifier
         model to make predictions. It prints the size and values of the feature matrix
```

### Comparing `breastcancermlpmodel-0.0.30/setup.py` & `breastcancermlpmodel-0.0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='BreastCancerMLPModel',  
-    version='0.0.30',
+    version='0.0.31',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'scikit-learn==1.4.2',
         'numpy==1.25.2'
     ],
     author='Sergio Sánchez Sánchez',
@@ -31,15 +31,15 @@
 """
 BreastCancerMLPModel Setup
 
 This setup script configures the installation of the BreastCancerMLPModel package. BreastCancerMLPModel is a package for breast cancer diagnosis using MLP classifier.
 
 Project Details:
 - Name: BreastCancerMLPModel
-- Version: 0.0.30
+- Version: 0.0.31
 - Author: Sergio Sánchez Sánchez
 - Email: dreamsoftware92@gmail.com
 - Description: A package for breast cancer diagnosis using MLP classifier.
 - Repository: https://github.com/sergio11/breast_cancer_diagnosis_mlp
 
 Development Status: Beta
```

### Comparing `breastcancermlpmodel-0.0.30/tests/test_mlp_model.py` & `breastcancermlpmodel-0.0.31/tests/test_mlp_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from sklearn.datasets import load_breast_cancer
 from sklearn.model_selection import train_test_split
-from mlp_breast_cancer_diagnosis.mlp_model import BreastCancerMLPModel
+from BreastCancerMLPModel.BreastCancerMLPModel import BreastCancerMLPModel
 
 class TestMLPModel(unittest.TestCase):
     def setUp(self):
         self.model = BreastCancerMLPModel()
 
         # Load breast cancer dataset
         breast_cancer = load_breast_cancer()
```

