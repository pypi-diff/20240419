# Comparing `tmp/torchenhanced-0.3.0b1.tar.gz` & `tmp/torchenhanced-0.3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchenhanced-0.3.0b1.tar", last modified: Mon Apr 15 10:03:47 2024, max compression
+gzip compressed data, was "torchenhanced-0.3.0b2.tar", last modified: Fri Apr 19 10:11:42 2024, max compression
```

## Comparing `torchenhanced-0.3.0b1.tar` & `torchenhanced-0.3.0b2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.923660 torchenhanced-0.3.0b1/
--rw-rw-rw-   0        0        0       95 2024-04-11 10:37:32.000000 torchenhanced-0.3.0b1/.gitignore
--rw-rw-rw-   0        0        0     1118 2024-04-15 10:03:47.920653 torchenhanced-0.3.0b1/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-04-11 14:27:41.000000 torchenhanced-0.3.0b1/README.md
--rw-rw-rw-   0        0        0      901 2024-02-28 18:27:27.000000 torchenhanced-0.3.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       66 2024-04-11 10:34:25.000000 torchenhanced-0.3.0b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 10:03:47.923660 torchenhanced-0.3.0b1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.684312 torchenhanced-0.3.0b1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.740381 torchenhanced-0.3.0b1/src/torchenhanced/
--rw-rw-rw-   0        0        0      169 2024-04-11 10:38:23.000000 torchenhanced-0.3.0b1/src/torchenhanced/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.779282 torchenhanced-0.3.0b1/src/torchenhanced/ml/
--rw-rw-rw-   0        0        0        0 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.799285 torchenhanced-0.3.0b1/src/torchenhanced/ml/functional/
--rw-rw-rw-   0        0        0       34 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/functional/__init__.py
--rw-rw-rw-   0        0        0      959 2024-04-11 10:24:19.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/functional/batch_roll.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.821212 torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/
--rw-rw-rw-   0        0        0       39 2024-04-11 10:33:33.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/__init__.py
--rw-rw-rw-   0        0        0     3975 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/cosine_warmup.py
--rw-rw-rw-   0        0        0     2408 2024-04-11 17:04:26.000000 torchenhanced-0.3.0b1/src/torchenhanced/modules.py
--rw-rw-rw-   0        0        0    35707 2024-04-11 17:50:34.000000 torchenhanced-0.3.0b1/src/torchenhanced/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.866825 torchenhanced-0.3.0b1/src/torchenhanced/util/
--rw-rw-rw-   0        0        0      105 2024-04-11 10:40:11.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-06-14 09:27:16.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/color_compression.py
--rw-rw-rw-   0        0        0      723 2024-04-11 10:24:44.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/files.py
--rw-rw-rw-   0        0        0     1335 2023-06-14 09:27:16.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/misc.py
--rw-rw-rw-   0        0        0     8707 2024-04-11 10:35:08.000000 torchenhanced-0.3.0b1/src/torchenhanced/util/visualize.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.919176 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/
--rw-rw-rw-   0        0        0     1118 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-15 10:03:47.000000 torchenhanced-0.3.0b1/src/torchenhanced.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 10:03:47.916571 torchenhanced-0.3.0b1/tests/
--rw-rw-rw-   0        0        0      836 2024-04-11 17:12:42.000000 torchenhanced-0.3.0b1/tests/test_cosine.py
--rw-rw-rw-   0        0        0     4309 2024-04-11 17:32:43.000000 torchenhanced-0.3.0b1/tests/test_custom_dataset.py
--rw-rw-rw-   0        0        0     1855 2024-04-11 16:17:07.000000 torchenhanced-0.3.0b1/tests/test_modules.py
--rw-rw-rw-   0        0        0     7908 2024-04-11 17:43:48.000000 torchenhanced-0.3.0b1/tests/test_trainer.py
--rw-rw-rw-   0        0        0     2270 2024-04-11 16:19:01.000000 torchenhanced-0.3.0b1/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.483072 torchenhanced-0.3.0b2/
+-rw-rw-rw-   0        0        0       95 2024-04-11 10:37:32.000000 torchenhanced-0.3.0b2/.gitignore
+-rw-rw-rw-   0        0        0     1118 2024-04-19 10:11:42.480072 torchenhanced-0.3.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-11 14:27:41.000000 torchenhanced-0.3.0b2/README.md
+-rw-rw-rw-   0        0        0      901 2024-02-28 18:27:27.000000 torchenhanced-0.3.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       66 2024-04-11 10:34:25.000000 torchenhanced-0.3.0b2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:11:42.483072 torchenhanced-0.3.0b2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.372224 torchenhanced-0.3.0b2/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.401961 torchenhanced-0.3.0b2/src/torchenhanced/
+-rw-rw-rw-   0        0        0      169 2024-04-11 10:38:23.000000 torchenhanced-0.3.0b2/src/torchenhanced/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.442797 torchenhanced-0.3.0b2/src/torchenhanced/ml/
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b2/src/torchenhanced/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.445703 torchenhanced-0.3.0b2/src/torchenhanced/ml/functional/
+-rw-rw-rw-   0        0        0       34 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b2/src/torchenhanced/ml/functional/__init__.py
+-rw-rw-rw-   0        0        0      959 2024-04-11 10:24:19.000000 torchenhanced-0.3.0b2/src/torchenhanced/ml/functional/batch_roll.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.450715 torchenhanced-0.3.0b2/src/torchenhanced/ml/optim/
+-rw-rw-rw-   0        0        0       39 2024-04-11 10:33:33.000000 torchenhanced-0.3.0b2/src/torchenhanced/ml/optim/__init__.py
+-rw-rw-rw-   0        0        0     3975 2024-04-11 11:28:49.000000 torchenhanced-0.3.0b2/src/torchenhanced/ml/optim/cosine_warmup.py
+-rw-rw-rw-   0        0        0     2408 2024-04-11 17:04:26.000000 torchenhanced-0.3.0b2/src/torchenhanced/modules.py
+-rw-rw-rw-   0        0        0    35764 2024-04-19 10:10:26.000000 torchenhanced-0.3.0b2/src/torchenhanced/trainer.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.463501 torchenhanced-0.3.0b2/src/torchenhanced/util/
+-rw-rw-rw-   0        0        0      105 2024-04-11 10:40:11.000000 torchenhanced-0.3.0b2/src/torchenhanced/util/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-06-14 09:27:16.000000 torchenhanced-0.3.0b2/src/torchenhanced/util/color_compression.py
+-rw-rw-rw-   0        0        0      723 2024-04-11 10:24:44.000000 torchenhanced-0.3.0b2/src/torchenhanced/util/files.py
+-rw-rw-rw-   0        0        0     1335 2023-06-14 09:27:16.000000 torchenhanced-0.3.0b2/src/torchenhanced/util/misc.py
+-rw-rw-rw-   0        0        0     8707 2024-04-11 10:35:08.000000 torchenhanced-0.3.0b2/src/torchenhanced/util/visualize.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.478071 torchenhanced-0.3.0b2/src/torchenhanced.egg-info/
+-rw-rw-rw-   0        0        0     1118 2024-04-19 10:11:42.000000 torchenhanced-0.3.0b2/src/torchenhanced.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2024-04-19 10:11:42.000000 torchenhanced-0.3.0b2/src/torchenhanced.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:11:42.000000 torchenhanced-0.3.0b2/src/torchenhanced.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-19 10:11:42.000000 torchenhanced-0.3.0b2/src/torchenhanced.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 10:11:42.000000 torchenhanced-0.3.0b2/src/torchenhanced.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 10:11:42.475080 torchenhanced-0.3.0b2/tests/
+-rw-rw-rw-   0        0        0      836 2024-04-11 17:12:42.000000 torchenhanced-0.3.0b2/tests/test_cosine.py
+-rw-rw-rw-   0        0        0     4309 2024-04-11 17:32:43.000000 torchenhanced-0.3.0b2/tests/test_custom_dataset.py
+-rw-rw-rw-   0        0        0     1855 2024-04-11 16:17:07.000000 torchenhanced-0.3.0b2/tests/test_modules.py
+-rw-rw-rw-   0        0        0     7908 2024-04-11 17:43:48.000000 torchenhanced-0.3.0b2/tests/test_trainer.py
+-rw-rw-rw-   0        0        0     2270 2024-04-11 16:19:01.000000 torchenhanced-0.3.0b2/tests/test_util.py
```

### Comparing `torchenhanced-0.3.0b1/PKG-INFO` & `torchenhanced-0.3.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchenhanced
-Version: 0.3.0b1
+Version: 0.3.0b2
 Summary: Wrappers for pytorch stuff I use on the daily
 Author-email: Vassilis Papadopoulos <frotaur@hotmail.co.uk>
 License: MIT License
 Project-URL: Homepage, https://github.com/frotaur/torchenhanced
 Project-URL: Bug Tracker, https://github.com/frotaur/torchenhanced/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchenhanced-0.3.0b1/pyproject.toml` & `torchenhanced-0.3.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/ml/functional/batch_roll.py` & `torchenhanced-0.3.0b2/src/torchenhanced/ml/functional/batch_roll.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/ml/optim/cosine_warmup.py` & `torchenhanced-0.3.0b2/src/torchenhanced/ml/optim/cosine_warmup.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/modules.py` & `torchenhanced-0.3.0b2/src/torchenhanced/modules.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/trainer.py` & `torchenhanced-0.3.0b2/src/torchenhanced/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -608,17 +608,17 @@
 
         self.step_log = step_log
         self.step_loss=[]
         self.epoch_loss = None
 
         steps_completed = False
         if(pickup):
