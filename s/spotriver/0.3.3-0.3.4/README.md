# Comparing `tmp/spotRiver-0.3.3.tar.gz` & `tmp/spotriver-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotRiver-0.3.3.tar", last modified: Fri Mar 29 16:29:04 2024, max compression
+gzip compressed data, was "spotriver-0.3.4.tar", last modified: Fri Apr 19 09:13:34 2024, max compression
```

## Comparing `spotRiver-0.3.3.tar` & `spotriver-0.3.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.875489 spotRiver-0.3.3/
--rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotRiver-0.3.3/LICENSE
--rw-r--r--   0 bartz      (501) staff       (20)      164 2023-03-31 14:59:13.000000 spotRiver-0.3.3/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     3922 2024-03-29 16:29:04.875302 spotRiver-0.3.3/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotRiver-0.3.3/README.md
--rw-r--r--   0 bartz      (501) staff       (20)     1359 2024-03-29 16:28:43.000000 spotRiver-0.3.3/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2024-03-29 16:29:04.875527 spotRiver-0.3.3/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.866282 spotRiver-0.3.3/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.866729 spotRiver-0.3.3/src/spotRiver/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.872437 spotRiver-0.3.3/src/spotRiver/data/
--rw-r--r--   0 bartz      (501) staff       (20)  1993321 2023-07-25 11:59:12.000000 spotRiver-0.3.3/src/spotRiver/data/UnivariateData.csv
--rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotRiver-0.3.3/src/spotRiver/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotRiver-0.3.3/src/spotRiver/data/airline-passengers.csv
--rw-r--r--   0 bartz      (501) staff       (20)     1774 2023-11-07 07:37:14.000000 spotRiver-0.3.3/src/spotRiver/data/airline_passengers.py
--rw-r--r--   0 bartz      (501) staff       (20)    13101 2023-10-25 13:32:20.000000 spotRiver-0.3.3/src/spotRiver/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)     1252 2023-10-25 13:17:56.000000 spotRiver-0.3.3/src/spotRiver/data/bike_sharing.py
--rw-r--r--   0 bartz      (501) staff       (20)     2332 2024-02-15 08:41:57.000000 spotRiver-0.3.3/src/spotRiver/data/csvdataset.py
--rw-r--r--   0 bartz      (501) staff       (20)     2799 2023-10-25 12:50:24.000000 spotRiver-0.3.3/src/spotRiver/data/generic.py
--rw-r--r--   0 bartz      (501) staff       (20)     7759 2023-10-25 13:33:49.000000 spotRiver-0.3.3/src/spotRiver/data/opm.py
--rw-r--r--   0 bartz      (501) staff       (20)    36227 2024-03-18 18:34:20.000000 spotRiver-0.3.3/src/spotRiver/data/river_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      906 2024-03-11 18:16:36.000000 spotRiver-0.3.3/src/spotRiver/data/river_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     4996 2024-03-27 15:19:47.000000 spotRiver-0.3.3/src/spotRiver/data/selector.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.872649 spotRiver-0.3.3/src/spotRiver/data/synth/
--rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotRiver-0.3.3/src/spotRiver/data/synth/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2379 2023-11-07 07:37:14.000000 spotRiver-0.3.3/src/spotRiver/data/synth/sea.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.872764 spotRiver-0.3.3/src/spotRiver/drift/
--rw-r--r--   0 bartz      (501) staff       (20)     1080 2023-07-25 11:59:12.000000 spotRiver-0.3.3/src/spotRiver/drift/drift_generator.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.873111 spotRiver-0.3.3/src/spotRiver/evaluation/
--rw-r--r--   0 bartz      (501) staff       (20)    36257 2024-03-19 23:55:21.000000 spotRiver-0.3.3/src/spotRiver/evaluation/eval_bml.py
--rw-r--r--   0 bartz      (501) staff       (20)     4015 2023-10-25 12:50:38.000000 spotRiver-0.3.3/src/spotRiver/evaluation/eval_nowcast.py
--rw-r--r--   0 bartz      (501) staff       (20)     9236 2023-10-25 12:50:10.000000 spotRiver-0.3.3/src/spotRiver/evaluation/eval_oml.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.873395 spotRiver-0.3.3/src/spotRiver/fun/
--rw-r--r--   0 bartz      (501) staff       (20)    10786 2024-03-19 07:42:09.000000 spotRiver-0.3.3/src/spotRiver/fun/hyperriver.py
--rw-r--r--   0 bartz      (501) staff       (20)    32460 2023-06-18 15:33:18.000000 spotRiver-0.3.3/src/spotRiver/fun/hyperriver_old.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.873556 spotRiver-0.3.3/src/spotRiver/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1521 2023-07-25 11:59:12.000000 spotRiver-0.3.3/src/spotRiver/plot/stats.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.873663 spotRiver-0.3.3/src/spotRiver/preprocess/
--rw-r--r--   0 bartz      (501) staff       (20)     2488 2023-03-07 16:50:39.000000 spotRiver-0.3.3/src/spotRiver/preprocess/impute.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.873876 spotRiver-0.3.3/src/spotRiver/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     6092 2024-03-26 21:22:04.000000 spotRiver-0.3.3/src/spotRiver/utils/data_conversion.py
--rw-r--r--   0 bartz      (501) staff       (20)     6091 2023-07-25 11:59:12.000000 spotRiver-0.3.3/src/spotRiver/utils/features.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.875080 spotRiver-0.3.3/src/spotRiver.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     3922 2024-03-29 16:29:04.000000 spotRiver-0.3.3/src/spotRiver.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     1186 2024-03-29 16:29:04.000000 spotRiver-0.3.3/src/spotRiver.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2024-03-29 16:29:04.000000 spotRiver-0.3.3/src/spotRiver.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)      240 2024-03-29 16:29:04.000000 spotRiver-0.3.3/src/spotRiver.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       10 2024-03-29 16:29:04.000000 spotRiver-0.3.3/src/spotRiver.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-03-29 16:29:04.874861 spotRiver-0.3.3/test/
--rw-r--r--   0 bartz      (501) staff       (20)      509 2024-02-15 15:35:25.000000 spotRiver-0.3.3/test/test_data_selector.py
--rw-r--r--   0 bartz      (501) staff       (20)     4218 2024-03-17 19:50:16.000000 spotRiver-0.3.3/test/test_eval_bml.py
--rw-r--r--   0 bartz      (501) staff       (20)      510 2023-02-25 09:55:05.000000 spotRiver-0.3.3/test/test_features.py
--rw-r--r--   0 bartz      (501) staff       (20)      862 2023-11-07 07:37:14.000000 spotRiver-0.3.3/test/test_hyperriver.py
--rw-r--r--   0 bartz      (501) staff       (20)      510 2024-02-15 15:35:25.000000 spotRiver-0.3.3/test/test_river_data.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.072071 spotriver-0.3.4/
+-rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotriver-0.3.4/LICENSE
+-rw-r--r--   0 bartz      (501) staff       (20)      202 2024-04-19 09:01:28.000000 spotriver-0.3.4/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     3922 2024-04-19 09:13:34.071874 spotriver-0.3.4/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotriver-0.3.4/README.md
+-rw-r--r--   0 bartz      (501) staff       (20)     1359 2024-04-19 09:03:58.000000 spotriver-0.3.4/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2024-04-19 09:13:34.072108 spotriver-0.3.4/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.062308 spotriver-0.3.4/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.062814 spotriver-0.3.4/src/spotRiver/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.066651 spotriver-0.3.4/src/spotRiver/data/
+-rw-r--r--   0 bartz      (501) staff       (20)  1993321 2023-07-25 11:59:12.000000 spotriver-0.3.4/src/spotRiver/data/UnivariateData.csv
+-rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotriver-0.3.4/src/spotRiver/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotriver-0.3.4/src/spotRiver/data/airline-passengers.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     1774 2023-11-07 07:37:14.000000 spotriver-0.3.4/src/spotRiver/data/airline_passengers.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13101 2023-10-25 13:32:20.000000 spotriver-0.3.4/src/spotRiver/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1252 2023-10-25 13:17:56.000000 spotriver-0.3.4/src/spotRiver/data/bike_sharing.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2332 2024-02-15 08:41:57.000000 spotriver-0.3.4/src/spotRiver/data/csvdataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2799 2023-10-25 12:50:24.000000 spotriver-0.3.4/src/spotRiver/data/generic.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7759 2023-10-25 13:33:49.000000 spotriver-0.3.4/src/spotRiver/data/opm.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4996 2024-03-27 15:19:47.000000 spotriver-0.3.4/src/spotRiver/data/selector.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.066863 spotriver-0.3.4/src/spotRiver/data/synth/
+-rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotriver-0.3.4/src/spotRiver/data/synth/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2379 2023-11-07 07:37:14.000000 spotriver-0.3.4/src/spotRiver/data/synth/sea.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.066963 spotriver-0.3.4/src/spotRiver/drift/
+-rw-r--r--   0 bartz      (501) staff       (20)     1080 2023-07-25 11:59:12.000000 spotriver-0.3.4/src/spotRiver/drift/drift_generator.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.067742 spotriver-0.3.4/src/spotRiver/evaluation/
+-rw-r--r--   0 bartz      (501) staff       (20)    36257 2024-03-19 23:55:21.000000 spotriver-0.3.4/src/spotRiver/evaluation/eval_bml.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4015 2023-10-25 12:50:38.000000 spotriver-0.3.4/src/spotRiver/evaluation/eval_nowcast.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9236 2023-10-25 12:50:10.000000 spotriver-0.3.4/src/spotRiver/evaluation/eval_oml.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.068662 spotriver-0.3.4/src/spotRiver/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)    10786 2024-03-19 07:42:09.000000 spotriver-0.3.4/src/spotRiver/fun/hyperriver.py
+-rw-r--r--   0 bartz      (501) staff       (20)    32460 2023-06-18 15:33:18.000000 spotriver-0.3.4/src/spotRiver/fun/hyperriver_old.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.069630 spotriver-0.3.4/src/spotRiver/hyperdict/
+-rw-r--r--   0 bartz      (501) staff       (20)    36227 2024-03-18 18:34:20.000000 spotriver-0.3.4/src/spotRiver/hyperdict/river_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      906 2024-03-11 18:16:36.000000 spotriver-0.3.4/src/spotRiver/hyperdict/river_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.069757 spotriver-0.3.4/src/spotRiver/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1521 2023-07-25 11:59:12.000000 spotriver-0.3.4/src/spotRiver/plot/stats.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.069885 spotriver-0.3.4/src/spotRiver/preprocess/
+-rw-r--r--   0 bartz      (501) staff       (20)     2488 2023-03-07 16:50:39.000000 spotriver-0.3.4/src/spotRiver/preprocess/impute.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.070116 spotriver-0.3.4/src/spotRiver/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     6092 2024-03-26 21:22:04.000000 spotriver-0.3.4/src/spotRiver/utils/data_conversion.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6091 2023-07-25 11:59:12.000000 spotriver-0.3.4/src/spotRiver/utils/features.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.071630 spotriver-0.3.4/src/spotRiver.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     3922 2024-04-19 09:13:34.000000 spotriver-0.3.4/src/spotRiver.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     1380 2024-04-19 09:13:34.000000 spotriver-0.3.4/src/spotRiver.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2024-04-19 09:13:34.000000 spotriver-0.3.4/src/spotRiver.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      240 2024-04-19 09:13:34.000000 spotriver-0.3.4/src/spotRiver.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       10 2024-04-19 09:13:34.000000 spotriver-0.3.4/src/spotRiver.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-19 09:13:34.071474 spotriver-0.3.4/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      509 2024-02-15 15:35:25.000000 spotriver-0.3.4/test/test_data_selector.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4116 2024-04-19 09:08:50.000000 spotriver-0.3.4/test/test_eval_bml.py
+-rw-r--r--   0 bartz      (501) staff       (20)      510 2023-02-25 09:55:05.000000 spotriver-0.3.4/test/test_features.py
+-rw-r--r--   0 bartz      (501) staff       (20)      862 2023-11-07 07:37:14.000000 spotriver-0.3.4/test/test_hyperriver.py
+-rw-r--r--   0 bartz      (501) staff       (20)      510 2024-02-15 15:35:25.000000 spotriver-0.3.4/test/test_river_data.py
```

### Comparing `spotRiver-0.3.3/LICENSE` & `spotriver-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/PKG-INFO` & `spotriver-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: spotRiver
-Version: 0.3.3
-Summary: spotRiver - Sequential Parameter Optimization Interface to River
+Name: spotriver
+Version: 0.3.4
+Summary: spotriver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pytest
 Requires-Dist: pytorch-lightning>=1.4
 Requires-Dist: river>=0.21.0
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Requires-Dist: spotPython>=0.14.4
+Requires-Dist: spotpython>=0.14.4
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: tensorboard
 Requires-Dist: torch
 Requires-Dist: torch-tb-profiler
 Requires-Dist: torchmetrics
 Requires-Dist: torchvision
