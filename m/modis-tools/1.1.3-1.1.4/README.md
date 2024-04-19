# Comparing `tmp/modis_tools-1.1.3.tar.gz` & `tmp/modis_tools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modis_tools-1.1.3.tar", last modified: Tue Nov 28 15:37:55 2023, max compression
+gzip compressed data, was "modis_tools-1.1.4.tar", last modified: Fri Apr 19 14:33:54 2024, max compression
```

## Comparing `modis_tools-1.1.3.tar` & `modis_tools-1.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-11-28 15:37:55.900264 modis_tools-1.1.3/
--rw-r--r--   0 leith      (502) staff       (20)    10141 2023-07-14 16:52:13.000000 modis_tools-1.1.3/LICENSE
--rw-r--r--   0 leith      (502) staff       (20)       25 2023-07-14 16:52:13.000000 modis_tools-1.1.3/MANIFEST.in
--rw-r--r--   0 leith      (502) staff       (20)    10856 2023-11-28 15:37:55.899997 modis_tools-1.1.3/PKG-INFO
--rw-r--r--   0 leith      (502) staff       (20)    10128 2023-11-28 15:32:13.000000 modis_tools-1.1.3/README.md
-drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-11-28 15:37:55.897270 modis_tools-1.1.3/modis_tools/
--rw-r--r--   0 leith      (502) staff       (20)        0 2023-07-14 16:52:13.000000 modis_tools-1.1.3/modis_tools/__init__.py
--rw-r--r--   0 leith      (502) staff       (20)     2414 2023-07-14 16:52:13.000000 modis_tools-1.1.3/modis_tools/api.py
--rw-r--r--   0 leith      (502) staff       (20)     4022 2023-07-14 16:52:13.000000 modis_tools-1.1.3/modis_tools/auth.py
-drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-11-28 15:37:55.898423 modis_tools-1.1.3/modis_tools/constants/
--rw-r--r--   0 leith      (502) staff       (20)        0 2023-07-14 16:52:13.000000 modis_tools-1.1.3/modis_tools/constants/__init__.py
--rw-r--r--   0 leith      (502) staff       (20)      559 2023-07-14 16:52:13.000000 modis_tools-1.1.3/modis_tools/constants/mimetypes.py
--rw-r--r--   0 leith      (502) staff       (20)      570 2023-11-28 15:32:13.000000 modis_tools-1.1.3/modis_tools/constants/urls.py
--rw-r--r--   0 leith      (502) staff       (20)     1092 2023-08-07 13:19:24.000000 modis_tools-1.1.3/modis_tools/decorators.py
--rw-r--r--   0 leith      (502) staff       (20)     8395 2023-11-28 15:32:13.000000 modis_tools-1.1.3/modis_tools/granule_handler.py
--rw-r--r--   0 leith      (502) staff       (20)     2697 2023-11-28 15:32:13.000000 modis_tools-1.1.3/modis_tools/models.py
--rw-r--r--   0 leith      (502) staff       (20)     8558 2023-08-10 15:13:46.000000 modis_tools-1.1.3/modis_tools/request_helpers.py
--rw-r--r--   0 leith      (502) staff       (20)     4732 2023-08-07 13:19:24.000000 modis_tools-1.1.3/modis_tools/resources.py
-drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-11-28 15:37:55.899588 modis_tools-1.1.3/modis_tools.egg-info/
--rw-r--r--   0 leith      (502) staff       (20)    10856 2023-11-28 15:37:55.000000 modis_tools-1.1.3/modis_tools.egg-info/PKG-INFO
--rw-r--r--   0 leith      (502) staff       (20)      632 2023-11-28 15:37:55.000000 modis_tools-1.1.3/modis_tools.egg-info/SOURCES.txt
--rw-r--r--   0 leith      (502) staff       (20)        1 2023-11-28 15:37:55.000000 modis_tools-1.1.3/modis_tools.egg-info/dependency_links.txt
--rw-r--r--   0 leith      (502) staff       (20)      103 2023-11-28 15:37:55.000000 modis_tools-1.1.3/modis_tools.egg-info/requires.txt
--rw-r--r--   0 leith      (502) staff       (20)       18 2023-11-28 15:37:55.000000 modis_tools-1.1.3/modis_tools.egg-info/top_level.txt
--rw-r--r--   0 leith      (502) staff       (20)       74 2023-07-14 16:52:13.000000 modis_tools-1.1.3/requirements.txt
--rw-r--r--   0 leith      (502) staff       (20)       38 2023-11-28 15:37:55.900307 modis_tools-1.1.3/setup.cfg
--rw-r--r--   0 leith      (502) staff       (20)      916 2023-11-28 15:37:11.000000 modis_tools-1.1.3/setup.py
-drwxr-xr-x   0 leith      (502) staff       (20)        0 2023-11-28 15:37:55.899342 modis_tools-1.1.3/tests/
--rw-r--r--   0 leith      (502) staff       (20)        0 2023-07-14 16:52:13.000000 modis_tools-1.1.3/tests/__init__.py
--rw-r--r--   0 leith      (502) staff       (20)     2422 2023-07-14 16:52:13.000000 modis_tools-1.1.3/tests/test_api.py
--rw-r--r--   0 leith      (502) staff       (20)     3966 2023-07-14 16:52:13.000000 modis_tools-1.1.3/tests/test_auth.py
--rw-r--r--   0 leith      (502) staff       (20)     7991 2023-11-28 15:32:13.000000 modis_tools-1.1.3/tests/test_models.py
--rw-r--r--   0 leith      (502) staff       (20)     6662 2023-07-14 16:52:13.000000 modis_tools-1.1.3/tests/test_request_helpers.py
+drwxr-xr-x   0 jamiesgro   (501) staff       (20)        0 2024-04-19 14:33:54.801072 modis_tools-1.1.4/
+-rw-r--r--   0 jamiesgro   (501) staff       (20)    10141 2022-01-26 21:26:12.000000 modis_tools-1.1.4/LICENSE
+-rw-r--r--   0 jamiesgro   (501) staff       (20)       25 2022-01-26 21:26:12.000000 modis_tools-1.1.4/MANIFEST.in
+-rw-r--r--   0 jamiesgro   (501) staff       (20)    11213 2024-04-19 14:33:54.800800 modis_tools-1.1.4/PKG-INFO
+-rw-r--r--   0 jamiesgro   (501) staff       (20)    10425 2024-04-05 18:19:42.000000 modis_tools-1.1.4/README.md
+drwxr-xr-x   0 jamiesgro   (501) staff       (20)        0 2024-04-19 14:33:54.797540 modis_tools-1.1.4/modis_tools/
+-rw-r--r--   0 jamiesgro   (501) staff       (20)        0 2022-01-26 21:26:12.000000 modis_tools-1.1.4/modis_tools/__init__.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     2414 2022-01-26 21:26:12.000000 modis_tools-1.1.4/modis_tools/api.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     4022 2023-08-08 13:53:15.000000 modis_tools-1.1.4/modis_tools/auth.py
+drwxr-xr-x   0 jamiesgro   (501) staff       (20)        0 2024-04-19 14:33:54.798882 modis_tools-1.1.4/modis_tools/constants/
+-rw-r--r--   0 jamiesgro   (501) staff       (20)        0 2022-01-26 21:26:12.000000 modis_tools-1.1.4/modis_tools/constants/__init__.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)      559 2022-01-26 21:26:12.000000 modis_tools-1.1.4/modis_tools/constants/mimetypes.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)      570 2024-04-05 18:19:42.000000 modis_tools-1.1.4/modis_tools/constants/urls.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     1092 2022-01-26 21:26:12.000000 modis_tools-1.1.4/modis_tools/decorators.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     8395 2024-04-05 18:19:42.000000 modis_tools-1.1.4/modis_tools/granule_handler.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     2697 2024-04-05 18:19:42.000000 modis_tools-1.1.4/modis_tools/models.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     8558 2022-01-26 21:26:12.000000 modis_tools-1.1.4/modis_tools/request_helpers.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     4732 2023-08-08 13:53:15.000000 modis_tools-1.1.4/modis_tools/resources.py
+drwxr-xr-x   0 jamiesgro   (501) staff       (20)        0 2024-04-19 14:33:54.800359 modis_tools-1.1.4/modis_tools.egg-info/
+-rw-r--r--   0 jamiesgro   (501) staff       (20)    11213 2024-04-19 14:33:54.000000 modis_tools-1.1.4/modis_tools.egg-info/PKG-INFO
+-rw-r--r--   0 jamiesgro   (501) staff       (20)      632 2024-04-19 14:33:54.000000 modis_tools-1.1.4/modis_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 jamiesgro   (501) staff       (20)        1 2024-04-19 14:33:54.000000 modis_tools-1.1.4/modis_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 jamiesgro   (501) staff       (20)      151 2024-04-19 14:33:54.000000 modis_tools-1.1.4/modis_tools.egg-info/requires.txt
+-rw-r--r--   0 jamiesgro   (501) staff       (20)       18 2024-04-19 14:33:54.000000 modis_tools-1.1.4/modis_tools.egg-info/top_level.txt
+-rw-r--r--   0 jamiesgro   (501) staff       (20)      116 2024-04-19 14:29:24.000000 modis_tools-1.1.4/requirements.txt
+-rw-r--r--   0 jamiesgro   (501) staff       (20)       38 2024-04-19 14:33:54.801121 modis_tools-1.1.4/setup.cfg
+-rw-r--r--   0 jamiesgro   (501) staff       (20)      916 2024-04-19 14:33:39.000000 modis_tools-1.1.4/setup.py
+drwxr-xr-x   0 jamiesgro   (501) staff       (20)        0 2024-04-19 14:33:54.800115 modis_tools-1.1.4/tests/
+-rw-r--r--   0 jamiesgro   (501) staff       (20)        0 2022-01-26 21:26:12.000000 modis_tools-1.1.4/tests/__init__.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     2422 2022-01-26 21:26:12.000000 modis_tools-1.1.4/tests/test_api.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     3966 2022-01-26 21:26:12.000000 modis_tools-1.1.4/tests/test_auth.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     7991 2024-04-05 18:19:42.000000 modis_tools-1.1.4/tests/test_models.py
+-rw-r--r--   0 jamiesgro   (501) staff       (20)     6662 2022-01-26 21:26:12.000000 modis_tools-1.1.4/tests/test_request_helpers.py
```

### Comparing `modis_tools-1.1.3/LICENSE` & `modis_tools-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/PKG-INFO` & `modis_tools-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: modis_tools
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tools for working with the MODIS API and MODIS data.
 Home-page: https://github.com/fraymio/modis-tools.git
 Author: fraym
 Author-email: datascience@fraym.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.*
 Requires-Dist: pydantic==1.*
 Requires-Dist: python-dateutil==2.*
