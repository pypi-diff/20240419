# Comparing `tmp/dataidea-0.2.0.tar.gz` & `tmp/dataidea-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.2.0.tar", max compression
+gzip compressed data, was "dataidea-0.2.1.tar", max compression
```

## Comparing `dataidea-0.2.0.tar` & `dataidea-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       41 2024-04-18 17:10:00.344848 dataidea-0.2.0/README.md
--rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.0/dataidea/datasets/cluster.csv
--rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.0/dataidea/datasets/demo.csv
--rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.0/dataidea/datasets/fpl.csv
--rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.0/dataidea/datasets/homeprices.csv
--rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.0/dataidea/datasets/melbourne.csv
--rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.0/dataidea/datasets/music.csv
--rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.0/dataidea/datasets/salaries.csv
--rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.0/dataidea/datasets/titanic.csv
--rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.0/dataidea/datasets/vgsales.csv
--rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.0/dataidea/datasets/weather.csv
--rw-r--r--   0        0        0      814 2024-04-19 07:19:41.314532 dataidea-0.2.0/dataidea/datasets.py
--rw-r--r--   0        0        0      210 2024-04-19 05:07:03.723401 dataidea-0.2.0/dataidea/feature_selection.py
--rw-r--r--   0        0        0      416 2024-04-19 05:06:32.502225 dataidea-0.2.0/dataidea/models.py
--rw-r--r--   0        0        0      139 2024-04-19 05:06:09.074706 dataidea-0.2.0/dataidea/packages.py
--rw-r--r--   0        0        0      817 2024-04-19 07:09:44.256023 dataidea-0.2.0/dataidea/tabular.py
--rw-r--r--   0        0        0      481 2024-04-19 07:21:25.802194 dataidea-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 dataidea-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-18 17:10:00.344848 dataidea-0.2.1/README.md
+-rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.1/dataidea/datasets/cluster.csv
+-rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.1/dataidea/datasets/demo.csv
+-rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.1/dataidea/datasets/fpl.csv
+-rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.1/dataidea/datasets/homeprices.csv
+-rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.1/dataidea/datasets/melbourne.csv
+-rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.1/dataidea/datasets/music.csv
+-rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.1/dataidea/datasets/salaries.csv
+-rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.1/dataidea/datasets/titanic.csv
+-rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.1/dataidea/datasets/vgsales.csv
+-rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.1/dataidea/datasets/weather.csv
+-rw-r--r--   0        0        0      814 2024-04-19 07:19:41.314532 dataidea-0.2.1/dataidea/datasets.py
+-rw-r--r--   0        0        0      210 2024-04-19 05:07:03.723401 dataidea-0.2.1/dataidea/feature_selection.py
+-rw-r--r--   0        0        0      469 2024-04-19 07:45:59.402478 dataidea-0.2.1/dataidea/models.py
+-rw-r--r--   0        0        0      139 2024-04-19 05:06:09.074706 dataidea-0.2.1/dataidea/packages.py
+-rw-r--r--   0        0        0      888 2024-04-19 07:46:23.127702 dataidea-0.2.1/dataidea/tabular.py
+-rw-r--r--   0        0        0      481 2024-04-19 07:47:33.279311 dataidea-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 dataidea-0.2.1/PKG-INFO
```

### Comparing `dataidea-0.2.0/dataidea/datasets/demo.csv` & `dataidea-0.2.1/dataidea/datasets/demo.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.0/dataidea/datasets/fpl.csv` & `dataidea-0.2.1/dataidea/datasets/fpl.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.0/dataidea/datasets/melbourne.csv` & `dataidea-0.2.1/dataidea/datasets/melbourne.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.0/dataidea/datasets/salaries.csv` & `dataidea-0.2.1/dataidea/datasets/salaries.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.0/dataidea/datasets/titanic.csv` & `dataidea-0.2.1/dataidea/datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.0/dataidea/datasets/vgsales.csv` & `dataidea-0.2.1/dataidea/datasets/vgsales.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.0/dataidea/datasets.py` & `dataidea-0.2.1/dataidea/datasets.py`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.0/dataidea/tabular.py` & `dataidea-0.2.1/dataidea/tabular.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from joblib import load as load_model
 from joblib import dump as save_model
 # feature selection
 from sklearn.feature_selection import SelectKBest
 from sklearn.feature_selection import f_classif
 from sklearn.feature_selection import f_regression
 from sklearn.feature_selection import RFE
+# model selection
+from sklearn.model_selection import train_test_split
 # models
 from sklearn.linear_model import LogisticRegression
 from sklearn.linear_model import LinearRegression
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.ensemble import RandomForestRegressor
```

### Comparing `dataidea-0.2.0/PKG-INFO` & `dataidea-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataidea
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package to ease data analysis for DATAIDEA students
 License: MIT
 Author: jumashafara
 Author-email: jumashafara0@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```