```

### Comparing `spotRiver-0.3.3/README.md` & `spotriver-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/pyproject.toml` & `spotriver-0.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,20 @@
             "graphviz",
             "numpy",
             "scikit-learn",
             "matplotlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "spotRiver"
-version = "0.3.3"
+name = "spotriver"
+version = "0.3.4"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
-description = "spotRiver - Sequential Parameter Optimization Interface to River"
+description = "spotriver - Sequential Parameter Optimization Interface to River"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
 ]
@@ -32,15 +32,15 @@
   "pandas",
   "plotly",
   "pytest",
   "pytorch-lightning>=1.4",
   "river>=0.21.0",
   "scikit-learn",
   "scipy",
-  "spotPython>=0.14.4",
+  "spotpython>=0.14.4",
   "seaborn",
   "tabulate",
   "tensorboard",
   "torch",
   "torch-tb-profiler",
   "torchmetrics",
   "torchvision"
@@ -55,9 +55,9 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.black]
 line-length = 120
-target-version = ["py310"]
+target-version = ["py311"]
```

### Comparing `spotRiver-0.3.3/src/spotRiver/data/UnivariateData.csv` & `spotriver-0.3.4/src/spotRiver/data/UnivariateData.csv`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/airline-passengers.csv` & `spotriver-0.3.4/src/spotRiver/data/airline-passengers.csv`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/airline_passengers.py` & `spotriver-0.3.4/src/spotRiver/data/airline_passengers.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/base.py` & `spotriver-0.3.4/src/spotRiver/data/base.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/bike_sharing.py` & `spotriver-0.3.4/src/spotRiver/data/bike_sharing.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/csvdataset.py` & `spotriver-0.3.4/src/spotRiver/data/csvdataset.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/generic.py` & `spotriver-0.3.4/src/spotRiver/data/generic.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/opm.py` & `spotriver-0.3.4/src/spotRiver/data/opm.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/river_hyper_dict.json` & `spotriver-0.3.4/src/spotRiver/hyperdict/river_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/river_hyper_dict.py` & `spotriver-0.3.4/src/spotRiver/hyperdict/river_hyper_dict.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/selector.py` & `spotriver-0.3.4/src/spotRiver/data/selector.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/data/synth/sea.py` & `spotriver-0.3.4/src/spotRiver/data/synth/sea.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/drift/drift_generator.py` & `spotriver-0.3.4/src/spotRiver/drift/drift_generator.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/evaluation/eval_bml.py` & `spotriver-0.3.4/src/spotRiver/evaluation/eval_bml.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/evaluation/eval_nowcast.py` & `spotriver-0.3.4/src/spotRiver/evaluation/eval_nowcast.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/evaluation/eval_oml.py` & `spotriver-0.3.4/src/spotRiver/evaluation/eval_oml.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/fun/hyperriver.py` & `spotriver-0.3.4/src/spotRiver/fun/hyperriver.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/fun/hyperriver_old.py` & `spotriver-0.3.4/src/spotRiver/fun/hyperriver_old.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/plot/stats.py` & `spotriver-0.3.4/src/spotRiver/plot/stats.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/preprocess/impute.py` & `spotriver-0.3.4/src/spotRiver/preprocess/impute.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/utils/data_conversion.py` & `spotriver-0.3.4/src/spotRiver/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver/utils/features.py` & `spotriver-0.3.4/src/spotRiver/utils/features.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.3.3/src/spotRiver.egg-info/PKG-INFO` & `spotriver-0.3.4/src/spotRiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: spotRiver
-Version: 0.3.3
-Summary: spotRiver - Sequential Parameter Optimization Interface to River
+Name: spotriver
+Version: 0.3.4
+Summary: spotriver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pytest
 Requires-Dist: pytorch-lightning>=1.4
 Requires-Dist: river>=0.21.0
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Requires-Dist: spotPython>=0.14.4
+Requires-Dist: spotpython>=0.14.4
 Requires-Dist: seaborn
 Requires-Dist: tabulate
 Requires-Dist: tensorboard
 Requires-Dist: torch
 Requires-Dist: torch-tb-profiler
 Requires-Dist: torchmetrics
 Requires-Dist: torchvision
