# Comparing `tmp/pyiron_lammps-0.2.8.tar.gz` & `tmp/pyiron_lammps-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_lammps-0.2.8.tar", last modified: Mon Nov 27 14:34:15 2023, max compression
+gzip compressed data, was "pyiron_lammps-0.2.9.tar", last modified: Mon Nov 27 14:54:15 2023, max compression
```

## Comparing `pyiron_lammps-0.2.8.tar` & `pyiron_lammps-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:34:15.819974 pyiron_lammps-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-11-27 14:34:15.819974 pyiron_lammps-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:34:15.815974 pyiron_lammps-0.2.8/pyiron_lammps/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/pyiron_lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-27 14:34:15.819974 pyiron_lammps-0.2.8/pyiron_lammps/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/pyiron_lammps/calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/pyiron_lammps/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/pyiron_lammps/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:34:15.819974 pyiron_lammps-0.2.8/pyiron_lammps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-11-27 14:34:15.000000 pyiron_lammps-0.2.8/pyiron_lammps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-11-27 14:34:15.000000 pyiron_lammps-0.2.8/pyiron_lammps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:34:15.000000 pyiron_lammps-0.2.8/pyiron_lammps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-27 14:34:15.000000 pyiron_lammps-0.2.8/pyiron_lammps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-27 14:34:15.000000 pyiron_lammps-0.2.8/pyiron_lammps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2023-11-27 14:34:14.000000 pyiron_lammps-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 14:34:15.819974 pyiron_lammps-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:34:15.819974 pyiron_lammps-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/tests/test_elastic_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/tests/test_elastic_parallel_single_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/tests/test_elastic_parallel_two_cores.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/tests/test_evcurve_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/tests/test_evcurve_parallel_single_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-11-27 14:33:53.000000 pyiron_lammps-0.2.8/tests/test_evcurve_parallel_two_cores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:54:15.141373 pyiron_lammps-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-11-27 14:54:15.141373 pyiron_lammps-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:54:15.141373 pyiron_lammps-0.2.9/pyiron_lammps/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/pyiron_lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-27 14:54:15.141373 pyiron_lammps-0.2.9/pyiron_lammps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/pyiron_lammps/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/pyiron_lammps/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/pyiron_lammps/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:54:15.141373 pyiron_lammps-0.2.9/pyiron_lammps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-11-27 14:54:15.000000 pyiron_lammps-0.2.9/pyiron_lammps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-11-27 14:54:15.000000 pyiron_lammps-0.2.9/pyiron_lammps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:54:15.000000 pyiron_lammps-0.2.9/pyiron_lammps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-27 14:54:15.000000 pyiron_lammps-0.2.9/pyiron_lammps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-27 14:54:15.000000 pyiron_lammps-0.2.9/pyiron_lammps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-11-27 14:54:12.000000 pyiron_lammps-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 14:54:15.141373 pyiron_lammps-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:54:15.141373 pyiron_lammps-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/tests/test_elastic_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/tests/test_elastic_parallel_single_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/tests/test_elastic_parallel_two_cores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/tests/test_evcurve_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/tests/test_evcurve_parallel_single_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-11-27 14:52:55.000000 pyiron_lammps-0.2.9/tests/test_evcurve_parallel_two_cores.py
```

### Comparing `pyiron_lammps-0.2.8/LICENSE` & `pyiron_lammps-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/PKG-INFO` & `pyiron_lammps-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_lammps
-Version: 0.2.8
+Version: 0.2.9
 Summary: Vector-oriented LAMMPS interface to rapidly iterate over series of atomistic structures or interatomic potentials.
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, pyiron
         All rights reserved.
```

### Comparing `pyiron_lammps-0.2.8/README.md` & `pyiron_lammps-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/pyiron_lammps/__init__.py` & `pyiron_lammps-0.2.9/pyiron_lammps/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 from . import _version
-
+from atomistics.calculators.lammps import (
+    get_potential_dataframe,
+)
+from pylammpsmpi import LammpsASELibrary
 from pyiron_lammps.calculation import (
     optimize_structure,
     calculate_elastic_constants,
     calculate_energy_volume_curve,
 )
 from pyiron_lammps.parallel import (
     optimize_structure_parallel,
     calculate_elastic_constants_parallel,
     calculate_energy_volume_curve_parallel,
 )
 
-try:
-    from atomistics.calculators.lammps import (
-        get_potential_dataframe,
-    )
-except ImportError:
-    pass
-
 
 def get_lammps_engine(
     working_directory=None,
     cores=1,
     comm=None,
     logger=None,
     log_file=None,
     library=None,
     diable_log_file=True,
 ):
