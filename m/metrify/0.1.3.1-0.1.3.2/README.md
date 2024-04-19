# Comparing `tmp/metrify-0.1.3.1.tar.gz` & `tmp/metrify-0.1.3.2.tar.gz`

## Comparing `metrify-0.1.3.1.tar` & `metrify-0.1.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 metrify-0.1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 metrify-0.1.3.1/.ruff.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 metrify-0.1.3.1/requirements.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 metrify-0.1.3.1/metrify/__init__.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 metrify-0.1.3.1/metrify/metrics.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 metrify-0.1.3.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metrify-0.1.3.1/LICENSE
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 metrify-0.1.3.1/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 metrify-0.1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 metrify-0.1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 metrify-0.1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 metrify-0.1.3.2/.ruff.toml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 metrify-0.1.3.2/requirements.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 metrify-0.1.3.2/metrify/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 metrify-0.1.3.2/metrify/metrics.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 metrify-0.1.3.2/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 metrify-0.1.3.2/LICENSE
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 metrify-0.1.3.2/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 metrify-0.1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 metrify-0.1.3.2/PKG-INFO
```

### Comparing `metrify-0.1.3.1/metrify/metrics.py` & `metrify-0.1.3.2/metrify/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,9 +74,13 @@
 
     # Get precisions, recalls and thresholds (shape for each of these (N, ))
     precisions, recalls, thresholds = precision_recall_curve(t, p)
 
     # Compute all the fbeta scores
     fbetas = (1 + beta**2) * (precisions * recalls) / (beta**2 * precisions + recalls)
 
+    # Find the highest beta score and its position *exlcuding nans*
+    max_fbeta = np.nanmax(fbetas)
+    position = np.nanargmax(fbetas)
+
     # Return the best fbeta score and the corresponding threshold
-    return fbetas.max(), thresholds[fbetas.argmax()]
+    return max_fbeta, thresholds[position]
```

### Comparing `metrify-0.1.3.1/.gitignore` & `metrify-0.1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `metrify-0.1.3.1/LICENSE` & `metrify-0.1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metrify-0.1.3.1/README.md` & `metrify-0.1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `metrify-0.1.3.1/pyproject.toml` & `metrify-0.1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metrify"
-version = "0.1.3.1"
+version = "0.1.3.2"
 authors = [
   { name="Giacomo Piccinini", email="giacomo.piccinini@proton.me" },
 ]
 description = "A package for computing informedness, markedness and phi score"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metrify-0.1.3.1/PKG-INFO` & `metrify-0.1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: metrify
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: A package for computing informedness, markedness and phi score
 Project-URL: Homepage, https://github.com/giacomopiccinini/metrify
 Author-email: Giacomo Piccinini <giacomo.piccinini@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