```

### Comparing `spotRiver-0.3.3/src/spotRiver.egg-info/SOURCES.txt` & `spotriver-0.3.4/src/spotRiver.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,27 +12,32 @@
 src/spotRiver/data/airline-passengers.csv
 src/spotRiver/data/airline_passengers.py
 src/spotRiver/data/base.py
 src/spotRiver/data/bike_sharing.py
 src/spotRiver/data/csvdataset.py
 src/spotRiver/data/generic.py
 src/spotRiver/data/opm.py
-src/spotRiver/data/river_hyper_dict.json
-src/spotRiver/data/river_hyper_dict.py
 src/spotRiver/data/selector.py
 src/spotRiver/data/synth/__init__.py
 src/spotRiver/data/synth/sea.py
 src/spotRiver/drift/drift_generator.py
 src/spotRiver/evaluation/eval_bml.py
 src/spotRiver/evaluation/eval_nowcast.py
 src/spotRiver/evaluation/eval_oml.py
 src/spotRiver/fun/hyperriver.py
 src/spotRiver/fun/hyperriver_old.py
+src/spotRiver/hyperdict/river_hyper_dict.json
+src/spotRiver/hyperdict/river_hyper_dict.py
 src/spotRiver/plot/stats.py
 src/spotRiver/preprocess/impute.py
 src/spotRiver/utils/data_conversion.py
 src/spotRiver/utils/features.py
