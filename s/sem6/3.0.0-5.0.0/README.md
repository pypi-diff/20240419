# Comparing `tmp/sem6-3.0.0.tar.gz` & `tmp/sem6-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sem6-3.0.0.tar", last modified: Thu Apr 18 17:58:05 2024, max compression
+gzip compressed data, was "sem6-5.0.0.tar", last modified: Thu Apr 18 18:09:02 2024, max compression
```

## Comparing `sem6-3.0.0.tar` & `sem6-5.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 17:58:05.621381 sem6-3.0.0/
--rw-rw-rw-   0        0        0       51 2024-04-18 17:58:05.620382 sem6-3.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 17:58:05.591281 sem6-3.0.0/sem6/
--rw-rw-rw-   0        0        0        0 2024-04-13 12:06:54.000000 sem6-3.0.0/sem6/__init__.py
--rw-rw-rw-   0        0        0     1494 2024-04-18 17:11:23.000000 sem6-3.0.0/sem6/adaboost.py
--rw-rw-rw-   0        0        0     2934 2024-04-18 16:25:34.000000 sem6-3.0.0/sem6/clustering.py
--rw-rw-rw-   0        0        0     4128 2024-04-18 12:55:58.000000 sem6-3.0.0/sem6/decisiontree.py
--rw-rw-rw-   0        0        0     2666 2024-04-18 15:51:46.000000 sem6-3.0.0/sem6/ensemble_classification.py
--rw-rw-rw-   0        0        0     1855 2024-04-18 15:53:22.000000 sem6-3.0.0/sem6/ensemble_regression.py
--rw-rw-rw-   0        0        0     3651 2024-04-18 17:55:45.000000 sem6-3.0.0/sem6/gradientboosting.py
--rw-rw-rw-   0        0        0     3418 2024-04-14 14:55:07.000000 sem6-3.0.0/sem6/lightgbm.py
--rw-rw-rw-   0        0        0     3314 2024-04-14 14:55:09.000000 sem6-3.0.0/sem6/linearreg.py
--rw-rw-rw-   0        0        0     3315 2024-04-14 14:55:10.000000 sem6-3.0.0/sem6/logisticreg.py
--rw-rw-rw-   0        0        0     3666 2024-04-14 14:55:12.000000 sem6-3.0.0/sem6/randomforest.py
--rw-rw-rw-   0        0        0     4379 2024-04-18 16:32:26.000000 sem6-3.0.0/sem6/svm.py
--rw-rw-rw-   0        0        0    38016 2024-04-18 17:55:01.000000 sem6-3.0.0/sem6/theory.py
--rw-rw-rw-   0        0        0     3441 2024-04-18 16:33:42.000000 sem6-3.0.0/sem6/xgb.py
-drwxrwxrwx   0        0        0        0 2024-04-18 17:58:05.618379 sem6-3.0.0/sem6.egg-info/
--rw-rw-rw-   0        0        0       51 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-18 17:58:05.000000 sem6-3.0.0/sem6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 17:58:05.621381 sem6-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-18 17:56:54.000000 sem6-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:09:02.495756 sem6-5.0.0/
+-rw-rw-rw-   0        0        0       51 2024-04-18 18:09:02.495756 sem6-5.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 18:09:02.475024 sem6-5.0.0/sem6/
+-rw-rw-rw-   0        0        0        0 2024-04-13 12:06:54.000000 sem6-5.0.0/sem6/__init__.py
+-rw-rw-rw-   0        0        0     1494 2024-04-18 17:11:23.000000 sem6-5.0.0/sem6/adaboost.py
+-rw-rw-rw-   0        0        0     2934 2024-04-18 16:25:34.000000 sem6-5.0.0/sem6/clustering.py
+-rw-rw-rw-   0        0        0     4128 2024-04-18 18:04:08.000000 sem6-5.0.0/sem6/decisiontree.py
+-rw-rw-rw-   0        0        0     2666 2024-04-18 15:51:46.000000 sem6-5.0.0/sem6/ensemble_classification.py
+-rw-rw-rw-   0        0        0     1855 2024-04-18 15:53:22.000000 sem6-5.0.0/sem6/ensemble_regression.py
+-rw-rw-rw-   0        0        0     3651 2024-04-18 17:55:45.000000 sem6-5.0.0/sem6/gradientboosting.py
+-rw-rw-rw-   0        0        0     3418 2024-04-14 14:55:07.000000 sem6-5.0.0/sem6/lightgbm.py
+-rw-rw-rw-   0        0        0     3314 2024-04-14 14:55:09.000000 sem6-5.0.0/sem6/linearreg.py
+-rw-rw-rw-   0        0        0     3315 2024-04-14 14:55:10.000000 sem6-5.0.0/sem6/logisticreg.py
+-rw-rw-rw-   0        0        0     3666 2024-04-14 14:55:12.000000 sem6-5.0.0/sem6/randomforest.py
+-rw-rw-rw-   0        0        0     4379 2024-04-18 16:32:26.000000 sem6-5.0.0/sem6/svm.py
+-rw-rw-rw-   0        0        0    38016 2024-04-18 18:04:05.000000 sem6-5.0.0/sem6/theory.py
+-rw-rw-rw-   0        0        0     3441 2024-04-18 16:33:42.000000 sem6-5.0.0/sem6/xgb.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:09:02.493874 sem6-5.0.0/sem6.egg-info/
+-rw-rw-rw-   0        0        0       51 2024-04-18 18:09:02.000000 sem6-5.0.0/sem6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2024-04-18 18:09:02.000000 sem6-5.0.0/sem6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:09:02.000000 sem6-5.0.0/sem6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 18:09:02.000000 sem6-5.0.0/sem6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-18 18:09:02.000000 sem6-5.0.0/sem6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 18:09:02.495756 sem6-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-18 18:08:36.000000 sem6-5.0.0/setup.py
```

### Comparing `sem6-3.0.0/sem6/adaboost.py` & `sem6-5.0.0/sem6/adaboost.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/clustering.py` & `sem6-5.0.0/sem6/clustering.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/decisiontree.py` & `sem6-5.0.0/sem6/decisiontree.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/ensemble_classification.py` & `sem6-5.0.0/sem6/ensemble_classification.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/ensemble_regression.py` & `sem6-5.0.0/sem6/ensemble_regression.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/gradientboosting.py` & `sem6-5.0.0/sem6/gradientboosting.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/lightgbm.py` & `sem6-5.0.0/sem6/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/linearreg.py` & `sem6-5.0.0/sem6/linearreg.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/logisticreg.py` & `sem6-5.0.0/sem6/logisticreg.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/randomforest.py` & `sem6-5.0.0/sem6/randomforest.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/svm.py` & `sem6-5.0.0/sem6/svm.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/theory.py` & `sem6-5.0.0/sem6/theory.py`

 * *Files identical despite different names*

### Comparing `sem6-3.0.0/sem6/xgb.py` & `sem6-5.0.0/sem6/xgb.py`

 * *Files identical despite different names*