-    from pylammpsmpi import LammpsASELibrary
-
     return LammpsASELibrary(
         working_directory=working_directory,
         cores=cores,
         comm=comm,
         logger=logger,
         log_file=log_file,
         library=library,
```

### Comparing `pyiron_lammps-0.2.8/pyiron_lammps/calculation.py` & `pyiron_lammps-0.2.9/pyiron_lammps/calculation.py`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/pyiron_lammps/decorator.py` & `pyiron_lammps-0.2.9/pyiron_lammps/decorator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from pylammpsmpi import LammpsASELibrary
+
+
 def calculation(funct):
     def funct_return(lmp=None, *args, **kwargs):
         # Create temporary LAMMPS instance if necessary
         if lmp is None:
-            from pylammpsmpi import LammpsASELibrary
-
             close_lmp_after_calculation = True
             lmp = LammpsASELibrary()
         else:
             close_lmp_after_calculation = False
 
         # Run function
         result = funct(lmp=lmp, *args, **kwargs)
```

### Comparing `pyiron_lammps-0.2.8/pyiron_lammps/parallel.py` & `pyiron_lammps-0.2.9/pyiron_lammps/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 from ase.atoms import Atoms
 from pandas import DataFrame, Series
+from pympipool.mpi import PyMPIExecutor
+from pylammpsmpi import LammpsASELibrary
 
 from pyiron_lammps.calculation import (
     optimize_structure,
     calculate_elastic_constants,
     calculate_energy_volume_curve,
 )
 
 
 def _get_lammps_mpi(enable_mpi=True):
-    from pylammpsmpi import LammpsASELibrary
-
     if enable_mpi:
         # To get the right instance of MPI.COMM_SELF it is necessary to import it inside the function.
         from mpi4py import MPI
 
         return LammpsASELibrary(
             working_directory=None,
             cores=1,
@@ -40,16 +40,14 @@
 def _parallel_execution(function, input_parameter_lst, cores=1):
     if cores == 1:
         return [
             function(input_parameter=input_parameter + [False])
             for input_parameter in input_parameter_lst
         ]
     elif cores > 1:
-        from pympipool.mpi import PyMPIExecutor
-
         with PyMPIExecutor(max_workers=cores) as p:
             return list(
                 p.map(
                     function,
                     [
                         input_parameter + [True]
                         for input_parameter in input_parameter_lst
```

### Comparing `pyiron_lammps-0.2.8/pyiron_lammps.egg-info/PKG-INFO` & `pyiron_lammps-0.2.9/pyiron_lammps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-lammps
-Version: 0.2.8
+Version: 0.2.9
 Summary: Vector-oriented LAMMPS interface to rapidly iterate over series of atomistic structures or interatomic potentials.
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, pyiron
         All rights reserved.
```

### Comparing `pyiron_lammps-0.2.8/pyiron_lammps.egg-info/SOURCES.txt` & `pyiron_lammps-0.2.9/pyiron_lammps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/pyproject.toml` & `pyiron_lammps-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["ase", "atomistics", "jinja2", "numpy", "pandas", "setuptools", "versioneer[toml]==0.29"]
+requires = ["ase", "atomistics", "jinja2", "numpy", "pandas", "pylammpsmpi", "pympipool", "setuptools", "versioneer[toml]==0.29"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyiron_lammps"
 description = "Vector-oriented LAMMPS interface to rapidly iterate over series of atomistic structures or interatomic potentials."
 authors = [
     { name = "Jan Janssen", email = "janssen@mpie.de" },
```

### Comparing `pyiron_lammps-0.2.8/tests/test_elastic_base.py` & `pyiron_lammps-0.2.9/tests/test_elastic_base.py`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/tests/test_elastic_parallel_single_core.py` & `pyiron_lammps-0.2.9/tests/test_elastic_parallel_single_core.py`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/tests/test_elastic_parallel_two_cores.py` & `pyiron_lammps-0.2.9/tests/test_elastic_parallel_two_cores.py`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/tests/test_evcurve_base.py` & `pyiron_lammps-0.2.9/tests/test_evcurve_base.py`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/tests/test_evcurve_parallel_single_core.py` & `pyiron_lammps-0.2.9/tests/test_evcurve_parallel_single_core.py`

 * *Files identical despite different names*

### Comparing `pyiron_lammps-0.2.8/tests/test_evcurve_parallel_two_cores.py` & `pyiron_lammps-0.2.9/tests/test_evcurve_parallel_two_cores.py`

 * *Files identical despite different names*