+src/spotriver.egg-info/PKG-INFO
+src/spotriver.egg-info/SOURCES.txt
+src/spotriver.egg-info/dependency_links.txt
+src/spotriver.egg-info/requires.txt
+src/spotriver.egg-info/top_level.txt
 test/test_data_selector.py
 test/test_eval_bml.py
 test/test_features.py
 test/test_hyperriver.py
 test/test_river_data.py
```

### Comparing `spotRiver-0.3.3/test/test_eval_bml.py` & `spotriver-0.3.4/test/test_eval_bml.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import pandas as pd
 import numpy as np
 from river import linear_model
 from river import preprocessing
 from sklearn.metrics import mean_absolute_error
 from spotRiver.evaluation.eval_bml import eval_oml_horizon
 from sklearn.metrics import accuracy_score
-from river import preprocessing
 from river.forest import AMFClassifier
 from river.datasets import Bananas
-from spotRiver.data.river_hyper_dict import RiverHyperDict
+from spotRiver.hyperdict.river_hyper_dict import RiverHyperDict
 from spotRiver.utils.data_conversion import convert_to_df
 from spotPython.hyperparameters.values import add_core_model_to_fun_control
 from spotPython.utils.init import fun_control_init
 from spotPython.hyperparameters.values import modify_hyper_parameter_bounds
 from spotPython.hyperparameters.values import get_one_core_model_from_X
 from spotPython.hyperparameters.values import get_default_hyperparameters_as_array
