# Comparing `tmp/cul-spectrum-1.0.1.tar.gz` & `tmp/cul_spectrum-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cul-spectrum-1.0.1.tar", last modified: Tue Feb 13 22:21:05 2024, max compression
+gzip compressed data, was "cul_spectrum-1.0.2.tar", last modified: Thu Apr 18 22:48:57 2024, max compression
```

## Comparing `cul-spectrum-1.0.1.tar` & `cul_spectrum-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-02-13 22:21:05.512440 cul-spectrum-1.0.1/
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1572 2024-02-01 22:27:14.000000 cul-spectrum-1.0.1/LICENSE
--rw-r--r--   0 djuhasz   (1000) djuhasz   (1000)     3330 2024-02-13 22:21:05.512440 cul-spectrum-1.0.1/PKG-INFO
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     2713 2024-02-13 18:25:04.000000 cul-spectrum-1.0.1/README.md
-drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-02-13 22:21:05.512440 cul-spectrum-1.0.1/cul_spectrum/
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)      152 2024-02-13 22:17:37.000000 cul-spectrum-1.0.1/cul_spectrum/__init__.py
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1926 2024-02-13 17:47:03.000000 cul-spectrum-1.0.1/cul_spectrum/cli.py
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1627 2024-02-13 17:47:39.000000 cul-spectrum-1.0.1/cul_spectrum/client.py
-drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-02-13 22:21:05.512440 cul-spectrum-1.0.1/cul_spectrum.egg-info/
--rw-r--r--   0 djuhasz   (1000) djuhasz   (1000)     3330 2024-02-13 22:21:05.000000 cul-spectrum-1.0.1/cul_spectrum.egg-info/PKG-INFO
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)      367 2024-02-13 22:21:05.000000 cul-spectrum-1.0.1/cul_spectrum.egg-info/SOURCES.txt
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)        1 2024-02-13 22:21:05.000000 cul-spectrum-1.0.1/cul_spectrum.egg-info/dependency_links.txt
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       51 2024-02-13 22:21:05.000000 cul-spectrum-1.0.1/cul_spectrum.egg-info/entry_points.txt
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       13 2024-02-13 22:21:05.000000 cul-spectrum-1.0.1/cul_spectrum.egg-info/requires.txt
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       13 2024-02-13 22:21:05.000000 cul-spectrum-1.0.1/cul_spectrum.egg-info/top_level.txt
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       85 2024-02-01 22:14:53.000000 cul-spectrum-1.0.1/pyproject.toml
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1138 2024-02-13 22:21:05.512440 cul-spectrum-1.0.1/setup.cfg
-drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-02-13 22:21:05.512440 cul-spectrum-1.0.1/tests/
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     2709 2024-02-13 17:48:31.000000 cul-spectrum-1.0.1/tests/test_cli.py
--rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     3266 2024-02-13 17:50:43.000000 cul-spectrum-1.0.1/tests/test_client.py
+drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-04-18 22:48:57.224726 cul_spectrum-1.0.2/
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1572 2024-02-01 22:27:14.000000 cul_spectrum-1.0.2/LICENSE
+-rw-r--r--   0 djuhasz   (1000) djuhasz   (1000)     3330 2024-04-18 22:48:57.224726 cul_spectrum-1.0.2/PKG-INFO
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     2713 2024-02-13 18:25:04.000000 cul_spectrum-1.0.2/README.md
+drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-04-18 22:48:57.220726 cul_spectrum-1.0.2/cul_spectrum/
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)      152 2024-04-18 22:31:09.000000 cul_spectrum-1.0.2/cul_spectrum/__init__.py
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1926 2024-02-13 17:47:03.000000 cul_spectrum-1.0.2/cul_spectrum/cli.py
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1627 2024-04-18 22:29:07.000000 cul_spectrum-1.0.2/cul_spectrum/client.py
+drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-04-18 22:48:57.224726 cul_spectrum-1.0.2/cul_spectrum.egg-info/
+-rw-r--r--   0 djuhasz   (1000) djuhasz   (1000)     3330 2024-04-18 22:48:57.000000 cul_spectrum-1.0.2/cul_spectrum.egg-info/PKG-INFO
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)      367 2024-04-18 22:48:57.000000 cul_spectrum-1.0.2/cul_spectrum.egg-info/SOURCES.txt
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)        1 2024-04-18 22:48:57.000000 cul_spectrum-1.0.2/cul_spectrum.egg-info/dependency_links.txt
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       51 2024-04-18 22:48:57.000000 cul_spectrum-1.0.2/cul_spectrum.egg-info/entry_points.txt
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       13 2024-04-18 22:48:57.000000 cul_spectrum-1.0.2/cul_spectrum.egg-info/requires.txt
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       13 2024-04-18 22:48:57.000000 cul_spectrum-1.0.2/cul_spectrum.egg-info/top_level.txt
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)       85 2024-02-01 22:14:53.000000 cul_spectrum-1.0.2/pyproject.toml
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     1138 2024-04-18 22:48:57.224726 cul_spectrum-1.0.2/setup.cfg
+drwxrwxr-x   0 djuhasz   (1000) djuhasz   (1000)        0 2024-04-18 22:48:57.220726 cul_spectrum-1.0.2/tests/
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     2709 2024-02-13 17:48:31.000000 cul_spectrum-1.0.2/tests/test_cli.py
+-rw-rw-r--   0 djuhasz   (1000) djuhasz   (1000)     3266 2024-02-13 17:50:43.000000 cul_spectrum-1.0.2/tests/test_client.py
```

### Comparing `cul-spectrum-1.0.1/LICENSE` & `cul_spectrum-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cul-spectrum-1.0.1/PKG-INFO` & `cul_spectrum-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cul-spectrum
-Version: 1.0.1
+Version: 1.0.2
 Summary: Concordia University Library Spectrum Client
 Home-page: https://github.com/artefactual-labs/cul-spectrum
 Author: Artefactual Systems, Inc.
 Author-email: info@artefactual.com
 Project-URL: Bug Tracker, https://github.com/artefactual-labs/cul-spectrum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Click>=8.1.7
