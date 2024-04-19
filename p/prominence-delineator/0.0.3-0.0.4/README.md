# Comparing `tmp/prominence_delineator-0.0.3.tar.gz` & `tmp/prominence_delineator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prominence_delineator-0.0.3.tar", last modified: Fri Apr 19 10:08:11 2024, max compression
+gzip compressed data, was "prominence_delineator-0.0.4.tar", last modified: Fri Apr 19 10:22:37 2024, max compression
```

## Comparing `prominence_delineator-0.0.3.tar` & `prominence_delineator-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:08:11.332500 prominence_delineator-0.0.3/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.3/LICENSE
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45744 2024-04-19 10:08:11.331162 prominence_delineator-0.0.3/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)     4155 2024-04-19 08:59:11.000000 prominence_delineator-0.0.3/README.md
--rw-r--r--   0 jea7h      (922) spgstud    (504)     1081 2024-04-19 10:08:01.000000 prominence_delineator-0.0.3/pyproject.toml
--rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-19 10:08:11.332765 prominence_delineator-0.0.3/setup.cfg
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:08:11.289663 prominence_delineator-0.0.3/src/
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:08:11.302884 prominence_delineator-0.0.3/src/prominence_delineator/
--rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.3/src/prominence_delineator/__init__.py
--rw-r--r--   0 jea7h      (922) spgstud    (504)    17329 2024-04-04 10:04:51.000000 prominence_delineator-0.0.3/src/prominence_delineator/prominence_delineator.py
-drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:08:11.324763 prominence_delineator-0.0.3/src/prominence_delineator.egg-info/
--rw-r--r--   0 jea7h      (922) spgstud    (504)    45744 2024-04-19 10:08:11.000000 prominence_delineator-0.0.3/src/prominence_delineator.egg-info/PKG-INFO
--rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-19 10:08:11.000000 prominence_delineator-0.0.3/src/prominence_delineator.egg-info/SOURCES.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-19 10:08:11.000000 prominence_delineator-0.0.3/src/prominence_delineator.egg-info/dependency_links.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)      106 2024-04-19 10:08:11.000000 prominence_delineator-0.0.3/src/prominence_delineator.egg-info/requires.txt
--rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-19 10:08:11.000000 prominence_delineator-0.0.3/src/prominence_delineator.egg-info/top_level.txt
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.488569 prominence_delineator-0.0.4/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    35149 2024-04-04 09:00:43.000000 prominence_delineator-0.0.4/LICENSE
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-19 10:22:37.487465 prominence_delineator-0.0.4/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     4151 2024-04-19 10:22:04.000000 prominence_delineator-0.0.4/README.md
+-rw-r--r--   0 jea7h      (922) spgstud    (504)     1122 2024-04-19 10:19:34.000000 prominence_delineator-0.0.4/pyproject.toml
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       38 2024-04-19 10:22:37.488780 prominence_delineator-0.0.4/setup.cfg
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.455399 prominence_delineator-0.0.4/src/
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.464391 prominence_delineator-0.0.4/src/prominence_delineator/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       76 2024-04-02 12:11:52.000000 prominence_delineator-0.0.4/src/prominence_delineator/__init__.py
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    17329 2024-04-04 10:04:51.000000 prominence_delineator-0.0.4/src/prominence_delineator/prominence_delineator.py
+drwxr-xr-x   0 jea7h      (922) spgstud    (504)        0 2024-04-19 10:22:37.481078 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/
+-rw-r--r--   0 jea7h      (922) spgstud    (504)    45858 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/PKG-INFO
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      365 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/SOURCES.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)        1 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/dependency_links.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)      141 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/requires.txt
+-rw-r--r--   0 jea7h      (922) spgstud    (504)       22 2024-04-19 10:22:37.000000 prominence_delineator-0.0.4/src/prominence_delineator.egg-info/top_level.txt
```

### Comparing `prominence_delineator-0.0.3/LICENSE` & `prominence_delineator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.3/PKG-INFO` & `prominence_delineator-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -691,16 +691,19 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Provides-Extra: rpeak
 Requires-Dist: vg-beat-detectors; extra == "rpeak"
 Provides-Extra: cleaning
 Requires-Dist: neurokit2; extra == "cleaning"
+Provides-Extra: example
+Requires-Dist: matplotlib; extra == "example"
+Requires-Dist: wfdb; extra == "example"
 Provides-Extra: all
-Requires-Dist: prominence-delineator[cleaning,rpeak]; extra == "all"
+Requires-Dist: prominence-delineator[cleaning,example,rpeak]; extra == "all"
 
 # Physiology-Informed ECG Delineation Based on Peak Prominence
 
 This Python package implements the Peak Prominence ECG Delineator \[1\] and provides methods for ECG cleaning and R-peak detection \[2\], resulting in a complete delineation pipeline. This delineator allows for fast and precise detection of the positions, on- and offsets of morphology waves (e.g., _P_, _R_, _T_) in single or multi-lead ECG signals. An optional multi-lead correction procedure can be applied, leveraging information from all leads if available. 
 
 ## Advantages and Limits
 This proposed approach achieves a highly explainable and interpretable wave selection by leveraging prominence information. Hence, wave detection only depends on physiologically motivated parameters chosen so that morphologies of interest are well represented and portrayed, yielding high $F_1$-scores and low errors on established Datasets in comparison to competing methods \[1\]. 
