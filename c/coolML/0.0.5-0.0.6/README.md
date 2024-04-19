# Comparing `tmp/coolML-0.0.5.tar.gz` & `tmp/coolML-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolML-0.0.5.tar", last modified: Wed Apr 17 11:22:24 2024, max compression
+gzip compressed data, was "coolML-0.0.6.tar", last modified: Fri Apr 19 10:23:51 2024, max compression
```

## Comparing `coolML-0.0.5.tar` & `coolML-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 11:22:24.202565 coolML-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     3617 2024-04-17 11:22:24.202565 coolML-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2911 2024-04-17 11:22:08.000000 coolML-0.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 11:22:24.202565 coolML-0.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1405 2024-04-17 11:22:08.000000 coolML-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 11:22:24.198565 coolML-0.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 11:22:24.202565 coolML-0.0.5/src/coolML/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-17 11:22:08.000000 coolML-0.0.5/src/coolML/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23022 2024-04-17 11:22:08.000000 coolML-0.0.5/src/coolML/data_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     7840 2024-04-17 11:22:08.000000 coolML-0.0.5/src/coolML/model_fitting.py
--rw-rw-rw-   0 root         (0) root         (0)     8424 2024-04-17 11:22:08.000000 coolML-0.0.5/src/coolML/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 11:22:24.202565 coolML-0.0.5/src/coolML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3617 2024-04-17 11:22:24.000000 coolML-0.0.5/src/coolML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2024-04-17 11:22:24.000000 coolML-0.0.5/src/coolML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 11:22:24.000000 coolML-0.0.5/src/coolML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-17 11:22:24.000000 coolML-0.0.5/src/coolML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 11:22:24.000000 coolML-0.0.5/src/coolML.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 10:23:51.105880 coolML-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-04-19 10:23:51.105880 coolML-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2024-04-19 10:23:38.000000 coolML-0.0.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 10:23:51.105880 coolML-0.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2024-04-19 10:23:38.000000 coolML-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 10:23:51.101880 coolML-0.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 10:23:51.101880 coolML-0.0.6/src/coolML/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-19 10:23:38.000000 coolML-0.0.6/src/coolML/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23022 2024-04-19 10:23:38.000000 coolML-0.0.6/src/coolML/data_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7840 2024-04-19 10:23:38.000000 coolML-0.0.6/src/coolML/model_fitting.py
+-rw-rw-rw-   0 root         (0) root         (0)     8424 2024-04-19 10:23:38.000000 coolML-0.0.6/src/coolML/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 10:23:51.105880 coolML-0.0.6/src/coolML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-04-19 10:23:51.000000 coolML-0.0.6/src/coolML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2024-04-19 10:23:51.000000 coolML-0.0.6/src/coolML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 10:23:51.000000 coolML-0.0.6/src/coolML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-19 10:23:51.000000 coolML-0.0.6/src/coolML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-19 10:23:51.000000 coolML-0.0.6/src/coolML.egg-info/top_level.txt
```

### Comparing `coolML-0.0.5/PKG-INFO` & `coolML-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolML
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -14,24 +14,24 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Cool ML
 
 Cool Ml is a tool developed in the University of Santiago de Compostela in collaboration with the IM2NP of Aix-Marseille Université. This tool aims to accelerate the optimization of double asymmetric barrier heterostructures. The potential profile of this devices is shown in Fig. 1.
 
