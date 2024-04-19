# Comparing `tmp/sciveo-0.1.3.tar.gz` & `tmp/sciveo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.1.3.tar", last modified: Thu Apr 18 11:59:53 2024, max compression
+gzip compressed data, was "sciveo-0.1.4.tar", last modified: Fri Apr 19 06:48:02 2024, max compression
```

## Comparing `sciveo-0.1.3.tar` & `sciveo-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.738258 sciveo-0.1.3/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-18 11:59:53.737625 sciveo-0.1.3/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6361 2024-04-17 12:58:32.000000 sciveo-0.1.3/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.594442 sciveo-0.1.3/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.3/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.680482 sciveo-0.1.3/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.3/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.3/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.3/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.704501 sciveo-0.1.3/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.3/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.3/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.3/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.3/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.3/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.721040 sciveo-0.1.3/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.3/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.3/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.3/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-17 13:30:32.000000 sciveo-0.1.3/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.3/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.3/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.3/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.727285 sciveo-0.1.3/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.3/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.3/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.3/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.3/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.3/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.731412 sciveo-0.1.3/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.3/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5885 2024-04-18 11:59:12.000000 sciveo-0.1.3/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.3/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.3/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-18 11:59:24.000000 sciveo-0.1.3/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.677942 sciveo-0.1.3/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-18 11:59:53.000000 sciveo-0.1.3/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-18 11:59:53.000000 sciveo-0.1.3/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-18 11:59:53.000000 sciveo-0.1.3/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-18 11:59:53.000000 sciveo-0.1.3/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-18 11:59:53.000000 sciveo-0.1.3/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-18 11:59:53.738351 sciveo-0.1.3/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.3/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-18 11:59:53.737053 sciveo-0.1.3/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.3/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.3/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.3/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.3/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.955971 sciveo-0.1.4/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-19 06:48:02.955800 sciveo-0.1.4/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6601 2024-04-19 06:47:05.000000 sciveo-0.1.4/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.940477 sciveo-0.1.4/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.4/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.947422 sciveo-0.1.4/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.4/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.4/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.4/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.949066 sciveo-0.1.4/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.4/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.4/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.4/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.4/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.4/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.951210 sciveo-0.1.4/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.4/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.4/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.4/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-17 13:30:32.000000 sciveo-0.1.4/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.4/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.4/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.4/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.952830 sciveo-0.1.4/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.4/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.4/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.4/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.4/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.4/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.954096 sciveo-0.1.4/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.4/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5920 2024-04-18 12:04:34.000000 sciveo-0.1.4/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.4/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.4/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-19 06:40:50.000000 sciveo-0.1.4/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.946217 sciveo-0.1.4/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-19 06:48:02.000000 sciveo-0.1.4/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-19 06:48:02.000000 sciveo-0.1.4/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-19 06:48:02.000000 sciveo-0.1.4/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-19 06:48:02.000000 sciveo-0.1.4/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-19 06:48:02.000000 sciveo-0.1.4/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-19 06:48:02.956025 sciveo-0.1.4/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.4/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:48:02.955426 sciveo-0.1.4/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.4/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.4/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.4/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.4/test/test_sampling.py
```

### Comparing `sciveo-0.1.3/PKG-INFO` & `sciveo-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: sciveo
-Version: 0.1.3
-Description-Content-Type: text/markdown
-Provides-Extra: mon
-Provides-Extra: net
-Provides-Extra: all
-
 # SCIVEO - ML/AI and Scientific tools
 
 ## Experiments Management Client
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
@@ -42,20 +34,36 @@
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
+```shell
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
+```
 
-When using sciveo monitoring just run, using suitable python environment
+When using sciveo Monitoring just run, using suitable python environment
+```shell
 python -c "import sciveo; sciveo.monitor(period=120)"
+```
+
+Monitoring started along with other python code.
+```python
+import sciveo
+
+# Non blocking monitoring, so continue the code execution after it.
+sciveo.monitor(period=120, block=False)
+
+#rest of your code here
+
+
+```
 
-When using sciveo experimental projects management
+When using sciveo Experimental projects management
 
 ```python
 
 # These are experiment specific imports for the demo purposes only.
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score, mean_absolute_percentage_error
 from ml.time_series import TimeSeriesTrainer, TimeSeriesPredictor
 
@@ -157,8 +165,8 @@
 
 
 
 
 ### Who do I talk to? ###
 
 * Pavlin Georgiev
-* pavlin@softel.bg
+* pavlin@softel.bg
```

### Comparing `sciveo-0.1.3/README.md` & `sciveo-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: sciveo
+Version: 0.1.4
+Description-Content-Type: text/markdown
+Provides-Extra: mon
+Provides-Extra: net
+Provides-Extra: all
+
 # SCIVEO - ML/AI and Scientific tools
 
 ## Experiments Management Client
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
@@ -34,20 +42,36 @@
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
+```shell
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
+```
 
