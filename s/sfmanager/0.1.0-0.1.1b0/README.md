# Comparing `tmp/sfmanager-0.1.0.tar.gz` & `tmp/sfmanager-0.1.1b0.tar.gz`

## Comparing `sfmanager-0.1.0.tar` & `sfmanager-0.1.1b0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sfmanager-0.1.0/sfmanager/__init__.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.0/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.0/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.0/README.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 sfmanager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 sfmanager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/sfmanager/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/pyproject.toml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b0/PKG-INFO
```

### Comparing `sfmanager-0.1.0/sfmanager/app.py` & `sfmanager-0.1.1b0/sfmanager/app.py`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.0/.gitignore` & `sfmanager-0.1.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.0/LICENSE` & `sfmanager-0.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.0/PKG-INFO` & `sfmanager-0.1.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.0
+Version: 0.1.1b0
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/grandescobar/sfmanager
 Project-URL: Issues, https://github.com/grandescobar/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
+Requires-Dist: pillow>=9.0.1
 Description-Content-Type: text/markdown
 
 This library is not that useful. Perhaps someday it will become great.
```

