# Comparing `tmp/FlowKit-1.1.0.tar.gz` & `tmp/flowkit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowKit-1.1.0.tar", last modified: Fri Apr  5 04:46:34 2024, max compression
+gzip compressed data, was "flowkit-1.1.1.tar", last modified: Fri Apr 19 18:53:23 2024, max compression
```

## Comparing `FlowKit-1.1.0.tar` & `flowkit-1.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     1511 2019-08-08 15:30:26.000000 FlowKit-1.1.0/LICENSE
--rw-r--r--   0 swhite   (957844952) domain users (957800513)       48 2024-04-02 17:50:51.000000 FlowKit-1.1.0/MANIFEST.in
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    10601 2024-04-05 04:46:34.151234 FlowKit-1.1.0/PKG-INFO
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     9802 2024-04-02 17:50:51.000000 FlowKit-1.1.0/README.md
--rw-r--r--   0 swhite   (957844952) domain users (957800513)       88 2024-04-02 17:50:52.000000 FlowKit-1.1.0/pyproject.toml
--rw-r--r--   0 swhite   (957844952) domain users (957800513)       38 2024-04-05 04:46:34.151234 FlowKit-1.1.0/setup.cfg
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     1475 2024-04-04 16:10:48.000000 FlowKit-1.1.0/setup.py
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/FlowKit.egg-info/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    10601 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/PKG-INFO
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     1446 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/SOURCES.txt
--rw-r--r--   0 swhite   (957844952) domain users (957800513)        1 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/dependency_links.txt
--rw-r--r--   0 swhite   (957844952) domain users (957800513)      156 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/requires.txt
--rw-r--r--   0 swhite   (957844952) domain users (957800513)        8 2024-04-05 04:46:34.000000 FlowKit-1.1.0/src/FlowKit.egg-info/top_level.txt
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     1061 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/__init__.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)      769 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_conf.py
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_models/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)       36 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/__init__.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     5252 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/dimension.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     3274 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gate_node.py
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_models/gates/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)      251 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/__init__.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     1174 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_base_gate.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    15888 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_gates.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    13806 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_gml_gates.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     9766 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gates/_wsp_gates.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     6399 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gating_results.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    37938 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/gating_strategy.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    54529 2024-04-04 21:42:11.000000 FlowKit-1.1.0/src/flowkit/_models/sample.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    26532 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/session.py
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_models/transforms/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)      446 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/__init__.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     1515 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_base_transform.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     5307 2024-04-04 21:42:11.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_matrix.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    11735 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_transforms.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     8353 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/transforms/_wsp_transforms.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    32166 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_models/workspace.py
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_resources/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     4837 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/DataTypes.v2.0.xsd
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    11485 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/Gating-ML.v2.0.xsd
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     9210 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/Transformations.v2.0.xsd
--rw-r--r--   0 swhite   (957844952) domain users (957800513)      814 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_resources/__init__.py
-drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-05 04:46:34.151234 FlowKit-1.1.0/src/flowkit/_utils/
--rw-r--r--   0 swhite   (957844952) domain users (957800513)       21 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/__init__.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     4790 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/gating_utils.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    12097 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/gml_write.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    31092 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/plot_utils.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     4693 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/sample_utils.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    46376 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/wsp_utils.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)     2303 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/xml_common.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)    21437 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/_utils/xml_utils.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)       46 2024-04-04 23:47:31.000000 FlowKit-1.1.0/src/flowkit/_version.py
--rw-r--r--   0 swhite   (957844952) domain users (957800513)      954 2024-04-02 17:50:52.000000 FlowKit-1.1.0/src/flowkit/exceptions.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1511 2024-04-19 18:49:22.000000 flowkit-1.1.1/LICENSE
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       48 2024-04-19 18:49:22.000000 flowkit-1.1.1/MANIFEST.in
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    10429 2024-04-19 18:53:23.098187 flowkit-1.1.1/PKG-INFO
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     9630 2024-04-19 18:49:22.000000 flowkit-1.1.1/README.md
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       88 2024-04-19 18:49:22.000000 flowkit-1.1.1/pyproject.toml
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       38 2024-04-19 18:53:23.098187 flowkit-1.1.1/setup.cfg
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1475 2024-04-19 18:49:22.000000 flowkit-1.1.1/setup.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.094187 flowkit-1.1.1/src/
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/src/FlowKit.egg-info/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    10429 2024-04-19 18:53:23.000000 flowkit-1.1.1/src/FlowKit.egg-info/PKG-INFO
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1446 2024-04-19 18:53:23.000000 flowkit-1.1.1/src/FlowKit.egg-info/SOURCES.txt
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)        1 2024-04-19 18:53:23.000000 flowkit-1.1.1/src/FlowKit.egg-info/dependency_links.txt
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      156 2024-04-19 18:53:23.000000 flowkit-1.1.1/src/FlowKit.egg-info/requires.txt
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)        8 2024-04-19 18:53:23.000000 flowkit-1.1.1/src/FlowKit.egg-info/top_level.txt
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/src/flowkit/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1061 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      769 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_conf.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/src/flowkit/_models/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       36 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     5252 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/dimension.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     3274 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gate_node.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/src/flowkit/_models/gates/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      251 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gates/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1174 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gates/_base_gate.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    15888 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gates/_gates.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    13806 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gates/_gml_gates.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     9766 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gates/_wsp_gates.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     6399 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gating_results.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    37938 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/gating_strategy.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    54529 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/sample.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    26532 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/session.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/src/flowkit/_models/transforms/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      446 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/transforms/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     1515 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/transforms/_base_transform.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     5307 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/transforms/_matrix.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    11735 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/transforms/_transforms.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     8353 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/transforms/_wsp_transforms.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    32166 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_models/workspace.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/src/flowkit/_resources/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     4837 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_resources/DataTypes.v2.0.xsd
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    11485 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_resources/Gating-ML.v2.0.xsd
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     9210 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_resources/Transformations.v2.0.xsd
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      553 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_resources/__init__.py
+drwxr-xr-x   0 swhite   (957844952) domain users (957800513)        0 2024-04-19 18:53:23.098187 flowkit-1.1.1/src/flowkit/_utils/
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       21 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/__init__.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     4790 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/gating_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    12097 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/gml_write.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    31092 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/plot_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     4693 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/sample_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    46376 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/wsp_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)     2303 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/xml_common.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)    21437 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_utils/xml_utils.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)       46 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/_version.py
+-rw-r--r--   0 swhite   (957844952) domain users (957800513)      954 2024-04-19 18:49:22.000000 flowkit-1.1.1/src/flowkit/exceptions.py
```

### Comparing `FlowKit-1.1.0/LICENSE` & `flowkit-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/PKG-INFO` & `flowkit-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowKit
-Version: 1.1.0
+Version: 1.1.1
 Summary: Flow Cytometry Toolkit
 Home-page: https://github.com/whitews/flowkit
 Author: Scott White
 License: BSD
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
@@ -130,22 +130,21 @@
 
 ```
 pip install flowkit
 ```
 
 ### From source
 
