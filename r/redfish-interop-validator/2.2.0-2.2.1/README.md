# Comparing `tmp/redfish_interop_validator-2.2.0.tar.gz` & `tmp/redfish_interop_validator-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_interop_validator-2.2.0.tar", last modified: Fri Mar 22 19:23:49 2024, max compression
+gzip compressed data, was "redfish_interop_validator-2.2.1.tar", last modified: Fri Apr 19 19:58:50 2024, max compression
```

## Comparing `redfish_interop_validator-2.2.0.tar` & `redfish_interop_validator-2.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:23:49.406084 redfish_interop_validator-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-03-22 19:23:49.406084 redfish_interop_validator-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:23:49.402084 redfish_interop_validator-2.2.0/redfish_interop_validator/
--rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/RedfishInteropValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24266 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/RedfishLogo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/interop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/redfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/traverseInterop.py
--rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/redfish_interop_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:23:49.406084 redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-03-22 19:23:49.000000 redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-22 19:23:49.000000 redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 19:23:49.000000 redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-22 19:23:49.000000 redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-22 19:23:49.000000 redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-22 19:23:49.000000 redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 19:23:49.406084 redfish_interop_validator-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-22 19:23:34.000000 redfish_interop_validator-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/redfish_interop_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)    14138 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishInteropValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24266 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishLogo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36562 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/interop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/redfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21860 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/traverseInterop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21798 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/redfish_interop_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 19:58:50.000000 redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:58:50.833555 redfish_interop_validator-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 19:58:41.000000 redfish_interop_validator-2.2.1/setup.py
```

### Comparing `redfish_interop_validator-2.2.0/LICENSE.md` & `redfish_interop_validator-2.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/PKG-INFO` & `redfish_interop_validator-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_interop_validator
-Version: 2.2.0
+Version: 2.2.1
 Summary: Redfish Interop Validator
 Home-page: https://github.com/DMTF/Redfish-Interop-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_interop_validator-2.2.0/README.md` & `redfish_interop_validator-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/RedfishInteropValidator.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishInteropValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from urllib.parse import urlparse
 from collections import Counter
 
 import redfish_interop_validator.traverseInterop as traverseInterop
 from redfish_interop_validator.profile import getProfiles, checkProfileAgainstSchema, hashProfile
 from redfish_interop_validator.validateResource import validateSingleURI, validateURITree
 
-tool_version = '2.2.0'
+tool_version = '2.2.1'
 
 # Set up the custom debug levels
 VERBOSE1 = logging.INFO - 1
 VERBOSE2 = logging.INFO - 2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
```

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/RedfishLogo.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/config.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/interop.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/interop.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/profile.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/profile.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/redfish.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/redfish.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/session.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/session.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/tohtml.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/traverseInterop.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/traverseInterop.py`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator/validateResource.py` & `redfish_interop_validator-2.2.1/redfish_interop_validator/validateResource.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,15 +342,15 @@
                         "SubordinateTo": set([tuple(reversed(subordinate_tree))]),
                         "UseCasesFound": set(usecases_found),
                     }
                 else:
                     resource_stats[SchemaType]['Exists'] = True
                     resource_stats[SchemaType]['URIsFound'].append(link.rstrip('/'))
                     resource_stats[SchemaType]['SubordinateTo'].add(tuple(reversed(subordinate_tree)))
-                    resource_stats[SchemaType]['UseCasesFound'].union(usecases_found)
+                    resource_stats[SchemaType]['UseCasesFound'] = resource_stats[SchemaType]['UseCasesFound'].union(usecases_found)
 
             if refLinks is not currentLinks and len(newLinks) == 0 and len(refLinks) > 0:
                 currentLinks = refLinks
             else:
                 currentLinks = newLinks
 
         my_logger.info('Service Level Checks')
```

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/PKG-INFO` & `redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_interop_validator
-Version: 2.2.0
+Version: 2.2.1
 Summary: Redfish Interop Validator
 Home-page: https://github.com/DMTF/Redfish-Interop-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_interop_validator-2.2.0/redfish_interop_validator.egg-info/SOURCES.txt` & `redfish_interop_validator-2.2.1/redfish_interop_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_interop_validator-2.2.0/setup.py` & `redfish_interop_validator-2.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_interop_validator",
-    version="2.2.0",
+    version="2.2.1",
     description="Redfish Interop Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

