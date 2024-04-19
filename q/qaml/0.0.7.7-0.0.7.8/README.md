# Comparing `tmp/qaml-0.0.7.7.tar.gz` & `tmp/qaml-0.0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaml-0.0.7.7.tar", last modified: Thu Apr 18 20:03:09 2024, max compression
+gzip compressed data, was "qaml-0.0.7.8.tar", last modified: Thu Apr 18 20:16:20 2024, max compression
```

## Comparing `qaml-0.0.7.7.tar` & `qaml-0.0.7.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:03:09.340035 qaml-0.0.7.7/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.7/LICENSE
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:03:09.339895 qaml-0.0.7.7/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.7/README.md
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-18 20:02:31.000000 qaml-0.0.7.7/pyproject.toml
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:03:09.339026 qaml-0.0.7.7/qaml/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.7/qaml/__init__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.7.7/qaml/__main__.py
--rw-r--r--   0 miguelsalinas   (501) staff       (20)    13174 2024-04-18 19:52:37.000000 qaml-0.0.7.7/qaml/client.py
-drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:03:09.339724 qaml-0.0.7.7/qaml.egg-info/
--rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/PKG-INFO
--rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/SOURCES.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/dependency_links.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/entry_points.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/requires.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-18 20:03:09.000000 qaml-0.0.7.7/qaml.egg-info/top_level.txt
--rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-18 20:03:09.340064 qaml-0.0.7.7/setup.cfg
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:16:20.430022 qaml-0.0.7.8/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1065 2024-04-01 03:44:48.000000 qaml-0.0.7.8/LICENSE
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:16:20.429882 qaml-0.0.7.8/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1016 2024-04-11 17:16:45.000000 qaml-0.0.7.8/README.md
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      735 2024-04-18 20:16:16.000000 qaml-0.0.7.8/pyproject.toml
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:16:20.428993 qaml-0.0.7.8/qaml/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       27 2024-03-26 01:02:51.000000 qaml-0.0.7.8/qaml/__init__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      948 2024-04-18 00:07:26.000000 qaml-0.0.7.8/qaml/__main__.py
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)    13192 2024-04-18 20:15:06.000000 qaml-0.0.7.8/qaml/client.py
+drwxr-xr-x   0 miguelsalinas   (501) staff       (20)        0 2024-04-18 20:16:20.429705 qaml-0.0.7.8/qaml.egg-info/
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)     1563 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/PKG-INFO
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)      251 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        1 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       44 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/entry_points.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       56 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/requires.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)        5 2024-04-18 20:16:20.000000 qaml-0.0.7.8/qaml.egg-info/top_level.txt
+-rw-r--r--   0 miguelsalinas   (501) staff       (20)       38 2024-04-18 20:16:20.430053 qaml-0.0.7.8/setup.cfg
```

### Comparing `qaml-0.0.7.7/LICENSE` & `qaml-0.0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.7/PKG-INFO` & `qaml-0.0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.7
+Version: 0.0.7.8
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `qaml-0.0.7.7/README.md` & `qaml-0.0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.7/pyproject.toml` & `qaml-0.0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qaml"
-version = "0.0.7.7"
+version = "0.0.7.8"
 authors = [
     {name = "Miguel Salinas", email = "miguel@camelqa.com"},
 ]
 description = "Control your devices with natural language"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qaml-0.0.7.7/qaml/__main__.py` & `qaml-0.0.7.8/qaml/__main__.py`

 * *Files identical despite different names*

### Comparing `qaml-0.0.7.7/qaml/client.py` & `qaml-0.0.7.8/qaml/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,22 +116,22 @@
 class AndroidClient(BaseClient):
     def __init__(self, api_key, driver=None):
         super().__init__(api_key)
         self.platform = "Android"
         if driver:
             self.driver = driver
         else:
-            for _ in range(3):
+            max_retry = 3
+            for i in range(max_retry):
                 try:
                     self.setup_driver()
                     break
-                except:
-                    pass
-            else:
-                raise Exception("Failed to setup the driver.")
+                except Exception as e:
+                    if i == max_retry - 1:
+                        raise e
         self.screen_size = self.driver.get_window_size()
 
     def setup_driver(self):
         caps = {'deviceName': 'Android Device', 'automationName': 'UiAutomator2', 'autoGrantPermissions': True,
                 'newCommandTimeout': 600, 'mjpegScreenshotUrl': "http://localhost:4723/stream.mjpeg"}
         options = UiAutomator2Options().load_capabilities(caps)
```

### Comparing `qaml-0.0.7.7/qaml.egg-info/PKG-INFO` & `qaml-0.0.7.8/qaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qaml
-Version: 0.0.7.7
+Version: 0.0.7.8
 Summary: Control your devices with natural language
 Author-email: Miguel Salinas <miguel@camelqa.com>
 Project-URL: Homepage, https://github.com/qaml-ai/qaml-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

