# Comparing `tmp/fftvis-0.0.2.tar.gz` & `tmp/fftvis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fftvis-0.0.2.tar", last modified: Wed Apr 17 16:51:05 2024, max compression
+gzip compressed data, was "fftvis-0.0.4.tar", last modified: Thu Apr 18 22:17:21 2024, max compression
```

## Comparing `fftvis-0.0.2.tar` & `fftvis-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.420838 fftvis-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 16:50:59.000000 fftvis-0.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.412838 fftvis-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.412838 fftvis-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 16:50:59.000000 fftvis-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 16:50:59.000000 fftvis-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-17 16:50:59.000000 fftvis-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 16:50:59.000000 fftvis-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 16:51:05.420838 fftvis-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-17 16:50:59.000000 fftvis-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.412838 fftvis-0.0.2/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-17 16:50:59.000000 fftvis-0.0.2/ci/fftvis_tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.416838 fftvis-0.0.2/fftvis/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/beams.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.416838 fftvis-0.0.2/fftvis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/test_compare_matvis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/test_compare_pyuvsim.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-17 16:50:59.000000 fftvis-0.0.2/fftvis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:51:05.416838 fftvis-0.0.2/fftvis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 16:51:05.000000 fftvis-0.0.2/fftvis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-17 16:50:59.000000 fftvis-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-17 16:51:05.420838 fftvis-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-17 16:50:59.000000 fftvis-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.226088 fftvis-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 22:17:11.000000 fftvis-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-18 22:17:11.000000 fftvis-0.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-18 22:17:11.000000 fftvis-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-18 22:17:11.000000 fftvis-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-18 22:17:11.000000 fftvis-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-18 22:17:21.226088 fftvis-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-18 22:17:11.000000 fftvis-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 22:17:11.000000 fftvis-0.0.4/ci/fftvis_tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.222088 fftvis-0.0.4/fftvis/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.226088 fftvis-0.0.4/fftvis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/test_compare_matvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-18 22:17:11.000000 fftvis-0.0.4/fftvis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:21.226088 fftvis-0.0.4/fftvis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 22:17:21.000000 fftvis-0.0.4/fftvis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-18 22:17:11.000000 fftvis-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-18 22:17:21.226088 fftvis-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-18 22:17:11.000000 fftvis-0.0.4/setup.py
```

### Comparing `fftvis-0.0.2/.github/workflows/ci.yml` & `fftvis-0.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/.github/workflows/publish-to-pypi.yml` & `fftvis-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/.gitignore` & `fftvis-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/LICENSE` & `fftvis-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/PKG-INFO` & `fftvis-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fftvis
-Version: 0.0.2
+Version: 0.0.4
 Summary: An FFT-based visibility simulator
 Home-page: https://github.com/tyler-a-cox/fftvis
 Author: Tyler Cox
 Author-email: tyler.a.cox@berkeley.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fftvis-0.0.2/README.md` & `fftvis-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/fftvis/beams.py` & `fftvis-0.0.4/fftvis/beams.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/fftvis/simulate.py` & `fftvis-0.0.4/fftvis/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     fluxes: np.ndarray,
     beam,
     crd_eq: np.ndarray,
     eq2tops: np.ndarray,
     baselines: list[tuple] = None,
     precision: int = 2,
     polarized: bool = False,
-    eps: float = 1e-13,
+    eps: float = None,
     beam_spline_opts: dict = None,
 ):
     """
     Parameters:
     ----------
     ants : dict
         Dictionary of antenna positions in the form {ant_index: np.array([x,y,z])}.
@@ -175,14 +175,17 @@
     if precision == 1:
         real_dtype = np.float32
         complex_dtype = np.complex64
     else:
         real_dtype = np.float64
         complex_dtype = np.complex128
 
+    if eps is None:
+        eps = default_accuracy_dict[precision]
+
     # Get the redundant groups - TODO handle this better
     if not baselines:
         reds = utils.get_pos_reds(ants, include_autos=True)
         baselines = [red[0] for red in reds]
         nbls = len(baselines)
         bl_to_red_map = {red[0]: np.array(red) for red in reds}
         expand_vis = True
@@ -225,14 +228,17 @@
         above_horizon = tz > 0
         tx = tx[above_horizon]
         ty = ty[above_horizon]
 
         # Number of above horizon points
         nsim_sources = above_horizon.sum()
 
+        if nsim_sources == 0:
+            continue
+
         # Form the visibility array
         _vis = np.zeros((nfeeds, nfeeds, nbls, nfreqs), dtype=complex_dtype)
 
         if is_beam_complex:
             _vis_negatives = np.zeros(
                 (nfeeds, nfeeds, nbls, nfreqs), dtype=complex_dtype
             )
```

### Comparing `fftvis-0.0.2/fftvis/tests/__init__.py` & `fftvis-0.0.4/fftvis/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/fftvis/tests/test_compare_matvis.py` & `fftvis-0.0.4/fftvis/tests/test_compare_matvis.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/fftvis/tests/test_compare_pyuvsim.py` & `fftvis-0.0.4/fftvis/tests/test_compare_pyuvsim.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/fftvis/utils.py` & `fftvis-0.0.4/fftvis/utils.py`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/fftvis.egg-info/PKG-INFO` & `fftvis-0.0.4/fftvis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fftvis
-Version: 0.0.2
+Version: 0.0.4
 Summary: An FFT-based visibility simulator
 Home-page: https://github.com/tyler-a-cox/fftvis
 Author: Tyler Cox
 Author-email: tyler.a.cox@berkeley.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `fftvis-0.0.2/setup.cfg` & `fftvis-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fftvis-0.0.2/setup.py` & `fftvis-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This file is used to install the package using pip.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="fftvis",
-    version="0.0.2",
+    version="0.0.4",
     description="An FFT-based visibility simulator",
     author="Tyler Cox",
     author_email="tyler.a.cox@berkeley.edu",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