-            self.stepnum = self.batches
+            self.stepnum = self.steps_done # Pick up where we left off
         else:
-            self.stepnum = 0 #Current instance stepnumber, used for when to log and stop training.
+            self.stepnum = 0 # Stepnum used for logging, and when to stop. This means, we train for a further 'steps' steps.
 
         while not steps_completed:
             iter_on=enumerate(train_loader)
 
             if(resume_batches):
                 resume_batches=False # Only resume for the first epoch, not if we reach and and restart.
                 tofastforward = (self.batches)%self.totbatch
```

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/util/color_compression.py` & `torchenhanced-0.3.0b2/src/torchenhanced/util/color_compression.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/util/files.py` & `torchenhanced-0.3.0b2/src/torchenhanced/util/files.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/util/misc.py` & `torchenhanced-0.3.0b2/src/torchenhanced/util/misc.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced/util/visualize.py` & `torchenhanced-0.3.0b2/src/torchenhanced/util/visualize.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced.egg-info/PKG-INFO` & `torchenhanced-0.3.0b2/src/torchenhanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchenhanced
-Version: 0.3.0b1
+Version: 0.3.0b2
 Summary: Wrappers for pytorch stuff I use on the daily
 Author-email: Vassilis Papadopoulos <frotaur@hotmail.co.uk>
 License: MIT License
 Project-URL: Homepage, https://github.com/frotaur/torchenhanced
 Project-URL: Bug Tracker, https://github.com/frotaur/torchenhanced/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchenhanced-0.3.0b1/src/torchenhanced.egg-info/SOURCES.txt` & `torchenhanced-0.3.0b2/src/torchenhanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/tests/test_cosine.py` & `torchenhanced-0.3.0b2/tests/test_cosine.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/tests/test_custom_dataset.py` & `torchenhanced-0.3.0b2/tests/test_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/tests/test_modules.py` & `torchenhanced-0.3.0b2/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/tests/test_trainer.py` & `torchenhanced-0.3.0b2/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `torchenhanced-0.3.0b1/tests/test_util.py` & `torchenhanced-0.3.0b2/tests/test_util.py`

 * *Files identical despite different names*