@@ -709,15 +712,15 @@
 
 
 
 ## Installation
 
 You can install the latest version of the `prominence-delineator` package from the Python Package Index (PyPI) by running:
 ```
-    pip install prominence-delineator
+pip install prominence-delineator
 ```
 
 ## Usage
 
 A complete working example is provided in [example.ipynb](https://github.com/JonasEmrich/prominence-delineator/blob/main/example/example.ipynb), additionally the basic usage is depicted below.
 The ProminenceDelineator takes the `sampling_frequency` and optionally several physiological parameters as input.
 Then, R-peaks can be detected using any reliable R-peak detector or with the integrated method (applying the `FastNVG` \[2\] approach). Before detecting further waves, the required ECG cleaning can easily be performed by using `.clean_ecg(ecg)`.
```

### Comparing `prominence_delineator-0.0.3/README.md` & `prominence_delineator-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 
 ## Installation
 
 You can install the latest version of the `prominence-delineator` package from the Python Package Index (PyPI) by running:
 ```
-    pip install prominence-delineator
+pip install prominence-delineator
 ```
 
 ## Usage
 
 A complete working example is provided in [example.ipynb](https://github.com/JonasEmrich/prominence-delineator/blob/main/example/example.ipynb), additionally the basic usage is depicted below.
 The ProminenceDelineator takes the `sampling_frequency` and optionally several physiological parameters as input.
 Then, R-peaks can be detected using any reliable R-peak detector or with the integrated method (applying the `FastNVG` \[2\] approach). Before detecting further waves, the required ECG cleaning can easily be performed by using `.clean_ecg(ecg)`.
```

### Comparing `prominence_delineator-0.0.3/pyproject.toml` & `prominence_delineator-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prominence-delineator"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
   "numpy",
   "scipy",
 ]
 requires-python = ">=3.8"
 authors = [
     {name="Jonas Emrich", email="mail@jonasemrich.de"}
@@ -26,12 +26,13 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
 ]
 
 [project.optional-dependencies]
 rpeak = ["vg-beat-detectors"]
 cleaning = ["neurokit2"]
-all = ["prominence-delineator[rpeak,cleaning]"]
+example = ["matplotlib", "wfdb"]
+all = ["prominence-delineator[rpeak,cleaning,example]"]
 
 [project.urls]
 "Homepage" = "https://jonasemrich.de"
 "Source Code" = "https://github.com/JonasEmrich/prominence-delineator"
```

### Comparing `prominence_delineator-0.0.3/src/prominence_delineator/prominence_delineator.py` & `prominence_delineator-0.0.4/src/prominence_delineator/prominence_delineator.py`

 * *Files identical despite different names*

### Comparing `prominence_delineator-0.0.3/src/prominence_delineator.egg-info/PKG-INFO` & `prominence_delineator-0.0.4/src/prominence_delineator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prominence-delineator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Physiology-Informed ECG Delineator Based on Peak Prominence
 Author-email: Jonas Emrich <mail@jonasemrich.de>
 Maintainer-email: Jonas Emrich <mail@jonasemrich.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -691,16 +691,19 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Provides-Extra: rpeak
 Requires-Dist: vg-beat-detectors; extra == "rpeak"
 Provides-Extra: cleaning
 Requires-Dist: neurokit2; extra == "cleaning"
+Provides-Extra: example
+Requires-Dist: matplotlib; extra == "example"
+Requires-Dist: wfdb; extra == "example"
 Provides-Extra: all
-Requires-Dist: prominence-delineator[cleaning,rpeak]; extra == "all"
+Requires-Dist: prominence-delineator[cleaning,example,rpeak]; extra == "all"
 
 # Physiology-Informed ECG Delineation Based on Peak Prominence
 
 This Python package implements the Peak Prominence ECG Delineator \[1\] and provides methods for ECG cleaning and R-peak detection \[2\], resulting in a complete delineation pipeline. This delineator allows for fast and precise detection of the positions, on- and offsets of morphology waves (e.g., _P_, _R_, _T_) in single or multi-lead ECG signals. An optional multi-lead correction procedure can be applied, leveraging information from all leads if available. 
 
 ## Advantages and Limits
 This proposed approach achieves a highly explainable and interpretable wave selection by leveraging prominence information. Hence, wave detection only depends on physiologically motivated parameters chosen so that morphologies of interest are well represented and portrayed, yielding high $F_1$-scores and low errors on established Datasets in comparison to competing methods \[1\]. 
@@ -709,15 +712,15 @@
 
 
 
 ## Installation
 
 You can install the latest version of the `prominence-delineator` package from the Python Package Index (PyPI) by running:
 ```
-    pip install prominence-delineator
+pip install prominence-delineator
 ```
 
 ## Usage
 
 A complete working example is provided in [example.ipynb](https://github.com/JonasEmrich/prominence-delineator/blob/main/example/example.ipynb), additionally the basic usage is depicted below.
 The ProminenceDelineator takes the `sampling_frequency` and optionally several physiological parameters as input.
 Then, R-peaks can be detected using any reliable R-peak detector or with the integrated method (applying the `FastNVG` \[2\] approach). Before detecting further waves, the required ECG cleaning can easily be performed by using `.clean_ecg(ecg)`.
```

