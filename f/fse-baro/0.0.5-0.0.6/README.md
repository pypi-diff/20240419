# Comparing `tmp/fse_baro-0.0.5.tar.gz` & `tmp/fse_baro-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fse_baro-0.0.5.tar", last modified: Tue Apr 16 17:49:19 2024, max compression
+gzip compressed data, was "fse_baro-0.0.6.tar", last modified: Fri Apr 19 07:47:39 2024, max compression
```

## Comparing `fse_baro-0.0.5.tar` & `fse_baro-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:19.179517 fse_baro-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:19.171517 fse_baro-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:19.175517 fse_baro-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-16 17:49:14.000000 fse_baro-0.0.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 17:49:14.000000 fse_baro-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-16 17:49:14.000000 fse_baro-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-16 17:49:14.000000 fse_baro-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-16 17:49:19.175517 fse_baro-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-16 17:49:14.000000 fse_baro-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:19.175517 fse_baro-0.0.5/baro/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 17:49:14.000000 fse_baro-0.0.5/baro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 17:49:14.000000 fse_baro-0.0.5/baro/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-16 17:49:14.000000 fse_baro-0.0.5/baro/root_cause_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:19.175517 fse_baro-0.0.5/fse_baro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-16 17:49:19.000000 fse_baro-0.0.5/fse_baro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-16 17:49:19.000000 fse_baro-0.0.5/fse_baro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:49:19.000000 fse_baro-0.0.5/fse_baro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 17:49:19.000000 fse_baro-0.0.5/fse_baro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 17:49:19.000000 fse_baro-0.0.5/fse_baro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-16 17:49:14.000000 fse_baro-0.0.5/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-16 17:49:14.000000 fse_baro-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:49:19.179517 fse_baro-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:49:19.175517 fse_baro-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-16 17:49:14.000000 fse_baro-0.0.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.970316 fse_baro-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.970316 fse_baro-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-19 07:47:34.000000 fse_baro-0.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-19 07:47:34.000000 fse_baro-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-19 07:47:34.000000 fse_baro-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-19 07:47:34.000000 fse_baro-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-19 07:47:39.974316 fse_baro-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 07:47:34.000000 fse_baro-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/baro/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/_bocpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/root_cause_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-19 07:47:34.000000 fse_baro-0.0.6/baro/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/fse_baro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 07:47:39.000000 fse_baro-0.0.6/fse_baro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-19 07:47:34.000000 fse_baro-0.0.6/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-19 07:47:34.000000 fse_baro-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:47:39.974316 fse_baro-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:47:39.974316 fse_baro-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-19 07:47:34.000000 fse_baro-0.0.6/tests/test.py
```

### Comparing `fse_baro-0.0.5/.github/workflows/python-package.yml` & `fse_baro-0.0.6/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `fse_baro-0.0.5/.github/workflows/python-publish.yml` & `fse_baro-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.5/.gitignore` & `fse_baro-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.5/LICENSE` & `fse_baro-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.5/baro/root_cause_analysis.py` & `fse_baro-0.0.6/baro/root_cause_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,11 @@
 import pandas as pd
 from sklearn.preprocessing import RobustScaler, StandardScaler
 
-
-def drop_constant(df: pd.DataFrame):
-    return df.loc[:, (df != df.iloc[0]).any()]
-
-
-def drop_near_constant(df: pd.DataFrame, threshold: float = 0.1):
-    return df.loc[:, (df != df.iloc[0]).mean() > threshold]
-
-
-def drop_time(df: pd.DataFrame):
-    if "time" in df:
-        df = df.drop(columns=["time"])
-    if "Time" in df:
-        df = df.drop(columns=["Time"])
-    if "timestamp" in df:
-        df = df.drop(columns=["timestamp"])
-    return df
+from .utility import drop_time, drop_constant, drop_near_constant
 
 
 def select_useful_cols(data):
     selected_cols = []
     for c in data.columns:
         # keep time
         if "time" in c:
```

### Comparing `fse_baro-0.0.5/main.py` & `fse_baro-0.0.6/main.py`

 * *Files identical despite different names*

### Comparing `fse_baro-0.0.5/pyproject.toml` & `fse_baro-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 authors = [{name = "Luan Pham", email = "phamquiluan@gmail.com"}]
 license = {file = "LICENSE"}
 dependencies = [
     "numpy",
     "pandas",
     "scikit-learn",
     "pytest",
+    "tqdm",
+    "requests",
+    "matplotlib",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
```

