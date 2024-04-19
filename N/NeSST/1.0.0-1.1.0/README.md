# Comparing `tmp/NeSST-1.0.0.tar.gz` & `tmp/nesst-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeSST-1.0.0.tar", last modified: Tue Apr  2 10:06:02 2024, max compression
+gzip compressed data, was "nesst-1.1.0.tar", last modified: Fri Apr 19 10:29:52 2024, max compression
```

## Comparing `NeSST-1.0.0.tar` & `nesst-1.1.0.tar`

### file list

```diff
@@ -1,60 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:02.211508 NeSST-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 10:05:57.000000 NeSST-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-02 10:06:02.211508 NeSST-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-02 10:05:57.000000 NeSST-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-02 10:05:57.000000 NeSST-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:06:02.211508 NeSST-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:02.195508 NeSST-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:02.199508 NeSST-1.0.0/src/NeSST/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/cross_sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:02.211508 NeSST-1.0.0/src/NeSST/data/
--rw-r--r--   0 runner    (1001) docker     (127)    22889 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/CENDL_C12(n,elastic)_dx.dat
--rw-r--r--   0 runner    (1001) docker     (127)    18651 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/CENDL_C12(n,elastic)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/CENDL_C12(n,n1)_dx.dat
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/CENDL_C12(n,n1)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)    24149 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/CENDL_C12_totxsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)  1235112 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/CENDL_d(n,2n)_ddx.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/CENDL_d(n,2n)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)  1000100 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/Dn2n_matrix.dat
--rw-r--r--   0 runner    (1001) docker     (127)   565663 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_Be9(n,2n)_ddx.dat
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_Be9(n,2n)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_Be9(n,elastic)_dx.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_Be9(n,elastic)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_H1(n,elastic)_dx.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_H1(n,elastic)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_H2(n,elastic)_dx.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_H2(n,elastic)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_H3(n,elastic)_dx.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_H3(n,elastic)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_nBe9_totxsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_nH2_totxsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_nH3_totxsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/ENDF_t(n,2n)_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/TT_reac_ENDF.dat
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/TT_reac_McNally.dat
--rw-r--r--   0 runner    (1001) docker     (127)   410500 2024-04-02 10:05:57.000000 NeSST-1.0.0/src/NeSST/data/TT_spec_temprange.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1000100 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/data/Tn2n_matrix_CENDL_transform.dat
--rw-r--r--   0 runner    (1001) docker     (127)  1000100 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/data/Tn2n_matrix_ENDFLAW6.dat
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/data/VerbinskiLproton.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/data/nDnT_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/data/tot_D_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/data/tot_T_xsec.dat
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)    14091 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/spectral_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/time_of_flight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-02 10:05:58.000000 NeSST-1.0.0/src/NeSST/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:02.211508 NeSST-1.0.0/src/NeSST.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-02 10:06:02.000000 NeSST-1.0.0/src/NeSST.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-02 10:06:02.000000 NeSST-1.0.0/src/NeSST.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:06:02.000000 NeSST-1.0.0/src/NeSST.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 10:06:02.000000 NeSST-1.0.0/src/NeSST.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 10:06:02.000000 NeSST-1.0.0/src/NeSST.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:06:02.211508 NeSST-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-02 10:05:58.000000 NeSST-1.0.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-02 10:05:58.000000 NeSST-1.0.0/tests/test_time_of_flight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-02 10:05:58.000000 NeSST-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:52.953478 nesst-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 10:29:48.000000 nesst-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-19 10:29:52.953478 nesst-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-19 10:29:48.000000 nesst-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 10:29:48.000000 nesst-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:29:52.953478 nesst-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:52.937478 nesst-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:52.937478 nesst-1.1.0/src/NeSST/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18313 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/cross_sections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:52.941478 nesst-1.1.0/src/NeSST/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/Be9.json
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/C12.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:52.949478 nesst-1.1.0/src/NeSST/data/ENDF/
+-rw-r--r--   0 runner    (1001) docker     (127)   671232 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/ENDF/n-001_H_001.endf
+-rw-r--r--   0 runner    (1001) docker     (127)  2510919 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/ENDF/n-001_H_002.cendl
+-rw-r--r--   0 runner    (1001) docker     (127)   130340 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/ENDF/n-001_H_002.endf
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/ENDF/n-001_H_003.brond
+-rw-r--r--   0 runner    (1001) docker     (127)    75924 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/ENDF/n-001_H_003.endf
+-rw-r--r--   0 runner    (1001) docker     (127)  1303400 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/ENDF/n-004_Be_009.endf
+-rw-r--r--   0 runner    (1001) docker     (127)  3805168 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/ENDF/n-006_C_012.endf
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/H1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/H2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/H3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/TT_reac_ENDF.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/TT_reac_McNally.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   410500 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/TT_spec_temprange.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/VerbinskiLproton.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/endf_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12668 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/spectral_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/time_of_flight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-19 10:29:48.000000 nesst-1.1.0/src/NeSST/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:52.953478 nesst-1.1.0/src/NeSST.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-19 10:29:52.000000 nesst-1.1.0/src/NeSST.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 10:29:52.000000 nesst-1.1.0/src/NeSST.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:29:52.000000 nesst-1.1.0/src/NeSST.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 10:29:52.000000 nesst-1.1.0/src/NeSST.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 10:29:52.000000 nesst-1.1.0/src/NeSST.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:29:52.953478 nesst-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-19 10:29:48.000000 nesst-1.1.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-19 10:29:48.000000 nesst-1.1.0/tests/test_endf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 10:29:48.000000 nesst-1.1.0/tests/test_time_of_flight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-19 10:29:48.000000 nesst-1.1.0/tests/test_utils.py
```

### Comparing `NeSST-1.0.0/LICENSE` & `nesst-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/PKG-INFO` & `nesst-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: NeSST
-Version: 1.0.0
-Summary: Neutron Scattered Spectra Tool, ICF primary and scattered neutron spectroscopy analysis code
-Author: Aidan Crilly <ac116@ic.ac.uk>
-Project-URL: Homepage, https://github.com/aidancrilly/NeSST
-Project-URL: Bug Tracker, https://github.com/aidancrilly/NeSST/issues
-Keywords: python,reactor,fusion,power,sankey
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: jupyter; extra == "test"
-Requires-Dist: matplotlib; extra == "test"
-
 [![Continuous Integration](https://github.com/aidancrilly/NeSST/actions/workflows/ci.yml/badge.svg)](https://github.com/aidancrilly/NeSST/actions/workflows/ci.yml)
 
 # NeSST
 Neutron Scattered Spectra Tool: A python tool for ICF neutron spectroscopy in the single scatter regime
 
 ```
 import NeSST as nst
@@ -59,33 +36,26 @@
 cd NeSST
 pip install -e .
 ```
 
 ## Current model specifications:
 - Primary spectrum models for DT, DD and TT
 - Elastic and inelastic (n,2n) processes for D and T
+- ENDF file interface using [ENDF-python](https://github.com/paulromano/endf-python)
 - Relativistic corrections to elastic scattering kernels
 - Scattering of all primary neutron sources
 - Inclusion of areal density asymmetry effects and variable fuel fractions
 - Backscatter edge shape effects from scattering ion kinematics
-- Preliminary scattering in H, 12C, 9Be support
 - Synthetic neutron time-of-flight tools
 
 ## Future model developments:
 - Fitting models with ion kinematic approximations
 - Pre-computed table support for backscatter edge matrix
 - Knock-on ion spectra
 
-## DT cross section and reactivity data:
-ENDF: nT elastic, nD elastic, nH elastic, T(n,2n), TT primary
-
-CENDL: D(n,2n), n12C elastic and 4.4 MeV inelastic
-
-Bosch-Hale: DT primary, DD primary
-
 ## Publications:
 The models used in this code are described in the following publications:
 
 The effect of areal density asymmetries on scattered neutron spectra in ICF implosions, PoP, 2021
 
 Neutron backscatter edge: A measure of the hydrodynamic properties of the dense DT fuel at stagnation in ICF experiments, PoP, 2020
```

### Comparing `NeSST-1.0.0/README.md` & `nesst-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: NeSST
+Version: 1.1.0
+Summary: Neutron Scattered Spectra Tool, ICF primary and scattered neutron spectroscopy analysis code
+Author: Aidan Crilly <ac116@ic.ac.uk>
+Project-URL: Homepage, https://github.com/aidancrilly/NeSST
+Project-URL: Bug Tracker, https://github.com/aidancrilly/NeSST/issues
+Keywords: python,reactor,fusion,power,sankey
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: endf
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: jupyter; extra == "test"
+Requires-Dist: matplotlib; extra == "test"
+
 [![Continuous Integration](https://github.com/aidancrilly/NeSST/actions/workflows/ci.yml/badge.svg)](https://github.com/aidancrilly/NeSST/actions/workflows/ci.yml)
 
 # NeSST
 Neutron Scattered Spectra Tool: A python tool for ICF neutron spectroscopy in the single scatter regime
 
 ```
 import NeSST as nst
@@ -36,33 +60,26 @@
 cd NeSST
 pip install -e .
 ```
 
 ## Current model specifications:
 - Primary spectrum models for DT, DD and TT
 - Elastic and inelastic (n,2n) processes for D and T
+- ENDF file interface using [ENDF-python](https://github.com/paulromano/endf-python)
 - Relativistic corrections to elastic scattering kernels
 - Scattering of all primary neutron sources
 - Inclusion of areal density asymmetry effects and variable fuel fractions
 - Backscatter edge shape effects from scattering ion kinematics
-- Preliminary scattering in H, 12C, 9Be support
 - Synthetic neutron time-of-flight tools
 
 ## Future model developments:
 - Fitting models with ion kinematic approximations
 - Pre-computed table support for backscatter edge matrix
 - Knock-on ion spectra
 
-## DT cross section and reactivity data:
-ENDF: nT elastic, nD elastic, nH elastic, T(n,2n), TT primary
-
-CENDL: D(n,2n), n12C elastic and 4.4 MeV inelastic
-
-Bosch-Hale: DT primary, DD primary
-
 ## Publications:
 The models used in this code are described in the following publications:
 
 The effect of areal density asymmetries on scattered neutron spectra in ICF implosions, PoP, 2021
 
 Neutron backscatter edge: A measure of the hydrodynamic properties of the dense DT fuel at stagnation in ICF experiments, PoP, 2020
```

### Comparing `NeSST-1.0.0/pyproject.toml` & `nesst-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NeSST"
-version = "1.0.0"
+version = "1.1.0"
 description = "Neutron Scattered Spectra Tool, ICF primary and scattered neutron spectroscopy analysis code"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research"
@@ -17,25 +17,27 @@
   { name="Aidan Crilly <ac116@ic.ac.uk>" },
 ]
 requires-python = ">=3.0"
 keywords = ["python", "reactor", "fusion", "power", "sankey"]
 dependencies = [
     "numpy",
     "scipy",
-    "matplotlib"
+    "matplotlib",
+    "endf"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/aidancrilly/NeSST"
 "Bug Tracker" = "https://github.com/aidancrilly/NeSST/issues"
 
 
 [project.optional-dependencies]
 test = [
     "pytest", "jupyter", "matplotlib"
 ]
 
 [tool.setuptools.package-data]
-"NeSST.data" = ["*.dat", "*.txt","*.csv"]
+"NeSST.data" = ["*.dat", "*.txt","*.csv","*.json"]
+"NeSST.data.ENDF" = ["*.endf", "*.cendl","*.brond"]
 
 [tool.setuptools]
 package-dir = {"" = "src"}
```

### Comparing `NeSST-1.0.0/src/NeSST/collisions.py` & `nesst-1.1.0/src/NeSST/collisions.py`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/src/NeSST/constants.py` & `nesst-1.1.0/src/NeSST/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ''' Contains some physical constants used throughout the analysis '''
 import scipy.constants as sc
 import numpy as np
+import numpy.typing as npt
+
 # Scipy constants uses CODATA2018 database
 
 # Need to swap from MeV to eV
 amu  = sc.value('atomic mass constant energy equivalent in MeV')*1e6
 c    = sc.c
 Me   = sc.value('electron mass energy equivalent in MeV')*1e6
 Mn   = sc.value('neutron mass energy equivalent in MeV')*1e6
@@ -23,8 +25,9 @@
 sigmabarn = 1e-28 # barns to m^2
 E0_DT = ((Md+Mt)**2+Mn**2-MHe4**2)/(2*(Md+Mt))-Mn
 E0_DD = ((Md+Md)**2+Mn**2-MHe3**2)/(2*(Md+Md))-Mn
 
 # Directories
 import os
 package_directory = os.path.dirname(os.path.abspath(__file__))
-data_dir = os.path.join(package_directory,"./data/")
+data_dir = os.path.join(package_directory,"./data/")
+ENDF_dir = os.path.join(data_dir,"./ENDF/")
```

### Comparing `NeSST-1.0.0/src/NeSST/core.py` & `nesst-1.1.0/src/NeSST/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,18 +439,18 @@
         where x e [-1,1] and f(x) e [0,inf] and int f(x) dx = 1
 
     Returns:
         numpy.array: the total scattered spectrum
     
     """
     mat.calc_dNdEs(I_E,rhoL_func)
-    total = mat.elastic_dNdE
+    total = mat.elastic_dNdE.copy()
     if(mat.l_n2n):
         total += mat.n2n_dNdE
-    if(mat.inelastic):
+    if(mat.l_inelastic):
         total += mat.inelastic_dNdE
     return total
 
 ###############################
 # Full model fitting function #
 ###############################
```

### Comparing `NeSST-1.0.0/src/NeSST/data/TT_reac_ENDF.dat` & `nesst-1.1.0/src/NeSST/data/TT_reac_ENDF.dat`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/src/NeSST/data/TT_reac_McNally.dat` & `nesst-1.1.0/src/NeSST/data/TT_reac_McNally.dat`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/src/NeSST/data/TT_spec_temprange.txt` & `nesst-1.1.0/src/NeSST/data/TT_spec_temprange.txt`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/src/NeSST/fitting.py` & `nesst-1.1.0/src/NeSST/fitting.py`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/src/NeSST/spectral_model.py` & `nesst-1.1.0/src/NeSST/spectral_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Backend of spectral model
 
 import numpy as np
 
 from NeSST.constants import *
 from NeSST.utils import *
+from NeSST.endf_interface import retrieve_ENDF_data
 import NeSST.collisions as col
 import NeSST.cross_sections as xs
 
 ##################
 # Material class #
 ##################
 
@@ -21,179 +22,167 @@
 def unity(x):
     return np.ones_like(x)
 
 class material_data:
 
     def __init__(self,label):
         self.label = label
-        self.l_n2n = False
-        self.inelastic = False
         if(self.label == 'H'):
-            self.A = Mp/Mn
-            elastic_xsec_file  = data_dir + "ENDF_H1(n,elastic)_xsec.dat"
-            elastic_dxsec_file = data_dir + "ENDF_H1(n,elastic)_dx.dat"
-
-            tot_xsec_file      = data_dir + "ENDF_H1(n,elastic)_xsec.dat"
+            self.json = 'H1.json'
         elif(self.label == 'D'):
-            self.A = Md/Mn
-            elastic_xsec_file  = data_dir + "ENDF_H2(n,elastic)_xsec.dat"
-            elastic_dxsec_file = data_dir + "ENDF_H2(n,elastic)_dx.dat"
-
-            self.l_n2n         = True
-            # n2n_type = 0 is ENDF LAW=6, n2n_type = 1 is tabulated double differential cross sections
-            n2n_type           = 1
-            n2n_xsec_file      = data_dir + "CENDL_d(n,2n)_xsec.dat"
-            n2n_dxsec_file     = data_dir + "CENDL_d(n,2n)_ddx.dat"
-            n2n_params         = None
-
-            tot_xsec_file      = data_dir + "ENDF_nH2_totxsec.dat"
+            self.json = 'H2.json'
         elif(self.label == 'T'):
-            self.A = Mt/Mn
-            elastic_xsec_file  = data_dir + "ENDF_H3(n,elastic)_xsec.dat"
-            elastic_dxsec_file = data_dir + "ENDF_H3(n,elastic)_dx.dat"
-
-            self.l_n2n         = True
-            # n2n_type = 0 is ENDF LAW=6, n2n_type = 1 is tabulated double differential cross sections
-            n2n_type           = 0
-            n2n_xsec_file      = data_dir + "ENDF_t(n,2n)_xsec.dat"
-            n2n_dxsec_file     = None
-            n2n_params         = [1.0e0,1.0e0,2.990140e0,1.0e0,3.996800e0,-6.25756e6]
-
-            tot_xsec_file      = data_dir + "ENDF_nH3_totxsec.dat"
+            self.json = 'H3.json'
         elif(self.label == '12C'):
-            self.A = MC/Mn
-            elastic_xsec_file  = data_dir + "CENDL_C12(n,elastic)_xsec.dat"
-            elastic_dxsec_file = data_dir + "CENDL_C12(n,elastic)_dx.dat"
-
-            self.inelastic     = True
-            self.inelastic_Q   = -4.43890e6 # eV
-            inelastic_xsec_file  = data_dir + "CENDL_C12(n,n1)_xsec.dat"
-            inelastic_dxsec_file = data_dir + "CENDL_C12(n,n1)_dx.dat"
-
-            tot_xsec_file      = data_dir + "CENDL_C12_totxsec.dat"
+            self.json = 'C12.json'
         elif(self.label == '9Be'):
-            self.A = MBe/Mn
-            elastic_xsec_file  = data_dir + "ENDF_Be9(n,elastic)_xsec.dat"
-            elastic_dxsec_file = data_dir + "ENDF_Be9(n,elastic)_dx.dat"
-
-            self.l_n2n         = True
-            # n2n_type = 0 is ENDF LAW=6, n2n_type = 1 is tabulated double differential cross sections
-            n2n_type           = 1
-            n2n_xsec_file      = data_dir + "ENDF_Be9(n,2n)_xsec.dat"
-            n2n_dxsec_file     = data_dir + "ENDF_Be9(n,2n)_ddx.dat"
-            n2n_params         = None
-
-            tot_xsec_file      = data_dir + "ENDF_nBe9_totxsec.dat"
+            self.json = 'Be9.json'
         else:
             print("Material label "+self.label+" not recognised")
 
-        elastic_xsec_data = self.read_ENDF_xsec_file(elastic_xsec_file)
-        self.sigma = interpolate_1d(elastic_xsec_data[:,0],elastic_xsec_data[:,1],method='linear',bounds_error=False,fill_value=0.0)
+        ENDF_data = retrieve_ENDF_data(self.json)
 
-        dx_data = np.loadtxt(elastic_dxsec_file,skiprows = 6)
-        self.dx_spline = [unity]
-        for i in range(1,dx_data.shape[1]):
-            self.dx_spline.append(interpolate_1d(dx_data[:,0],dx_data[:,i],method='linear',bounds_error=False,fill_value=0.0))
+        self.A = ENDF_data['A']
 
-        tot_xsec_data = self.read_ENDF_xsec_file(tot_xsec_file)
-        self.sigma_tot = interpolate_1d(tot_xsec_data[:,0],tot_xsec_data[:,1],method='linear',bounds_error=False,fill_value=0.0)
+        if(ENDF_data['interactions'].total):
+            self.sigma_tot = interpolate_1d(ENDF_data['total_xsec']['E'],ENDF_data['total_xsec']['sig'],method='linear',bounds_error=False,fill_value=0.0)
 
-        if(self.l_n2n):
-            if(n2n_type == 0):
-                self.n2n_ddx = xs.doubledifferentialcrosssection_LAW6(n2n_xsec_file,*n2n_params)
-            elif(n2n_type == 1):
-                self.n2n_ddx = xs.doubledifferentialcrosssection_data(n2n_xsec_file,n2n_dxsec_file,True)
-
-        if(self.inelastic):
-            inelastic_xsec_data = self.read_ENDF_xsec_file(inelastic_xsec_file)
-            self.isigma = interpolate_1d(inelastic_xsec_data[:,0],inelastic_xsec_data[:,1],method='linear',bounds_error=False,fill_value=0.0)
-            idx_data = np.loadtxt(inelastic_dxsec_file,skiprows = 6)
-            self.idx_spline = [unity]
-            for i in range(1,idx_data.shape[1]):
-                self.idx_spline.append(interpolate_1d(idx_data[:,0],idx_data[:,i],method='linear',bounds_error=False,fill_value=0.0))
+        if(ENDF_data['interactions'].elastic):
+            self.sigma = interpolate_1d(ENDF_data['elastic_xsec']['E'],ENDF_data['elastic_xsec']['sig'],method='linear',bounds_error=False,fill_value=0.0)
+
+            self.elastic_legendre = ENDF_data['elastic_dxsec']['legendre']
+            if(self.elastic_legendre):
+                self.legendre_dx_spline = [unity]
+                for i in range(ENDF_data['elastic_dxsec']['N_l']):
+                    self.legendre_dx_spline.append(interpolate_1d(ENDF_data['elastic_dxsec']['E'],ENDF_data['elastic_dxsec']['a_l'][:,i],method='linear',bounds_error=False,fill_value=0.0))
+            else:
+                self.elastic_SDX_table = ENDF_data['elastic_dxsec']['SDX']
+
+        self.l_n2n = ENDF_data['interactions'].n2n
+        if(ENDF_data['interactions'].n2n):
+            if(ENDF_data['n2n_dxsec']['LAW'] == 6):
+                self.n2n_ddx = xs.doubledifferentialcrosssection_LAW6(ENDF_data['n2n_xsec'],ENDF_data['n2n_dxsec'])
+            elif(ENDF_data['n2n_dxsec']['LAW'] == 7):
+                self.n2n_ddx = xs.doubledifferentialcrosssection_data(ENDF_data['n2n_xsec'],ENDF_data['n2n_dxsec'])
+
+        self.l_inelastic = ENDF_data['interactions'].inelastic
+        if(ENDF_data['interactions'].inelastic):
+            self.n_inelastic = ENDF_data['n_inelastic']
+
+            self.isigma = []
+            self.inelasticQ = []
+            self.inelastic_legendre = []
+            self.legendre_idx_spline = []
+            self.inelastic_SDX_table = []
+
+            for i_inelastic in range(self.n_inelastic):
+                xsec_table = ENDF_data[f'inelastic_xsec_n{i_inelastic+1}']
+                self.isigma.append(interpolate_1d(xsec_table['E'],xsec_table['sig'],method='linear',bounds_error=False,fill_value=0.0))
+
+                dxsec_table = ENDF_data[f'inelastic_dxsec_n{i_inelastic+1}']
+                self.inelasticQ.append(dxsec_table['Q'])
+
+                self.inelastic_legendre.append(dxsec_table['legendre'])
+                if(dxsec_table['legendre']):
+                    idx_spline = [unity]
+                    for i in range(dxsec_table['N_l']):
+                        idx_spline.append(interpolate_1d(dxsec_table['E'],dxsec_table['a_l'][:,i],method='linear',bounds_error=False,fill_value=0.0))
+                    self.legendre_idx_spline.append(idx_spline)
+                    self.inelastic_SDX_table.append(None)
+                else:
+                    self.legendre_idx_spline.append(None)
+                    self.inelastic_SDX_table.append(dxsec_table['SDX'])
 
         self.Ein  = None       
         self.Eout = None
         self.vvec = None
-        
-    def read_ENDF_xsec_file(self,xsec_file):
-        with open(xsec_file,"r") as f:
-            file = f.read()
-            # Read number of points
-            NEin_xsec = int(file.split()[0])
-            elastic_xsec_data = np.zeros((NEin_xsec,2))
-            data = "".join(file.split("\n")[5:]).split()
-            E = data[::2]
-            x = data[1::2]
-            for i in range(NEin_xsec):
-                elastic_xsec_data[i,0] = xs.ENDF_format(E[i])
-                elastic_xsec_data[i,1] = xs.ENDF_format(x[i])
-        return elastic_xsec_data
 
     ############################################
     # Stationary ion scattered spectral shapes #
     ############################################
 
     def init_energy_grids(self,Eout,Ein):
         self.Eout = Eout
         self.Ein  = Ein
 
     def init_station_scatter_matrices(self,Nm=100):
         self.init_station_elastic_scatter()
         if(self.l_n2n):
             self.init_n2n_ddxs(Nm)
-        if(self.inelastic):
+        if(self.l_inelastic):
             self.init_station_inelastic_scatter()
 
     # Elastic scatter matrix
     def init_station_elastic_scatter(self):
         Ei,Eo  = np.meshgrid(self.Ein,self.Eout)
         muc    = col.muc(self.A,Ei,Eo,1.0,-1.0,0.0)
         sigma  = self.sigma(self.Ein)
-        Tlcoeff,Nl     = xs.interp_Tlcoeff(self.dx_spline,self.Ein)
-        Tlcoeff_interp = 0.5*(2*np.arange(0,Nl)+1)*Tlcoeff
         self.elastic_mu0 = col.mu_out(self.A,Ei,Eo,0.0)
-        dsdO = xs.diffxsec_legendre_eval(sigma,muc,Tlcoeff_interp)
+        if(self.elastic_legendre):
+            Tlcoeff,Nl     = xs.interp_Tlcoeff(self.legendre_dx_spline,self.Ein)
+            Tlcoeff_interp = 0.5*(2*np.arange(0,Nl)+1)*Tlcoeff
+            dsdO = xs.diffxsec_legendre_eval(sigma,muc,Tlcoeff_interp)
+        else:
+            dsdO = xs.diffxsec_table_eval(sigma,muc,Ei,self.elastic_SDX_table)
         jacob = col.g(self.A,Ei,Eo,1.0,-1.0,0.0)
         self.elastic_dNdEdmu = jacob*dsdO
 
     # Inelastic scatter matrix
     # Currently uses classical kinematics
     def init_station_inelastic_scatter(self):
         Ei,Eo  = np.meshgrid(self.Ein,self.Eout)
-        kin_a  = np.sqrt((self.A/(self.A+1))**2*(1.0+(self.A+1)/self.A*self.inelastic_Q/Ei))
-        kin_b  = 1.0/(self.A+1)
-        muc    = ((Eo/Ei)-kin_a**2-kin_b**2)/(2*kin_a*kin_b)
-        sigma  = self.isigma(self.Ein)
-        Tlcoeff,Nl     = xs.interp_Tlcoeff(self.idx_spline,self.Ein)
-        Tlcoeff_interp = 0.5*(2*np.arange(0,Nl)+1)*Tlcoeff
-        self.inelastic_mu0 = (np.sqrt(Eo/Ei)-(kin_a**2-kin_b**2)*np.sqrt(Ei/Eo))/(2*kin_b)
-        dsdO = xs.diffxsec_legendre_eval(sigma,muc,Tlcoeff_interp)
-        jacob = 2.0/((kin_a+kin_b)**2-(kin_a-kin_b)**2)/Ei
-        self.inelastic_dNdEdmu = jacob*dsdO
+        self.inelastic_mu0 = []
+        self.inelastic_dNdEdmu = []
+        for i_inelastic in range(self.n_inelastic):
+            kin_a2 = (self.A/(self.A+1))**2*(1.0+(self.A+1)/self.A*self.inelasticQ[i_inelastic]/Ei)
+            kin_a2_safe = kin_a2.copy()
+            kin_a2_safe[kin_a2_safe < 0.0] = 1.0
+            kin_a  = np.sqrt(kin_a2_safe)
+            kin_b  = 1.0/(self.A+1)
+            muc    = ((Eo/Ei)-kin_a**2-kin_b**2)/(2*kin_a*kin_b)
+            sigma  = self.isigma[i_inelastic](self.Ein)
+            inelastic_mu0 = (np.sqrt(Eo/Ei)-(kin_a**2-kin_b**2)*np.sqrt(Ei/Eo))/(2*kin_b)
+            inelastic_mu0[kin_a2 < 0.0] = 0.0
+            self.inelastic_mu0.append(inelastic_mu0)
+
+            if(self.inelastic_legendre[i_inelastic]):
+                Tlcoeff,Nl     = xs.interp_Tlcoeff(self.legendre_idx_spline[i_inelastic],self.Ein)
+                Tlcoeff_interp = 0.5*(2*np.arange(0,Nl)+1)*Tlcoeff
+                dsdO = xs.diffxsec_legendre_eval(sigma,muc,Tlcoeff_interp)
+            else:
+                dsdO = xs.diffxsec_table_eval(sigma,muc,Ei,self.inelastic_SDX_table[i_inelastic])
+
+            jacob = 2.0/((kin_a+kin_b)**2-(kin_a-kin_b)**2)/Ei
+            inelastic_dNdEdmu = jacob*dsdO
+            
+            inelastic_dNdEdmu[kin_a2 < 0.0] = 0.0
+
+            self.inelastic_dNdEdmu.append(inelastic_dNdEdmu)
 
     def init_n2n_ddxs(self,Nm=100):
         self.n2n_mu = np.linspace(-1.0,1.0,Nm)
         self.n2n_ddx.regular_grid(self.Ein,self.n2n_mu,self.Eout)
 
     def calc_dNdEs(self,I_E,rhoL_func):
         self.calc_station_elastic_dNdE(I_E,rhoL_func)
         if(self.l_n2n):
             self.calc_n2n_dNdE(I_E,rhoL_func)
-        if(self.inelastic):
+        if(self.l_inelastic):
             self.calc_station_inelastic_dNdE(I_E,rhoL_func)
 
     # Spectrum produced by scattering of incoming isotropic neutron source I_E with normalised areal density asymmetry rhoR_asym_func
     def calc_station_elastic_dNdE(self,I_E,rhoL_func):
         rhoL_asym = rhoL_func(self.elastic_mu0)
         self.elastic_dNdE = np.trapz(self.elastic_dNdEdmu*rhoL_asym*I_E[None,:],self.Ein,axis=1)
 
     def calc_station_inelastic_dNdE(self,I_E,rhoL_func):
-        rhoL_asym = rhoL_func(self.elastic_mu0)
-        self.inelastic_dNdE = np.trapz(self.inelastic_dNdEdmu*rhoL_asym*I_E[None,:],self.Ein,axis=1)
+        self.inelastic_dNdE = np.zeros(self.Eout.shape[0])
+        for i_inelastic in range(self.n_inelastic):
+            rhoL_asym = rhoL_func(self.inelastic_mu0[i_inelastic])
+            self.inelastic_dNdE += np.trapz(self.inelastic_dNdEdmu[i_inelastic]*rhoL_asym*I_E[None,:],self.Ein,axis=1)
 
     def calc_n2n_dNdE(self,I_E,rhoL_func):
         rhoL_asym = rhoL_func(self.n2n_mu)
         grid_dNdE = np.trapz(self.n2n_ddx.rgrid*rhoL_asym[None,:,None],self.n2n_mu,axis=1)
         self.n2n_dNdE = np.trapz(I_E[:,None]*grid_dNdE,self.Ein,axis=0)
 
     def rhoR_2_A1s(self,rhoR):
@@ -203,15 +192,15 @@
 
     # # Spectrum produced by scattering of incoming neutron source with anisotropic birth spectrum
     # def elastic_scatter_aniso(self,Eout,Ein,mean_iso,mean_aniso,var_iso,b_spec,rhoR_asym_func):
     #     Ei,Eo  = np.meshgrid(Ein,Eout)
     #     muc    = col.muc(self.A,Ei,Eo,1.0,-1.0,0.0)
     #     sigma  = sigma_nT(Ein)
     #     E_vec  = Ein
-    #     Tlcoeff,Nl     = interp_Tlcoeff(self.dx_spline,E_vec)
+    #     Tlcoeff,Nl     = interp_Tlcoeff(self.legendre_dx_spline,E_vec)
     #     Tlcoeff_interp = 0.5*(2*np.arange(0,Nl)+1)*Tlcoeff
     #     mu0 = col.mu_out(self.A,Ei,Eo,0.0)
     #     rhoR_asym = rhoR_asym_func(mu0)
     #     prim_mean = mean_iso+mean_aniso*mu0
     #     I_E_aniso = b_spec(Ei,prim_mean,var_iso)
     #     dsdO = diffxsec_legendre_eval(sigma,muc,Tlcoeff_interp)
     #     jacob = col.g(self.A,Ei,Eo,1.0,-1.0,0.0)
@@ -256,16 +245,16 @@
         return interp(E)
 
 
 # Default load
 mat_H = material_data('H')
 mat_D = material_data('D')
 mat_T = material_data('T')
-mat_12C = material_data('12C')
 mat_9Be = material_data('9Be')
+mat_12C = material_data('12C')
 
 available_materials_dict = {"H" : mat_H, "D" : mat_D, "T" : mat_T, "12C" : mat_12C, "9Be" : mat_9Be}
 
 # Load in TT spectrum
 # Based on Appelbe, stationary emitter, temperature range between 1 and 10 keV
 # https://www.sciencedirect.com/science/article/pii/S1574181816300295
 # N.B. requires some unit conversion to uniform eV
@@ -299,22 +288,8 @@
     C1 = 3.5741e-22
     xi = 6.2696*Ti_kev**(-0.333333333)
     eta = 1-np.polyval([5.8577e-3,0.0e0],Ti_kev)/np.polyval([-0.002964e-3,7.6822e-3,1.0e0],Ti_kev)
     return C1*eta**(-0.833333333)*xi**2*np.exp(-3*eta**(0.333333333)*xi)
 
 def reac_TT(Ti):
     Ti_kev = Ti/1e3
-    return TT_reac_spline(Ti_kev)
-
-##############################################################################
-# Deprecated n2n matrix representation
-E1_n2n = np.linspace(13.0e6,15.0e6,100)
-E2_n2n = np.linspace(1.0e6,13.0e6,500)
-Dn2n_matrix = np.loadtxt(data_dir + "Dn2n_matrix.dat")
-Tn2n_matrix_1 = np.loadtxt(data_dir + "Tn2n_matrix_ENDFLAW6.dat")
-Tn2n_matrix_2 = np.loadtxt(data_dir + "Tn2n_matrix_CENDL_transform.dat")
-# 2D interpolation functions
-Dn2n_2dinterp = interpolate_2d(E1_n2n,E2_n2n,Dn2n_matrix,method='linear',bounds_error=False,fill_value=0.0)
-Tn2n_1_2dinterp = interpolate_2d(E1_n2n,E2_n2n,Tn2n_matrix_1,method='linear',bounds_error=False,fill_value=0.0)
-Tn2n_2_2dinterp = interpolate_2d(E1_n2n,E2_n2n,Tn2n_matrix_2,method='linear',bounds_error=False,fill_value=0.0)
-# Deprecated n2n matrix representation
-############################################################################
+    return TT_reac_spline(Ti_kev)
```

### Comparing `NeSST-1.0.0/src/NeSST/time_of_flight.py` & `nesst-1.1.0/src/NeSST/time_of_flight.py`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/src/NeSST/utils.py` & `nesst-1.1.0/src/NeSST/utils.py`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/src/NeSST.egg-info/PKG-INFO` & `nesst-1.1.0/src/NeSST.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeSST
-Version: 1.0.0
+Version: 1.1.0
 Summary: Neutron Scattered Spectra Tool, ICF primary and scattered neutron spectroscopy analysis code
 Author: Aidan Crilly <ac116@ic.ac.uk>
 Project-URL: Homepage, https://github.com/aidancrilly/NeSST
 Project-URL: Bug Tracker, https://github.com/aidancrilly/NeSST/issues
 Keywords: python,reactor,fusion,power,sankey
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
+Requires-Dist: endf
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: jupyter; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 
 [![Continuous Integration](https://github.com/aidancrilly/NeSST/actions/workflows/ci.yml/badge.svg)](https://github.com/aidancrilly/NeSST/actions/workflows/ci.yml)
 
@@ -59,33 +60,26 @@
 cd NeSST
 pip install -e .
 ```
 
 ## Current model specifications:
 - Primary spectrum models for DT, DD and TT
 - Elastic and inelastic (n,2n) processes for D and T
+- ENDF file interface using [ENDF-python](https://github.com/paulromano/endf-python)
 - Relativistic corrections to elastic scattering kernels
 - Scattering of all primary neutron sources
 - Inclusion of areal density asymmetry effects and variable fuel fractions
 - Backscatter edge shape effects from scattering ion kinematics
-- Preliminary scattering in H, 12C, 9Be support
 - Synthetic neutron time-of-flight tools
 
 ## Future model developments:
 - Fitting models with ion kinematic approximations
 - Pre-computed table support for backscatter edge matrix
 - Knock-on ion spectra
 
-## DT cross section and reactivity data:
-ENDF: nT elastic, nD elastic, nH elastic, T(n,2n), TT primary
-
-CENDL: D(n,2n), n12C elastic and 4.4 MeV inelastic
-
-Bosch-Hale: DT primary, DD primary
-
 ## Publications:
 The models used in this code are described in the following publications:
 
 The effect of areal density asymmetries on scattered neutron spectra in ICF implosions, PoP, 2021
 
 Neutron backscatter edge: A measure of the hydrodynamic properties of the dense DT fuel at stagnation in ICF experiments, PoP, 2020
```

### Comparing `NeSST-1.0.0/tests/test_core.py` & `nesst-1.1.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/tests/test_time_of_flight.py` & `nesst-1.1.0/tests/test_time_of_flight.py`

 * *Files identical despite different names*

### Comparing `NeSST-1.0.0/tests/test_utils.py` & `nesst-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

