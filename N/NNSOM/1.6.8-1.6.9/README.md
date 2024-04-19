# Comparing `tmp/nnsom-1.6.8.tar.gz` & `tmp/nnsom-1.6.9.tar.gz`

## Comparing `nnsom-1.6.8.tar` & `nnsom-1.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/__init__.py
--rw-r--r--   0        0        0    77374 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/plots.py
--rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/som.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/som_gpu.py
--rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.6.8/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.8/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.8/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.8/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/__init__.py
+-rw-r--r--   0        0        0    77599 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    19217 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/som.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/som_gpu.py
+-rw-r--r--   0        0        0    20937 2020-02-02 00:00:00.000000 nnsom-1.6.9/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16111 2020-02-02 00:00:00.000000 nnsom-1.6.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.6.9/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.6.9/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.6.9/PKG-INFO
```

### Comparing `nnsom-1.6.8/src/NNSOM/plots.py` & `nnsom-1.6.9/src/NNSOM/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-from .som import SOM
+# Dynamically choose a parent class for your subclass based on whether CuPy is available
+try:
+    import cupy as cp
+    from .som_gpu import SOMGpu
+    base_class = SOMGpu
+except ImportError:
+    from .som import SOM
+    base_class = SOM
+
 from .utils import *
 
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 from matplotlib.widgets import Button
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import matplotlib.colors as mcolors
 
 
-class SOMPlots(SOM):
+class SOMPlots(base_class):
     """
     SOMPlots extends the SOM class by adding visualization capabilities to
     the Self-Organizing Map (SOM). It allows for the graphical representation
     of the SOM's structure, the distribution of input data across its neurons,
     and various other analytical visualizations that aid in the interpretation
     of the SOM's behavior and characteristics.
```

### Comparing `nnsom-1.6.8/src/NNSOM/som.py` & `nnsom-1.6.9/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.8/src/NNSOM/som_gpu.py` & `nnsom-1.6.9/src/NNSOM/som_gpu.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.8/src/NNSOM/utils.py` & `nnsom-1.6.9/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.8/.gitignore` & `nnsom-1.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.6.8/pyproject.toml` & `nnsom-1.6.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.6.8"
+version = "1.6.9"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.6.8/PKG-INFO` & `nnsom-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.6.8
+Version: 1.6.9
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

