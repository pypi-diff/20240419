# Comparing `tmp/virgo_modules-0.0.79.tar.gz` & `tmp/virgo_modules-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.79.tar", last modified: Tue Apr 16 08:24:07 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.80.tar", last modified: Fri Apr 19 12:32:00 2024, max compression
```

## Comparing `virgo_modules-0.0.79.tar` & `virgo_modules-0.0.80.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.740811 virgo_modules-0.0.79/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.79/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-16 08:24:07.737817 virgo_modules-0.0.79/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.79/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 08:24:07.741813 virgo_modules-0.0.79/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-16 08:11:25.000000 virgo_modules-0.0.79/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.546290 virgo_modules-0.0.79/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.604067 virgo_modules-0.0.79/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.728811 virgo_modules-0.0.79/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    69517 2024-04-16 08:22:56.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.644800 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:00.184300 virgo_modules-0.0.80/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.80/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-04-19 12:32:00.178296 virgo_modules-0.0.80/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.80/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 12:32:00.185692 virgo_modules-0.0.80/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-19 12:31:49.000000 virgo_modules-0.0.80/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:00.015908 virgo_modules-0.0.80/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:00.067565 virgo_modules-0.0.80/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.80/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:00.168665 virgo_modules-0.0.80/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.80/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.80/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.80/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.80/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    71586 2024-04-19 12:31:32.000000 virgo_modules-0.0.80/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.80/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:32:00.135807 virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-04-19 12:31:59.000000 virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-19 12:31:59.000000 virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 12:31:59.000000 virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-19 12:31:59.000000 virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 12:31:59.000000 virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.79/LICENSE` & `virgo_modules-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.79/PKG-INFO` & `virgo_modules-0.0.80/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.79
+Version: 0.0.80
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.79/setup.py` & `virgo_modules-0.0.80/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.79",
+    version="0.0.80",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.79/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.80/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.79/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.80/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.79/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.80/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.79/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.80/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,68 @@
     df['low_signas'] = df[low_columns].sum(axis=1)
     
     top_up = list(df.sort_values('up_signas', ascending = False).index)[:top]
     top_low = list(df.sort_values('low_signas', ascending = False).index)[:top]
     
     return top_up, top_low
 
+def ranking_first(data, weighted_features, top = 5, window = 5):
+    '''
+    Create a ranking of assets given current signals and weighted average importance
+
+            Parameters:
+                    data (pd.Dataframe): base data
+                    weighted_features (dict): configuration dictionary
+                    top (int): top n to get result
+                    window (int): number of days to assess
+
+            Returns:
+                    top_up (list): top roof signal asset
+                    top_low (list): top botton signal asset
+    '''
+    features = weighted_features.keys()
+    up_columns = ['signal_up_' + x for x in features]
+    low_columns = ['signal_low_' + x for x in features]
+
+    def compute_score(df,col,window):
+        score = 0
+        for i in range(window):
+            row = df.iloc[i]
+            if (row[col] == 1) and (i == 0):
+                score += 1000
+            elif (row[col] == 1) and (i == 1):
+                score -= 200
+            elif (row[col] == 1) and (i >= 2):
+                score -= 50
+        return score
+    
+    ticket_list= list(data.Ticket.unique())
+    result = dict()
+    for ticket in ticket_list:
+        result[ticket] = dict()
+        df = data[data.Ticket == ticket].sort_values('Date').iloc[-window:]
+        
+        for col in low_columns:
+            df = df.sort_values('Date', ascending = False)
+            score = compute_score(df,col,window)
+            result[ticket][col] = score
+        for col in up_columns:
+            score = 0
+            df = df.sort_values('Date', ascending = False)
+            score = compute_score(df,col,window)
+            result[ticket][col] = score
+            
+    df = pd.DataFrame(result).T
+    df['up_signas'] = df[up_columns].sum(axis=1)
+    df['low_signas'] = df[low_columns].sum(axis=1)
+    
+    top_up = list(df.sort_values('up_signas', ascending = False).index)[:top]
+    top_low = list(df.sort_values('low_signas', ascending = False).index)[:top]
+    return top_up, top_low, df
+
 def produce_dashboard(data, columns , ticket_list, show_plot = True, nrows = 150,save_name = False, save_path = False, save_aws = False, aws_credential = False):
     '''
     produce dashboard using signals and list of assets
 
             Parameters:
                     data (pd.Dataframe): base data
                     columns (list): list of features or signals
```

### Comparing `virgo_modules-0.0.79/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.80/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.79
+Version: 0.0.80
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.80/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