-from spotRiver.evaluation.eval_bml import eval_oml_horizon
 
 
 def test_eval_oml_horizon():
     # create a sample model
     model = (
         preprocessing.StandardScaler() |
         linear_model.LinearRegression(intercept_lr=.5)
@@ -38,29 +36,30 @@
     horizon = 5
 
     # set the metric
     metric = mean_absolute_error
 
     # evaluate the model
     res, preds = eval_oml_horizon(
-        model = model,
-        train = train,
-        test = test,
-        target_column = target_column,
-        horizon = horizon,
-        include_remainder = True,
-        metric = metric,
-        oml_grace_period = horizon,
+        model=model,
+        train=train,
+        test=test,
+        target_column=target_column,
+        horizon=horizon,
+        include_remainder=True,
+        metric=metric,
+        oml_grace_period=horizon,
     )
 
     # result should have one value for the initial model and one value for each horizon
     assert res.shape[0] == 1 + test.shape[0] // horizon
     # predictions  should be based on the test set only
     assert preds.shape == (test.shape[0], 3)
 
+
 def test_eval_oml_horizon_with_default():
     PREFIX = "0000"
     fun_control = fun_control_init(
         PREFIX=PREFIX,
         TENSORBOARD_CLEAN=True)
     #fun_control
     horizon = 30
@@ -89,15 +88,14 @@
     add_core_model_to_fun_control(core_model=AMFClassifier,
                                 fun_control=fun_control,
                                 hyper_dict=RiverHyperDict,
                                 filename=None)
     modify_hyper_parameter_bounds(fun_control, "n_estimators", bounds=[2,20])
     modify_hyper_parameter_bounds(fun_control, "step", bounds=[0.5,2])
 
-
     X_start = get_default_hyperparameters_as_array(fun_control)
     model_default = get_one_core_model_from_X(X_start, fun_control, default=True)
     df_eval_default, df_true_default = eval_oml_horizon(
                         model=model_default,
                         train=fun_control["train"],
                         test=fun_control["test"],
                         target_column=fun_control["target_column"],
```

### Comparing `spotRiver-0.3.3/test/test_hyperriver.py` & `spotriver-0.3.4/test/test_hyperriver.py`

 * *Files identical despite different names*

