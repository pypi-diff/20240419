# Comparing `tmp/culminator-0.6.tar.gz` & `tmp/culminator-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culminator-0.6.tar", last modified: Fri Apr 19 01:05:54 2024, max compression
+gzip compressed data, was "culminator-0.7.tar", last modified: Fri Apr 19 02:15:20 2024, max compression
```

## Comparing `culminator-0.6.tar` & `culminator-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 01:05:54.490851 culminator-0.6/
--rw-rw-rw-   0        0        0     3015 2024-04-19 01:05:54.489852 culminator-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2870 2024-04-18 08:42:42.000000 culminator-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 01:05:54.480728 culminator-0.6/culminator/
--rw-rw-rw-   0        0        0      107 2024-04-19 01:01:07.000000 culminator-0.6/culminator/__init__.py
--rw-rw-rw-   0        0        0     4241 2024-04-18 07:59:37.000000 culminator-0.6/culminator/classification.py
--rw-rw-rw-   0        0        0     4743 2024-04-18 07:59:43.000000 culminator-0.6/culminator/clustering.py
--rw-rw-rw-   0        0        0     7456 2024-04-18 07:18:31.000000 culminator-0.6/culminator/regression.py
-drwxrwxrwx   0        0        0        0 2024-04-19 01:05:54.487804 culminator-0.6/culminator.egg-info/
--rw-rw-rw-   0        0        0     3015 2024-04-19 01:05:54.000000 culminator-0.6/culminator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-19 01:05:54.000000 culminator-0.6/culminator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 01:05:54.000000 culminator-0.6/culminator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-19 01:05:54.000000 culminator-0.6/culminator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 01:05:54.000000 culminator-0.6/culminator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 01:05:54.491855 culminator-0.6/setup.cfg
--rw-rw-rw-   0        0        0      352 2024-04-19 01:05:51.000000 culminator-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 02:15:20.744329 culminator-0.7/
+-rw-rw-rw-   0        0        0     3015 2024-04-19 02:15:20.742331 culminator-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2024-04-18 08:42:42.000000 culminator-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 02:15:20.734330 culminator-0.7/culminator/
+-rw-rw-rw-   0        0        0      107 2024-04-19 01:01:07.000000 culminator-0.7/culminator/__init__.py
+-rw-rw-rw-   0        0        0     4371 2024-04-19 02:10:59.000000 culminator-0.7/culminator/classification.py
+-rw-rw-rw-   0        0        0     4837 2024-04-19 02:12:55.000000 culminator-0.7/culminator/clustering.py
+-rw-rw-rw-   0        0        0     7578 2024-04-19 02:13:49.000000 culminator-0.7/culminator/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-19 02:15:20.741332 culminator-0.7/culminator.egg-info/
+-rw-rw-rw-   0        0        0     3015 2024-04-19 02:15:20.000000 culminator-0.7/culminator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-19 02:15:20.000000 culminator-0.7/culminator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 02:15:20.000000 culminator-0.7/culminator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 02:15:20.000000 culminator-0.7/culminator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 02:15:20.000000 culminator-0.7/culminator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 02:15:20.744329 culminator-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      352 2024-04-19 02:14:04.000000 culminator-0.7/setup.py
```

### Comparing `culminator-0.6/PKG-INFO` & `culminator-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: culminator
-Version: 0.6
+Version: 0.7
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 # Culminator
 Culminator is a Python package designed to facilitate regression, classification, and clustering. It provides functionalities for data loading, preprocessing,  training, and predicting. This README file serves as a guide to understand and utilize the package effectively.
```

### Comparing `culminator-0.6/README.md` & `culminator-0.7/README.md`

 * *Files identical despite different names*

### Comparing `culminator-0.6/culminator/classification.py` & `culminator-0.7/culminator/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,21 @@
             drop_columns = [data.columns.get_loc(column) for column in drop_columns]
     except:
         pass
     drop_columns.append(y_column)
     X = data.drop(data.columns[drop_columns], axis=1)
 
     if for_predictions:
-        input_df = pd.DataFrame(prediction_input, columns=X.columns).apply(pd.to_numeric, errors='ignore')
+        input_df = pd.DataFrame(prediction_input, columns=X.columns)
+        for col in input_df.columns:
+            try:
+                input_df[col] = input_df[col].astype(int)
+            except:
+                pass
+        
         X = pd.concat([input_df, X], axis=0)
                 
         string_columns = X.select_dtypes(include=['object']).columns
         X = pd.get_dummies(X, columns=string_columns, dtype=int)
         X = X.values
 
         altered_input = X[:len(prediction_input)]
```

### Comparing `culminator-0.6/culminator/clustering.py` & `culminator-0.7/culminator/clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,23 +19,29 @@
     if drop_columns != None:
         if isinstance(drop_columns[0], str):
             X = data.drop(drop_columns, axis=1)
         else:
             X = data.drop(data.columns[drop_columns], axis=1)
 
     if for_predictions:
-            input_df = pd.DataFrame(prediction_input, columns=X.columns).apply(pd.to_numeric, errors='ignore')
-            X = pd.concat([input_df, X], axis=0)
+        input_df = pd.DataFrame(prediction_input, columns=X.columns)
+        for col in input_df.columns:
+            try:
+                input_df[col] = input_df[col].astype(int)
+            except:
+                pass
+
+        X = pd.concat([input_df, X], axis=0)
                     
-            string_columns = X.select_dtypes(include=['object']).columns
-            X = pd.get_dummies(X, columns=string_columns, dtype=int)
-            X = X.values
+        string_columns = X.select_dtypes(include=['object']).columns
+        X = pd.get_dummies(X, columns=string_columns, dtype=int)
+        X = X.values
 
-            altered_input = X[:len(prediction_input)]
-            return altered_input
+        altered_input = X[:len(prediction_input)]
+        return altered_input
 
     string_columns = X.select_dtypes(include=['object']).columns
     X = pd.get_dummies(X, columns=string_columns, dtype=int)
     X[X == True] = 1
     X[X == False] = 0
     
     X = X.values
```

### Comparing `culminator-0.6/culminator/regression.py` & `culminator-0.7/culminator/regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,21 @@
             drop_columns = [data.columns.get_loc(column) for column in drop_columns]
     except:
         pass
     drop_columns.append(y_column)
     X = data.drop(data.columns[drop_columns], axis=1)
 
     if for_predictions:
-        input_df = pd.DataFrame(prediction_input, columns=X.columns).apply(pd.to_numeric, errors='ignore')
+        input_df = pd.DataFrame(prediction_input, columns=X.columns)
+        for col in input_df.columns:
+            try:
+                input_df[col] = input_df[col].astype(int)
+            except:
+                pass
+
         X = pd.concat([input_df, X], axis=0)
                 
         string_columns = X.select_dtypes(include=['object']).columns
         X = pd.get_dummies(X, columns=string_columns, dtype=int)
         X = X.values
 
         altered_input = X[:len(prediction_input)]
```

### Comparing `culminator-0.6/culminator.egg-info/PKG-INFO` & `culminator-0.7/culminator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: culminator
-Version: 0.6
+Version: 0.7
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 
 # Culminator
 Culminator is a Python package designed to facilitate regression, classification, and clustering. It provides functionalities for data loading, preprocessing,  training, and predicting. This README file serves as a guide to understand and utilize the package effectively.
```