-Requires-Dist: shapely==1.*
+Requires-Dist: shapely==2.*
 Requires-Dist: tqdm>=4.42.0
+Requires-Dist: setuptools==69.2.0; python_version >= "3.12"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: gdal
 Requires-Dist: gdal; extra == "gdal"
 
 # MODIS Tools
 
@@ -278,7 +279,14 @@
 * Test upload to TestPyPi with `twine upload -r testpypi dist/*`
 * If you haven't set up MFA for PyPi/TestPyPi, use your normal login username
   and password
 * If you have, use `__token__` as the username and an [API
   token](https://pypi.org/help/#apitoken) as your password
 * Assuming the test upload goes smoothly, upload to PyPi with `twine upload dist`
 * Merge the version update branch to main
+
+
+## Issues and Contributing
+
+We welcome any feedback and contributions from the community!
+- To report an issue or to request support, please use the [github issues](https://github.com/fraymio/modis-tools/issues).
+- To contribute, please check out our [contribution guidline](./CONTRIBUTING.md).
```

### Comparing `modis_tools-1.1.3/README.md` & `modis_tools-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -254,8 +254,15 @@
 *The final steps assumes you've set up your PyPi and TestPyPi accounts*
 * Test upload to TestPyPi with `twine upload -r testpypi dist/*`
 * If you haven't set up MFA for PyPi/TestPyPi, use your normal login username
   and password
 * If you have, use `__token__` as the username and an [API
   token](https://pypi.org/help/#apitoken) as your password
 * Assuming the test upload goes smoothly, upload to PyPi with `twine upload dist`
-* Merge the version update branch to main
+* Merge the version update branch to main
+
+
+## Issues and Contributing
+
+We welcome any feedback and contributions from the community!
+- To report an issue or to request support, please use the [github issues](https://github.com/fraymio/modis-tools/issues).
+- To contribute, please check out our [contribution guidline](./CONTRIBUTING.md).
```

### Comparing `modis_tools-1.1.3/modis_tools/api.py` & `modis_tools-1.1.4/modis_tools/api.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/auth.py` & `modis_tools-1.1.4/modis_tools/auth.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/constants/mimetypes.py` & `modis_tools-1.1.4/modis_tools/constants/mimetypes.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/constants/urls.py` & `modis_tools-1.1.4/modis_tools/constants/urls.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/decorators.py` & `modis_tools-1.1.4/modis_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/granule_handler.py` & `modis_tools-1.1.4/modis_tools/granule_handler.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/models.py` & `modis_tools-1.1.4/modis_tools/models.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/request_helpers.py` & `modis_tools-1.1.4/modis_tools/request_helpers.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools/resources.py` & `modis_tools-1.1.4/modis_tools/resources.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/modis_tools.egg-info/PKG-INFO` & `modis_tools-1.1.4/modis_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: modis-tools
-Version: 1.1.3
+Name: modis_tools
+Version: 1.1.4
 Summary: Tools for working with the MODIS API and MODIS data.
 Home-page: https://github.com/fraymio/modis-tools.git
 Author: fraym
 Author-email: datascience@fraym.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.*
 Requires-Dist: pydantic==1.*
 Requires-Dist: python-dateutil==2.*
-Requires-Dist: shapely==1.*
+Requires-Dist: shapely==2.*
 Requires-Dist: tqdm>=4.42.0
+Requires-Dist: setuptools==69.2.0; python_version >= "3.12"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: gdal
 Requires-Dist: gdal; extra == "gdal"
 
 # MODIS Tools
 
@@ -278,7 +279,14 @@
 * Test upload to TestPyPi with `twine upload -r testpypi dist/*`
 * If you haven't set up MFA for PyPi/TestPyPi, use your normal login username
   and password
 * If you have, use `__token__` as the username and an [API
   token](https://pypi.org/help/#apitoken) as your password
 * Assuming the test upload goes smoothly, upload to PyPi with `twine upload dist`
 * Merge the version update branch to main
+
+
+## Issues and Contributing
+
+We welcome any feedback and contributions from the community!
+- To report an issue or to request support, please use the [github issues](https://github.com/fraymio/modis-tools/issues).
+- To contribute, please check out our [contribution guidline](./CONTRIBUTING.md).
```

### Comparing `modis_tools-1.1.3/modis_tools.egg-info/SOURCES.txt` & `modis_tools-1.1.4/modis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/setup.py` & `modis_tools-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     install_requires = fh.read().split()
 
 setuptools.setup(
     name="modis_tools",
-    version="1.1.3",
+    version="1.1.4",
     author="fraym",
     author_email="datascience@fraym.io",
     description="Tools for working with the MODIS API and MODIS data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fraymio/modis-tools.git",
     packages=setuptools.find_packages(),
```

### Comparing `modis_tools-1.1.3/tests/test_api.py` & `modis_tools-1.1.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/tests/test_auth.py` & `modis_tools-1.1.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/tests/test_models.py` & `modis_tools-1.1.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `modis_tools-1.1.3/tests/test_request_helpers.py` & `modis_tools-1.1.4/tests/test_request_helpers.py`

 * *Files identical despite different names*