-When using sciveo monitoring just run, using suitable python environment
+When using sciveo Monitoring just run, using suitable python environment
+```shell
 python -c "import sciveo; sciveo.monitor(period=120)"
+```
+
+Monitoring started along with other python code.
+```python
+import sciveo
+
+# Non blocking monitoring, so continue the code execution after it.
+sciveo.monitor(period=120, block=False)
+
+#rest of your code here
+
+
+```
 
-When using sciveo experimental projects management
+When using sciveo Experimental projects management
 
 ```python
 
 # These are experiment specific imports for the demo purposes only.
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score, mean_absolute_percentage_error
 from ml.time_series import TimeSeriesTrainer, TimeSeriesPredictor
 
@@ -149,8 +173,8 @@
 
 
 
 
 ### Who do I talk to? ###
 
 * Pavlin Georgiev
-* pavlin@softel.bg
+* pavlin@softel.bg
```

### Comparing `sciveo-0.1.3/sciveo/__init__.py` & `sciveo-0.1.4/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/api/base.py` & `sciveo-0.1.4/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/api/upload.py` & `sciveo-0.1.4/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/configuration.py` & `sciveo-0.1.4/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/model.py` & `sciveo-0.1.4/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/optimizers.py` & `sciveo-0.1.4/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/sampling.py` & `sciveo-0.1.4/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/tools/daemon.py` & `sciveo-0.1.4/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/tools/formating.py` & `sciveo-0.1.4/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/tools/hardware.py` & `sciveo-0.1.4/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/tools/logger.py` & `sciveo-0.1.4/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/tools/synchronized.py` & `sciveo-0.1.4/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/common/tools/timers.py` & `sciveo-0.1.4/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/content/dataset.py` & `sciveo-0.1.4/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/content/experiment.py` & `sciveo-0.1.4/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/content/project.py` & `sciveo-0.1.4/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/content/runner.py` & `sciveo-0.1.4/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/monitoring/monitor.py` & `sciveo-0.1.4/sciveo/monitoring/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import os
 import subprocess
 import time
 import datetime
 import socket
 import psutil
 import platform
+import re
 import uuid
 import numpy as np
 
 from sciveo.common.tools.logger import *
 from sciveo.common.tools.daemon import DaemonBase
 from sciveo.common.tools.hardware import *
 from sciveo.common.tools.formating import format_memory_size
@@ -30,15 +31,16 @@
   @staticmethod
   def serial():
     machine_serial = ""
     s = "-"
     list_uid_calls = [socket.gethostname, psutil.cpu_count, platform.processor]
     for uid_call in list_uid_calls:
       try:
-        machine_serial += f"{uid_call().replace(' ', '')}{s}"
+        uid = re.sub(r'[\s,\.]', '', uid_call())
+        machine_serial += f"{uid}{s}"
         s = ""
       except Exception:
         pass
     return machine_serial
 
 
 class BaseMonitor(DaemonBase):
```

### Comparing `sciveo-0.1.3/sciveo/monitoring/network.py` & `sciveo-0.1.4/sciveo/monitoring/network.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo/monitoring/start.py` & `sciveo-0.1.4/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/sciveo.egg-info/PKG-INFO` & `sciveo-0.1.4/sciveo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.3
+Version: 0.1.4
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
 
@@ -42,20 +42,36 @@
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
 
 When have sciveo account:
+```shell
 export SCIVEO_SECRET_ACCESS_KEY='my_sciveo_user_auth_token'
+```
 
-When using sciveo monitoring just run, using suitable python environment
+When using sciveo Monitoring just run, using suitable python environment
+```shell
 python -c "import sciveo; sciveo.monitor(period=120)"
+```
 
-When using sciveo experimental projects management
+Monitoring started along with other python code.
+```python
+import sciveo
+
+# Non blocking monitoring, so continue the code execution after it.
+sciveo.monitor(period=120, block=False)
+
+#rest of your code here
+
+
+```
+
+When using sciveo Experimental projects management
 
 ```python
 
 # These are experiment specific imports for the demo purposes only.
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score, mean_absolute_percentage_error
 from ml.time_series import TimeSeriesTrainer, TimeSeriesPredictor
```

### Comparing `sciveo-0.1.3/sciveo.egg-info/SOURCES.txt` & `sciveo-0.1.4/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/setup.py` & `sciveo-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/test/test_configuration.py` & `sciveo-0.1.4/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/test/test_monitoring.py` & `sciveo-0.1.4/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/test/test_runner.py` & `sciveo-0.1.4/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.3/test/test_sampling.py` & `sciveo-0.1.4/test/test_sampling.py`

 * *Files identical despite different names*

