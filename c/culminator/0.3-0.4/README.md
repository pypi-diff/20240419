# Comparing `tmp/culminator-0.3.tar.gz` & `tmp/culminator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culminator-0.3.tar", last modified: Thu Apr 18 05:16:16 2024, max compression
+gzip compressed data, was "culminator-0.4.tar", last modified: Thu Apr 18 08:45:50 2024, max compression
```

## Comparing `culminator-0.3.tar` & `culminator-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:16:16.941354 culminator-0.3/
--rw-rw-rw-   0        0        0      151 2024-04-18 05:16:16.939350 culminator-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-04-18 05:07:17.000000 culminator-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 05:16:16.929798 culminator-0.3/culminator/
--rw-rw-rw-   0        0        0      197 2024-04-18 04:27:17.000000 culminator-0.3/culminator/__init__.py
--rw-rw-rw-   0        0        0     4196 2024-04-18 04:25:35.000000 culminator-0.3/culminator/classification.py
--rw-rw-rw-   0        0        0     4700 2024-04-18 04:25:45.000000 culminator-0.3/culminator/clustering.py
--rw-rw-rw-   0        0        0     7417 2024-04-18 04:25:57.000000 culminator-0.3/culminator/regression.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:16:16.937351 culminator-0.3/culminator.egg-info/
--rw-rw-rw-   0        0        0      151 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-18 05:16:16.000000 culminator-0.3/culminator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 05:16:16.941354 culminator-0.3/setup.cfg
--rw-rw-rw-   0        0        0      352 2024-04-18 05:07:57.000000 culminator-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:45:50.476888 culminator-0.4/
+-rw-rw-rw-   0        0        0     3015 2024-04-18 08:45:50.475888 culminator-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2870 2024-04-18 08:42:42.000000 culminator-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 08:45:50.463076 culminator-0.4/culminator/
+-rw-rw-rw-   0        0        0      197 2024-04-18 04:27:17.000000 culminator-0.4/culminator/__init__.py
+-rw-rw-rw-   0        0        0     4241 2024-04-18 07:59:37.000000 culminator-0.4/culminator/classification.py
+-rw-rw-rw-   0        0        0     4743 2024-04-18 07:59:43.000000 culminator-0.4/culminator/clustering.py
+-rw-rw-rw-   0        0        0     7456 2024-04-18 07:18:31.000000 culminator-0.4/culminator/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-18 08:45:50.473876 culminator-0.4/culminator.egg-info/
+-rw-rw-rw-   0        0        0     3015 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 08:45:50.000000 culminator-0.4/culminator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 08:45:50.476888 culminator-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      352 2024-04-18 08:45:28.000000 culminator-0.4/setup.py
```

### Comparing `culminator-0.3/culminator/classification.py` & `culminator-0.4/culminator/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         input_df = pd.DataFrame(prediction_input, columns=X.columns).apply(pd.to_numeric, errors='ignore')
         X = pd.concat([input_df, X], axis=0)
                 
         string_columns = X.select_dtypes(include=['object']).columns
         X = pd.get_dummies(X, columns=string_columns, dtype=int)
         X = X.values
 
-        return X[:len(prediction_input)]
+        altered_input = X[:len(prediction_input)]
+        return altered_input
 
     string_columns = X.select_dtypes(include=['object']).columns
     X = pd.get_dummies(X, columns=string_columns, dtype=int)
 
     X = X.values
     y = y.values
 
@@ -82,29 +83,29 @@
         print(f"prediction {i + 1}: {predictions[i]}, target value: {y[i]}")
         if (y[i] != predictions[i]):
             wrong += 1
     print(f"Amount wrong: {wrong}")
     
     return predictions
 
-def classification(filename, y_column=None, drop_columns=None, alpha=0.01, num_iters=100000):
+def classification(filename, y_column=None, drop_columns=None, alpha=0.01, num_attempts=100000):
     X, y = load_data(filename, y_column, drop_columns)
     X, mean, std = scale_features(X)
     m, n = X.shape
 
     unique_classes = np.unique(y)
     num_classes = len(unique_classes)
     
     label_map = {i: species for i, species in enumerate(unique_classes)}
     parameters = np.zeros((n + 1, num_classes))
 
     for i, cls in enumerate(unique_classes):
         binary_y = (y == cls).astype(int)
         X_train = np.hstack((np.ones((m, 1)), X))
-        parameters[:, i] = gradient_descent(X_train, binary_y, parameters[:, i], alpha, num_iters)
+        parameters[:, i] = gradient_descent(X_train, binary_y, parameters[:, i], alpha, num_attempts)
     
     predictions = print_predictions(X_train, y, parameters, label_map)
 
     return X, y, parameters, predictions, label_map, mean, std
 
 def predict_values_classification(input, filename, mean, std, parameters, label_map, y_column=None, drop_columns=None):
     input_scaled = load_data(filename, y_column, drop_columns, True, input)
```

### Comparing `culminator-0.3/culminator/clustering.py` & `culminator-0.4/culminator/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,16 @@
             input_df = pd.DataFrame(prediction_input, columns=X.columns).apply(pd.to_numeric, errors='ignore')
             X = pd.concat([input_df, X], axis=0)
                     
             string_columns = X.select_dtypes(include=['object']).columns
             X = pd.get_dummies(X, columns=string_columns, dtype=int)
             X = X.values
 
-            return X[:len(prediction_input)]
+            altered_input = X[:len(prediction_input)]
+            return altered_input
 
     string_columns = X.select_dtypes(include=['object']).columns
     X = pd.get_dummies(X, columns=string_columns, dtype=int)
     X[X == True] = 1
     X[X == False] = 0
     
     X = X.values
```

### Comparing `culminator-0.3/culminator/regression.py` & `culminator-0.4/culminator/regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         input_df = pd.DataFrame(prediction_input, columns=X.columns).apply(pd.to_numeric, errors='ignore')
         X = pd.concat([input_df, X], axis=0)
                 
         string_columns = X.select_dtypes(include=['object']).columns
         X = pd.get_dummies(X, columns=string_columns, dtype=int)
         X = X.values
 
-        return X[:len(prediction_input)]
+        altered_input = X[:len(prediction_input)]
+        return altered_input
 
     string_columns = X.select_dtypes(include=['object']).columns
     X = pd.get_dummies(X, columns=string_columns, dtype=int)
 
     X = X.values
     y = y.values
```