-Clone the repository and ensure `pip` is up-to-date. It is recommended to use `pip` to install requirements as relying on `setuptools` may result in incompatible dependency versions.
+Clone the repository and ensure `pip` is up-to-date.
 
 ```
 git clone https://github.com/whitews/flowkit
 cd flowkit
 pip install --upgrade pip
-pip install -r requirements.txt
-python setup.py install
+pip install .
 ```
 
 ## Documentation
 
 The FlowKit API documentation is available [on ReadTheDocs here](https://flowkit.readthedocs.io/en/latest/?badge=latest). The tutorial notebooks in the `docs/notebooks` directory are a great place to get started with FlowKit, and are linked below.
 If you have any questions about FlowKit, find any bugs, or feel something is missing from the tutorials below [please submit an issue to the GitHub repository here](https://github.com/whitews/FlowKit/issues/new/).
```

### Comparing `FlowKit-1.1.0/README.md` & `flowkit-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,22 +104,21 @@
 
 ```
 pip install flowkit
 ```
 
 ### From source
 
-Clone the repository and ensure `pip` is up-to-date. It is recommended to use `pip` to install requirements as relying on `setuptools` may result in incompatible dependency versions.
+Clone the repository and ensure `pip` is up-to-date.
 
 ```
 git clone https://github.com/whitews/flowkit
 cd flowkit
 pip install --upgrade pip
-pip install -r requirements.txt
-python setup.py install
+pip install .
 ```
 
 ## Documentation
 
 The FlowKit API documentation is available [on ReadTheDocs here](https://flowkit.readthedocs.io/en/latest/?badge=latest). The tutorial notebooks in the `docs/notebooks` directory are a great place to get started with FlowKit, and are linked below.
 If you have any questions about FlowKit, find any bugs, or feel something is missing from the tutorials below [please submit an issue to the GitHub repository here](https://github.com/whitews/FlowKit/issues/new/).
```

### Comparing `FlowKit-1.1.0/setup.py` & `flowkit-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/FlowKit.egg-info/PKG-INFO` & `flowkit-1.1.1/src/FlowKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowKit
-Version: 1.1.0
+Version: 1.1.1
 Summary: Flow Cytometry Toolkit
 Home-page: https://github.com/whitews/flowkit
 Author: Scott White
 License: BSD
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
@@ -130,22 +130,21 @@
 
 ```
 pip install flowkit
 ```
 
 ### From source
 
-Clone the repository and ensure `pip` is up-to-date. It is recommended to use `pip` to install requirements as relying on `setuptools` may result in incompatible dependency versions.
+Clone the repository and ensure `pip` is up-to-date.
 
 ```
 git clone https://github.com/whitews/flowkit
 cd flowkit
 pip install --upgrade pip
-pip install -r requirements.txt
-python setup.py install
+pip install .
 ```
 
 ## Documentation
 
 The FlowKit API documentation is available [on ReadTheDocs here](https://flowkit.readthedocs.io/en/latest/?badge=latest). The tutorial notebooks in the `docs/notebooks` directory are a great place to get started with FlowKit, and are linked below.
 If you have any questions about FlowKit, find any bugs, or feel something is missing from the tutorials below [please submit an issue to the GitHub repository here](https://github.com/whitews/FlowKit/issues/new/).
```

### Comparing `FlowKit-1.1.0/src/FlowKit.egg-info/SOURCES.txt` & `flowkit-1.1.1/src/FlowKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/__init__.py` & `flowkit-1.1.1/src/flowkit/__init__.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_conf.py` & `flowkit-1.1.1/src/flowkit/_conf.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/dimension.py` & `flowkit-1.1.1/src/flowkit/_models/dimension.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/gate_node.py` & `flowkit-1.1.1/src/flowkit/_models/gate_node.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/gates/_base_gate.py` & `flowkit-1.1.1/src/flowkit/_models/gates/_base_gate.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/gates/_gates.py` & `flowkit-1.1.1/src/flowkit/_models/gates/_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/gates/_gml_gates.py` & `flowkit-1.1.1/src/flowkit/_models/gates/_gml_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/gates/_wsp_gates.py` & `flowkit-1.1.1/src/flowkit/_models/gates/_wsp_gates.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/gating_results.py` & `flowkit-1.1.1/src/flowkit/_models/gating_results.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/gating_strategy.py` & `flowkit-1.1.1/src/flowkit/_models/gating_strategy.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/sample.py` & `flowkit-1.1.1/src/flowkit/_models/sample.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/session.py` & `flowkit-1.1.1/src/flowkit/_models/session.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/transforms/_base_transform.py` & `flowkit-1.1.1/src/flowkit/_models/transforms/_base_transform.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/transforms/_matrix.py` & `flowkit-1.1.1/src/flowkit/_models/transforms/_matrix.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/transforms/_transforms.py` & `flowkit-1.1.1/src/flowkit/_models/transforms/_transforms.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/transforms/_wsp_transforms.py` & `flowkit-1.1.1/src/flowkit/_models/transforms/_wsp_transforms.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_models/workspace.py` & `flowkit-1.1.1/src/flowkit/_models/workspace.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_resources/DataTypes.v2.0.xsd` & `flowkit-1.1.1/src/flowkit/_resources/DataTypes.v2.0.xsd`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_resources/Gating-ML.v2.0.xsd` & `flowkit-1.1.1/src/flowkit/_resources/Gating-ML.v2.0.xsd`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_resources/Transformations.v2.0.xsd` & `flowkit-1.1.1/src/flowkit/_resources/Transformations.v2.0.xsd`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_utils/gating_utils.py` & `flowkit-1.1.1/src/flowkit/_utils/gating_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_utils/gml_write.py` & `flowkit-1.1.1/src/flowkit/_utils/gml_write.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_utils/plot_utils.py` & `flowkit-1.1.1/src/flowkit/_utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_utils/sample_utils.py` & `flowkit-1.1.1/src/flowkit/_utils/sample_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_utils/wsp_utils.py` & `flowkit-1.1.1/src/flowkit/_utils/wsp_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_utils/xml_common.py` & `flowkit-1.1.1/src/flowkit/_utils/xml_common.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/_utils/xml_utils.py` & `flowkit-1.1.1/src/flowkit/_utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `FlowKit-1.1.0/src/flowkit/exceptions.py` & `flowkit-1.1.1/src/flowkit/exceptions.py`

 * *Files identical despite different names*

