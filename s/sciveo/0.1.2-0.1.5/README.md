# Comparing `tmp/sciveo-0.1.2.tar.gz` & `tmp/sciveo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.1.2.tar", last modified: Wed Apr 17 13:39:49 2024, max compression
+gzip compressed data, was "sciveo-0.1.5.tar", last modified: Fri Apr 19 06:54:31 2024, max compression
```

## Comparing `sciveo-0.1.2.tar` & `sciveo-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.959001 sciveo-0.1.2/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 13:39:49.958840 sciveo-0.1.2/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6361 2024-04-17 12:58:32.000000 sciveo-0.1.2/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.938600 sciveo-0.1.2/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.2/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.950655 sciveo-0.1.2/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.2/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.2/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.2/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.952108 sciveo-0.1.2/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.2/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.2/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.2/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.2/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.2/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.954186 sciveo-0.1.2/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.2/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.2/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.2/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-17 13:30:32.000000 sciveo-0.1.2/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.2/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.2/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.2/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.955551 sciveo-0.1.2/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.2/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.2/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.2/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.2/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.2/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.957137 sciveo-0.1.2/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.2/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5868 2024-04-17 13:39:18.000000 sciveo-0.1.2/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.2/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.2/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-17 13:39:38.000000 sciveo-0.1.2/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.949715 sciveo-0.1.2/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 13:39:49.000000 sciveo-0.1.2/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-17 13:39:49.000000 sciveo-0.1.2/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-17 13:39:49.000000 sciveo-0.1.2/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-17 13:39:49.000000 sciveo-0.1.2/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-17 13:39:49.000000 sciveo-0.1.2/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-17 13:39:49.959067 sciveo-0.1.2/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.2/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:39:49.958411 sciveo-0.1.2/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.2/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.2/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.2/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.2/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.921843 sciveo-0.1.5/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-19 06:54:31.921660 sciveo-0.1.5/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6601 2024-04-19 06:47:05.000000 sciveo-0.1.5/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.905472 sciveo-0.1.5/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.5/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.913660 sciveo-0.1.5/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.5/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.5/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.5/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.915434 sciveo-0.1.5/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.5/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.5/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.5/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.5/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.5/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.917942 sciveo-0.1.5/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.5/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.5/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.5/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-17 13:30:32.000000 sciveo-0.1.5/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.5/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.5/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.5/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.919532 sciveo-0.1.5/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.5/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.5/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.5/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.5/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.5/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.920574 sciveo-0.1.5/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.5/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5902 2024-04-19 06:53:07.000000 sciveo-0.1.5/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.5/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.5/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-19 06:54:25.000000 sciveo-0.1.5/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.912694 sciveo-0.1.5/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6753 2024-04-19 06:54:31.000000 sciveo-0.1.5/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-19 06:54:31.000000 sciveo-0.1.5/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-19 06:54:31.000000 sciveo-0.1.5/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-19 06:54:31.000000 sciveo-0.1.5/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-19 06:54:31.000000 sciveo-0.1.5/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-19 06:54:31.921899 sciveo-0.1.5/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.5/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-19 06:54:31.921389 sciveo-0.1.5/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.5/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.5/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.5/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.5/test/test_sampling.py
```

### Comparing `sciveo-0.1.2/PKG-INFO` & `sciveo-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: sciveo
-Version: 0.1.2
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

### Comparing `sciveo-0.1.2/README.md` & `sciveo-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: sciveo
+Version: 0.1.5
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

### Comparing `sciveo-0.1.2/sciveo/__init__.py` & `sciveo-0.1.5/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/api/base.py` & `sciveo-0.1.5/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/api/upload.py` & `sciveo-0.1.5/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/configuration.py` & `sciveo-0.1.5/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/model.py` & `sciveo-0.1.5/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/optimizers.py` & `sciveo-0.1.5/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/sampling.py` & `sciveo-0.1.5/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/tools/daemon.py` & `sciveo-0.1.5/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/tools/formating.py` & `sciveo-0.1.5/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/tools/hardware.py` & `sciveo-0.1.5/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/tools/logger.py` & `sciveo-0.1.5/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/tools/synchronized.py` & `sciveo-0.1.5/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/common/tools/timers.py` & `sciveo-0.1.5/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/content/dataset.py` & `sciveo-0.1.5/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/content/experiment.py` & `sciveo-0.1.5/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/content/project.py` & `sciveo-0.1.5/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/content/runner.py` & `sciveo-0.1.5/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/monitoring/monitor.py` & `sciveo-0.1.5/sciveo/monitoring/monitor.py`

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
@@ -34,15 +35,15 @@
     list_uid_calls = [socket.gethostname, psutil.cpu_count, platform.processor]
     for uid_call in list_uid_calls:
       try:
         machine_serial += f"{uid_call()}{s}"
         s = ""
       except Exception:
         pass
-    return machine_serial
+    return re.sub(r'[\s,\.]', '', machine_serial)
 
 
 class BaseMonitor(DaemonBase):
   def __init__(self, period=5):
     super().__init__(period=period)
 
     self.data = HardwareInfo()()
```

### Comparing `sciveo-0.1.2/sciveo/monitoring/network.py` & `sciveo-0.1.5/sciveo/monitoring/network.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo/monitoring/start.py` & `sciveo-0.1.5/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/sciveo.egg-info/PKG-INFO` & `sciveo-0.1.5/sciveo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.2
+Version: 0.1.5
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

### Comparing `sciveo-0.1.2/sciveo.egg-info/SOURCES.txt` & `sciveo-0.1.5/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/setup.py` & `sciveo-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/test/test_configuration.py` & `sciveo-0.1.5/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/test/test_monitoring.py` & `sciveo-0.1.5/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/test/test_runner.py` & `sciveo-0.1.5/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.2/test/test_sampling.py` & `sciveo-0.1.5/test/test_sampling.py`

 * *Files identical despite different names*