+Requires-Dist: Click>=8.0.4
 
 # CUL Spectrum
 
 ## About
 
 CUL Spectrum implements a Python CLI client for the Concordia University Library
 Spectrum REST API.
```

### Comparing `cul-spectrum-1.0.1/README.md` & `cul_spectrum-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cul-spectrum-1.0.1/cul_spectrum/cli.py` & `cul_spectrum-1.0.2/cul_spectrum/cli.py`

 * *Files identical despite different names*

### Comparing `cul-spectrum-1.0.1/cul_spectrum/client.py` & `cul_spectrum-1.0.2/cul_spectrum/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         if "token" in kwargs:
             self.token = kwargs["token"]
 
     def set_uuid(self, uuid, name):
         r = requests.post(
             self.url + "/set_uuid",
             headers={"Authorization": "Basic " + self.token},
-            data={"uuid": uuid, "amid": name},
+            json={"uuid": uuid, "amid": name},
         )
 
         result = {
             "http_status": f"{r.status_code} {r.reason}",
             "http_body": r.text,
         }
```

### Comparing `cul-spectrum-1.0.1/cul_spectrum.egg-info/PKG-INFO` & `cul_spectrum-1.0.2/cul_spectrum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cul-spectrum
-Version: 1.0.1
+Version: 1.0.2
 Summary: Concordia University Library Spectrum Client
 Home-page: https://github.com/artefactual-labs/cul-spectrum
 Author: Artefactual Systems, Inc.
 Author-email: info@artefactual.com
 Project-URL: Bug Tracker, https://github.com/artefactual-labs/cul-spectrum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Click>=8.1.7
+Requires-Dist: Click>=8.0.4
 
 # CUL Spectrum
 
 ## About
 
 CUL Spectrum implements a Python CLI client for the Concordia University Library
 Spectrum REST API.
```

### Comparing `cul-spectrum-1.0.1/setup.cfg` & `cul_spectrum-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
+[bumpversion]
+current_version = 1.0.2
+commit = True
+tag = True
+
 [metadata]
 name = cul-spectrum
-version = 1.0.1
+version = 1.0.2
 author = Artefactual Systems, Inc.
 author_email = info@artefactual.com
 description = Concordia University Library Spectrum Client
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/artefactual-labs/cul-spectrum
 project_urls = 
 	Bug Tracker = https://github.com/artefactual-labs/cul-spectrum/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 
-[bumpversion]
-current_version = 1.0.1
-commit = True
-tag = True
-
 [bumpversion:file:cul_spectrum/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [options]
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	Click>=8.1.7
+	Click>=8.0.4
 
 [options.entry_points]
 console_scripts = 
 	spectrum = cul_spectrum.cli:main
 
 [options.packages.find]
 exclude =
```

### Comparing `cul-spectrum-1.0.1/tests/test_cli.py` & `cul_spectrum-1.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cul-spectrum-1.0.1/tests/test_client.py` & `cul_spectrum-1.0.2/tests/test_client.py`

 * *Files identical despite different names*