-![img](images/Cooling_device.png)
+!["image/png"](images/Cooling_device.png)
 
 **Fig.1:** Lb1, LQW, and Lb2, are the lengths of the first barrier (b1),  quantum well (QW), and the second barrier (b2), respectively. The height of the first barrier (hb1) is determined from the band offset between AlAs and the emitter, and the height of the second barrier (hb2) is proportional to gamma, which is the fraction of aluminium in the alloy. V is the bias between the Efe and the Efc, V=Efe-Efc. W1 is the energy interval between the Eo and Efe. The W2 is the energy interval between Eo and the Eb2.
 
 This code consists of a double machine learning workflow based on two multi-layer perceptron neural networks, with the ability of predict not only the energetic and thermal properties of the device but also the whole potential profile, from design parameters.
 
 The machine learning workflow is feeded with data from the accurate NEGF simulation methodology coupled with the heat equation. More information about the NEGF+H methodology is shared in [BESCOND:Phys. Rev. Applied:2020](https://doi.org/10.1103/PhysRevApplied.14.064022).
 
 
-Data used to feed the neural networks is shared in the following [Zenodo Repository with DOI:](https://doi.org/10.1103/PhysRevApplied.14.064022).
+Data used to feed the neural networks is shared in the following [Zenodo Repository with DOI: NOT WORKING BY NOW](https://doi.org/10.1103/PhysRevApplied.14.064022).
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
```

### Comparing `coolML-0.0.5/README.md` & `coolML-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Cool ML
 
 Cool Ml is a tool developed in the University of Santiago de Compostela in collaboration with the IM2NP of Aix-Marseille Université. This tool aims to accelerate the optimization of double asymmetric barrier heterostructures. The potential profile of this devices is shown in Fig. 1.
 
-![img](images/Cooling_device.png)
+!["image/png"](images/Cooling_device.png)
 
 **Fig.1:** Lb1, LQW, and Lb2, are the lengths of the first barrier (b1),  quantum well (QW), and the second barrier (b2), respectively. The height of the first barrier (hb1) is determined from the band offset between AlAs and the emitter, and the height of the second barrier (hb2) is proportional to gamma, which is the fraction of aluminium in the alloy. V is the bias between the Efe and the Efc, V=Efe-Efc. W1 is the energy interval between the Eo and Efe. The W2 is the energy interval between Eo and the Eb2.
 
 This code consists of a double machine learning workflow based on two multi-layer perceptron neural networks, with the ability of predict not only the energetic and thermal properties of the device but also the whole potential profile, from design parameters.
 
 The machine learning workflow is feeded with data from the accurate NEGF simulation methodology coupled with the heat equation. More information about the NEGF+H methodology is shared in [BESCOND:Phys. Rev. Applied:2020](https://doi.org/10.1103/PhysRevApplied.14.064022).
 
 
-Data used to feed the neural networks is shared in the following [Zenodo Repository with DOI:](https://doi.org/10.1103/PhysRevApplied.14.064022).
+Data used to feed the neural networks is shared in the following [Zenodo Repository with DOI: NOT WORKING BY NOW](https://doi.org/10.1103/PhysRevApplied.14.064022).
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
```

### Comparing `coolML-0.0.5/setup.py` & `coolML-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='coolML',
-    version='0.0.5',
+    version='0.0.6',
     description='Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Julian Garcia Fernandez ',
     author_email='julian.garcia.fernandez2@usc.es',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML',
     setup_requires=['setuptools'],
```

### Comparing `coolML-0.0.5/src/coolML/data_processing.py` & `coolML-0.0.6/src/coolML/data_processing.py`

 * *Files identical despite different names*

### Comparing `coolML-0.0.5/src/coolML/model_fitting.py` & `coolML-0.0.6/src/coolML/model_fitting.py`

 * *Files identical despite different names*

### Comparing `coolML-0.0.5/src/coolML/models.py` & `coolML-0.0.6/src/coolML/models.py`

 * *Files identical despite different names*

### Comparing `coolML-0.0.5/src/coolML.egg-info/PKG-INFO` & `coolML-0.0.6/src/coolML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolML
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -14,24 +14,24 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Cool ML
 
 Cool Ml is a tool developed in the University of Santiago de Compostela in collaboration with the IM2NP of Aix-Marseille Université. This tool aims to accelerate the optimization of double asymmetric barrier heterostructures. The potential profile of this devices is shown in Fig. 1.
 
-![img](images/Cooling_device.png)
+!["image/png"](images/Cooling_device.png)
 
 **Fig.1:** Lb1, LQW, and Lb2, are the lengths of the first barrier (b1),  quantum well (QW), and the second barrier (b2), respectively. The height of the first barrier (hb1) is determined from the band offset between AlAs and the emitter, and the height of the second barrier (hb2) is proportional to gamma, which is the fraction of aluminium in the alloy. V is the bias between the Efe and the Efc, V=Efe-Efc. W1 is the energy interval between the Eo and Efe. The W2 is the energy interval between Eo and the Eb2.
 
 This code consists of a double machine learning workflow based on two multi-layer perceptron neural networks, with the ability of predict not only the energetic and thermal properties of the device but also the whole potential profile, from design parameters.
 
 The machine learning workflow is feeded with data from the accurate NEGF simulation methodology coupled with the heat equation. More information about the NEGF+H methodology is shared in [BESCOND:Phys. Rev. Applied:2020](https://doi.org/10.1103/PhysRevApplied.14.064022).
 
 
-Data used to feed the neural networks is shared in the following [Zenodo Repository with DOI:](https://doi.org/10.1103/PhysRevApplied.14.064022).
+Data used to feed the neural networks is shared in the following [Zenodo Repository with DOI: NOT WORKING BY NOW](https://doi.org/10.1103/PhysRevApplied.14.064022).
 
 ## Installation
 First you need to have installed **pip3** on your system. For Ubuntu, open up a terminal and type:
 
     sudo apt update
     sudo apt install python3-pip
```
