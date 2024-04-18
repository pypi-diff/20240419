# Comparing `tmp/polyhedral_gravity-2.1.tar.gz` & `tmp/polyhedral_gravity-3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyhedral_gravity-2.1.tar", last modified: Thu Aug 31 19:04:06 2023, max compression
+gzip compressed data, was "polyhedral_gravity-3.0rc3.tar", last modified: Thu Apr 18 22:17:28 2024, max compression
```

## Comparing `polyhedral_gravity-2.1.tar` & `polyhedral_gravity-3.0rc3.tar`

### file list

```diff
@@ -1,61 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/
--rw-r--r--   0 runner    (1001) docker     (999)     4638 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (999)    36310 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       72 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)      648 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    11063 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.623157 polyhedral_gravity-2.1/cmake/
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/FindSphinx.cmake
--rw-r--r--   0 runner    (1001) docker     (999)      650 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/gtest.cmake
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/pybind11.cmake
--rw-r--r--   0 runner    (1001) docker     (999)      890 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/spdlog.cmake
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/tbb.cmake
--rw-r--r--   0 runner    (1001) docker     (999)     1721 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/tetgen.cmake
--rw-r--r--   0 runner    (1001) docker     (999)      762 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/thrust.cmake
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/xsimd.cmake
--rw-r--r--   0 runner    (1001) docker     (999)      913 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/cmake/yaml.cmake
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.623157 polyhedral_gravity-2.1/polyhedral_gravity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      648 2023-08-31 19:04:06.000000 polyhedral_gravity-2.1/polyhedral_gravity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1733 2023-08-31 19:04:06.000000 polyhedral_gravity-2.1/polyhedral_gravity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 19:04:06.000000 polyhedral_gravity-2.1/polyhedral_gravity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 19:04:06.000000 polyhedral_gravity-2.1/polyhedral_gravity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       19 2023-08-31 19:04:06.000000 polyhedral_gravity-2.1/polyhedral_gravity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     7389 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.623157 polyhedral_gravity-2.1/src/
--rw-r--r--   0 runner    (1001) docker     (999)     2093 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (999)     3823 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.623157 polyhedral_gravity-2.1/src/polyhedralGravity/
--rw-r--r--   0 runner    (1001) docker     (999)      204 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/
--rw-r--r--   0 runner    (1001) docker     (999)    16711 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityEvaluable.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     8269 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityEvaluable.h
--rw-r--r--   0 runner    (1001) docker     (999)     1015 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityModel.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     2035 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityModel.h
--rw-r--r--   0 runner    (1001) docker     (999)    25085 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityModelDetail.cpp
--rw-r--r--   0 runner    (1001) docker     (999)    11175 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityModelDetail.h
--rw-r--r--   0 runner    (1001) docker     (999)     3738 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/MeshChecking.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     2689 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/MeshChecking.h
--rw-r--r--   0 runner    (1001) docker     (999)     1320 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/calculation/PolyhedronTransform.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/src/polyhedralGravity/input/
--rw-r--r--   0 runner    (1001) docker     (999)     1427 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/input/ConfigSource.h
--rw-r--r--   0 runner    (1001) docker     (999)      488 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/input/DataSource.h
--rw-r--r--   0 runner    (1001) docker     (999)     6104 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/input/TetgenAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     6096 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/input/TetgenAdapter.h
--rw-r--r--   0 runner    (1001) docker     (999)     2703 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/input/YAMLConfigReader.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     3367 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/input/YAMLConfigReader.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/src/polyhedralGravity/model/
--rw-r--r--   0 runner    (1001) docker     (999)     7647 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/model/GravityModelData.h
--rw-r--r--   0 runner    (1001) docker     (999)     5574 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/model/Polyhedron.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/src/polyhedralGravity/output/
--rw-r--r--   0 runner    (1001) docker     (999)     1222 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/output/CSVWriter.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     1878 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/output/CSVWriter.h
--rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/output/Logging.cpp
--rw-r--r--   0 runner    (1001) docker     (999)     1152 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/output/Logging.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/src/polyhedralGravity/util/
--rw-r--r--   0 runner    (1001) docker     (999)     1309 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/util/UtilityConstants.h
--rw-r--r--   0 runner    (1001) docker     (999)    13623 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/util/UtilityContainer.h
--rw-r--r--   0 runner    (1001) docker     (999)     1811 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravity/util/UtilityThrust.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 19:04:06.627157 polyhedral_gravity-2.1/src/polyhedralGravityPython/
--rw-r--r--   0 runner    (1001) docker     (999)     1061 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravityPython/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (999)     9451 2023-08-31 19:03:59.000000 polyhedral_gravity-2.1/src/polyhedralGravityPython/PolyhedralGravityPython.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.332030 polyhedral_gravity-3.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36310 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17185 2024-04-18 22:17:28.332030 polyhedral_gravity-3.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.328030 polyhedral_gravity-3.0rc3/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/FindSphinx.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/gtest.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/pybind11.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/spdlog.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/tbb.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/tetgen.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/thrust.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/xsimd.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-18 22:17:17.000000 polyhedral_gravity-3.0rc3/cmake/yaml.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.332030 polyhedral_gravity-3.0rc3/polyhedral_gravity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17185 2024-04-18 22:17:28.000000 polyhedral_gravity-3.0rc3/polyhedral_gravity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-18 22:17:28.000000 polyhedral_gravity-3.0rc3/polyhedral_gravity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:17:28.000000 polyhedral_gravity-3.0rc3/polyhedral_gravity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:17:28.000000 polyhedral_gravity-3.0rc3/polyhedral_gravity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 22:17:28.000000 polyhedral_gravity-3.0rc3/polyhedral_gravity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 22:17:28.332030 polyhedral_gravity-3.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.328030 polyhedral_gravity-3.0rc3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.328030 polyhedral_gravity-3.0rc3/src/polyhedralGravity/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.328030 polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/ConfigSource.h
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/DataSource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/TetgenAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/TetgenAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/YAMLConfigReader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/YAMLConfigReader.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.328030 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    16716 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityEvaluable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityEvaluable.h
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModelData.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25085 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModelDetail.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11006 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModelDetail.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/Polyhedron.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17551 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/Polyhedron.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.332030 polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/CSVWriter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/CSVWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/Logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/Logging.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.332030 polyhedral_gravity-3.0rc3/src/polyhedralGravity/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/util/UtilityConstants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/util/UtilityContainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravity/util/UtilityThrust.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:17:28.332030 polyhedral_gravity-3.0rc3/src/polyhedralGravityPython/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravityPython/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20584 2024-04-18 22:17:24.000000 polyhedral_gravity-3.0rc3/src/polyhedralGravityPython/PolyhedralGravityPython.cpp
```

### Comparing `polyhedral_gravity-2.1/CMakeLists.txt` & `polyhedral_gravity-3.0rc3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/LICENSE` & `polyhedral_gravity-3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/README.md` & `polyhedral_gravity-3.0rc3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,327 @@
+Metadata-Version: 2.1
+Name: polyhedral_gravity
+Version: 3.0rc3
+Summary: Package to compute full gravity tensor of a given constant density polyhedron for arbitrary points according to the geodetic convention
+Author: Jonas Schuhmacher
+Author-email: jonas.schuhmacher@tum.de
+License: GPLv3
+Project-URL: Homepage, https://github.com/esa/polyhedral-gravity-model
+Project-URL: Source, https://github.com/esa/polyhedral-gravity-model
+Project-URL: Documentation, https://esa.github.io/polyhedral-gravity-model/
+Project-URL: Issues, https://github.com/esa/polyhedral-gravity-model/issues
+Project-URL: Changelog, https://github.com/esa/polyhedral-gravity-model/releases
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # polyhedral-gravity-model
 
-![Build and Test](https://github.com/schuhmaj/polyhedral-gravity-model-cpp/actions/workflows/ctest.yml/badge.svg)
-[![Documentation Status](https://readthedocs.org/projects/polyhedral-gravity-model-cpp/badge/?version=latest)](https://polyhedral-gravity-model-cpp.readthedocs.io/en/latest/?badge=latest)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/esa/polyhedral-gravity-model/.github%2Fworkflows%2Fbuild-and-test.yml?logo=GitHub%20Actions&label=Build%20and%20Test)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/esa/polyhedral-gravity-model/.github%2Fworkflows%2Fdocs.yml?logo=GitBook&label=Documentation)
 ![GitHub](https://img.shields.io/github/license/esa/polyhedral-gravity-model)
 
 ![PyPI](https://img.shields.io/pypi/v/polyhedral-gravity)
 ![Static Badge](https://img.shields.io/badge/platform-linux--64_%7C_win--64_%7C_osx--64_%7C_linux--arm64_%7C_osx--arm64-lightgrey)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/polyhedral-gravity)
 
 ![Conda](https://img.shields.io/conda/v/conda-forge/polyhedral-gravity-model)
 ![Conda](https://img.shields.io/conda/pn/conda-forge/polyhedral-gravity-model)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/polyhedral-gravity-model)
 
 
+
+## Table of Contents
+
+- [References](#references)
+- [Documentation & Examples](#documentation--examples)
+  - [Input & Output (C++ and Python)](#input--output-c-and-python)
+  - [Minimal Python Example](#minimal-python-example)
+  - [Minimal C++ Example](#minimal-c-example)
+- [Installation](#installation)
+  - [With conda](#with-conda)
+  - [With pip](#with-pip)
+  - [From source](#from-source)
+- [C++ Library & Executable](#c-library--executable)
+  - [Building the C++ Library & Executable](#building-the-c-library--executable)
+  - [Running the C++ Executable](#running-the-c-executable)
+- [Testing](#testing)
+- [Contributing](#contributing)
+
+## References
+
 This code is a validated implementation in C++17 of the Polyhedral Gravity Model
 by Tsoulis et al.. It was created in a collaborative project between
 TU Munich and ESA's Advanced Concepts Team. Please refer to the
-[project report](https://mediatum.ub.tum.de/1695208)
+[project report](https://mediatum.ub.tum.de/doc/1695208/1695208.pdf)
 for extensive information about the theoretical background, related work,
 implementation & design decisions, application, verification,
 and runtime measurements of the presented code.
 
-
 The implementation is based on the
 paper [Tsoulis, D., 2012. Analytical computation of the full gravity tensor of a homogeneous arbitrarily shaped polyhedral source using line integrals. Geophysics, 77(2), pp.F1-F11.](http://dx.doi.org/10.1190/geo2010-0334.1)
-and its corresponding [implementation in FORTRAN](https://software.seg.org/2012/0001/index.html).
+and its corresponding implementation in FORTRAN.
 
 Supplementary details can be found in the more recent
 paper [TSOULIS, Dimitrios; GAVRIILIDOU, Georgia. A computational review of the line integral analytical formulation of the polyhedral gravity signal. Geophysical Prospecting, 2021, 69. Jg., Nr. 8-9, S. 1745-1760.](https://doi.org/10.1111/1365-2478.13134)
 and its corresponding [implementation in MATLAB](https://github.com/Gavriilidou/GPolyhedron),
 which is strongly based on the former implementation in FORTRAN.
 
-### Results and Plots
+## Documentation & Examples
+
+> [!NOTE]
+> The [GitHub Pages](https://esa.github.io/polyhedral-gravity-model) of this project
+contain the full extensive documentation of C++ Library and the Python Interface
+as well as background on the gravity model and advanced settings not detailed here!
+
+## Input & Output (C++ and Python)
+
+### Input
+
+The evaluation of the polyhedral gravity model requires the following parameters:
+
+| Name                                                                       |
+|----------------------------------------------------------------------------|
+| Polyhedral Mesh (either as vertices & faces or as polyhedral source files) |
+| Constant Density $\rho$                                                    |
 
-Some exemplary results and plots are stored in the
+The mesh and the constants density's unit must match.
+Have a look the documentation to view the [supported mesh files](https://esa.github.io/polyhedral-gravity-model/quickstart/supported_input.html).
+
+### Output
+
+The calculation outputs the following parameters for every Computation Point *P*.
+The units of the respective output depend on the units of the input parameters (mesh and density)!
+Hence, if e.g. your mesh is in $km$, the density must match. Further, output units will be different accordingly.
+
+|                            Name                            | Unit (if mesh in $[m]$ and $\rho$ in $[kg/m^3]$) |                              Comment                              |
+|:----------------------------------------------------------:|:------------------------------------------------:|:-----------------------------------------------------------------:|
+|                            $V$                             |       $\frac{m^2}{s^2}$ or $\frac{J}{kg}$        |           The potential or also called specific energy            |
+|                    $V_x$, $V_y$, $V_z$                     |                 $\frac{m}{s^2}$                  | The gravitational accerleration in the three cartesian directions |
+| $V_{xx}$, $V_{yy}$, $V_{zz}$, $V_{xy}$, $V_{xz}$, $V_{yz}$ |                 $\frac{1}{s^2}$                  |   The spatial rate of change of the gravitational accleration    |
+
+
+>[!NOTE]
+>This gravity model's output obeys to the geodesy and geophysics sign conventions.
+Hence, the potential $V$ for a polyhedron with a mass $m > 0$ is defined as **positive**.
+Accordingly, the accelerations are defined as $\textbf{g} = + \nabla V$.
+
+
+### Minimal Python Example
+
+The following example shows how to use the python interface to compute the gravity
+around a cube:
+
+```python
+import numpy as np
+from polyhedral_gravity import Polyhedron, GravityEvaluable, evaluate, PolyhedronIntegrity, NormalOrientation
+
+# We define the cube as a polyhedron with 8 vertices and 12 triangular faces
+# The polyhedron's normals point outwards (see below for checking this)
+# The density is set to 1.0
+cube_vertices = np.array(
+  [[-1, -1, -1], [1, -1, -1], [1, 1, -1], [-1, 1, -1],
+   [-1, -1, 1], [1, -1, 1], [1, 1, 1], [-1, 1, 1]]
+)
+cube_faces = np.array(
+  [[1, 3, 2], [0, 3, 1], [0, 1, 5], [0, 5, 4], [0, 7, 3], [0, 4, 7],
+   [1, 2, 6], [1, 6, 5], [2, 3, 6], [3, 7, 6], [4, 5, 6], [4, 6, 7]]
+)
+cube_density = 1.0
+computation_point = np.array([0, 0, 0])
+```
+
+We first, define a constant density Polyhedron from `vertices` and `faces`
+
+```python
+cube_polyhedron = Polyhedron(
+  polyhedral_source=(cube_vertices, cube_faces),
+  density=cube_density,
+)
+```
+
+In case you want to hand over the polyhedron via a supported file format,
+just replace the `polyhedral_source` argument with *a list of strings*,
+where each string is the path to a supported file format.
+
+Continuing, the simplest way to compute the gravity is to use the `evaluate` function:
+
+```python
+potential, acceleration, tensor = evaluate(
+  polyhedron=cube_polyhedron,
+  computation_points=computation_point,
+  parallel=True,
+)
+```
+
+The more advanced way is to use the `GravityEvaluable` class. It caches the
+internal data structure and properties which can be reused for multiple
+evaluations. This is especially useful if you want to compute the gravity
+for multiple computation points, but don't know the "future points" in advance.
+
+```python
+evaluable = GravityEvaluable(polyhedron=cube_polyhedron)
+potential, acceleration, tensor = evaluable(
+  computation_points=computation_point,
+  parallel=True,
+)
+```
+
+Note that the `computation_point` could also be (N, 3)-shaped array.
+In this case, the return value of `evaluate(..)` or an `GravityEvaluable` will
+be a list of triplets comprising potential, acceleration, and tensor.
+
+The gravity model requires that all the polyhedron's plane unit normals consistently
+point outwards or inwards the polyhedron. You can specify this via the `normal_orientation`.
+This property is - by default - checked when constructing the `Polyhedron`! So, don't worry, it
+is impossible if not **explicitly** disabled to create an invalid `Polyhedron`.
+You can disable/ enable this setting via the optional `integrity_check` flag and can even
+automatically repair the ordering via `HEAL`.
+As advanced user/ when you "know the mesh",
+you want to disable this check (via `DISABLE`) due to the additional runtime overhead!
+
+```python
+cube_polyhedron = Polyhedron(
+  polyhedral_source=(cube_vertices, cube_faces),
+  density=cube_density,
+  normal_orientation=NormalOrientation.INWARDS, # OUTWARDS (default) or INWARDS
+  integrity_check=PolyhedronIntegrity.VERIFY,   # AUTOMATIC (default) == VERIFY, DISABLE or HEAL
+)
+```
+
+> [!TIP]
+> More examples and plots are depicted in the
 [jupyter notebook](script/polyhedral-gravity.ipynb).
-It also provides a good introduction to the application of
-the python interface.
 
-## Documentation (readthedocs)
 
-The full extensive documentation can be found
-on [readthedocs](https://polyhedral-gravity-model-cpp.readthedocs.io/en/latest/).
+### Minimal C++ Example
 
-## Requirements
+The following example shows how to use the C++ library to compute the gravity.
+It works analogously to the Python example above.
 
-The project uses the following dependencies,
-all of them are **automatically** set-up via CMake:
+```cpp
+// Defining the input like above in the Python example
+std::vector<std::array<double, 3>> vertices = ...
+std::vector<std::array<size_t, 3>> faces = ...
+double density = 1.0;
+// The constant density polyhedron is defined by its vertices & faces
+// It also supports the hand-over of NormalOrientation and PolyhedronIntegrity as optional arguments
+// as above described for the Python Interface
+Polyhedron polyhedron{vertices, faces, density};
+std::vector<std::array<double, 3>> points = ...
+std::array<double, 3> point = points[0];
+bool parallel = true;
+```
+
+The C++ library provides also two ways to compute the gravity. Via
+the free function `evaluate`...
+
+```cpp
+const auto[pot, acc, tensor] = GravityModel::evaluate(polyhedron, point, parallel);
+```
+
+... or via the `GravityEvaluable` class.
+
+```cpp
+// Instantiation of the GravityEvaluable object
+GravityEvaluable evaluable{polyhedron};
+
+// From now, we can evaluate the gravity model for any point with
+const auto[potential, acceleration, tensor] = evaluable(point, parallel);
+// or for multiple points with
+const auto results = evaluable(points, parallel);
+```
 
-- GoogleTest (1.13.0 or compatible), only required for testing
-- spdlog (1.11.0 or compatible), required for logging
-- tetgen (1.6 or compatible), required for I/O
-- yaml-cpp (0.7.0 or compatible), required for I/O
-- thrust (2.1.0 or compatible), required for parallelization and utility
-- xsimd (11.1.0 or compatible), required for vectorization of the `atan(..)`
-- pybind11 (2.10.4 or compatible), required for the Python interface, but not the C++ standalone
+Similarly to Python, the C++ implementation also provides mesh checking capabilities.
+
+> [!TIP]
+> For reference, have a look at [the main method](./src/main.cpp) of the C++ executable.
 
-## Python interface
+## Installation
 
-### conda
+### With conda
 
 The python interface can be easily installed with
 [conda](https://anaconda.org/conda-forge/polyhedral-gravity-model):
 
-    conda install -c conda-forge polyhedral-gravity-model
+```bash
+conda install -c conda-forge polyhedral-gravity-model
+```
 
-### pip
+### With pip
 
-As a second option, you can also install the python interface with pip.
+As a second option, you can also install the python interface with pip from [PyPi](https://pypi.org/project/polyhedral-gravity/).
 
-    pip install polyhedral-gravity
+```bash
+pip install polyhedral-gravity
+```
 
 Binaries for the most common platforms are available on PyPI including
 Windows, Linux and macOS. For macOS and Linux, binaries for
 `x86_64` and `aarch64` are provided.
 In case `pip` uses the source distribution, please make sure that
-you have a C++17 capable compiler, CMake and ninja-build installed.
+you have a C++17 capable compiler and CMake installed.
 
 ### From source
 
+The project uses the following dependencies,
+all of them are **automatically** set-up via CMake:
+
+- GoogleTest (1.13.0 or compatible), only required for testing
+- spdlog (1.11.0 or compatible), required for logging
+- tetgen (1.6 or compatible), required for I/O
+- yaml-cpp (0.7.0 or compatible), required for I/O
+- thrust (2.1.0 or compatible), required for parallelization and utility
+- xsimd (11.1.0 or compatible), required for vectorization of the `atan(..)`
+- pybind11 (2.10.4 or compatible), required for the Python interface, but not the C++ standalone
+
 The module will be build using a C++17 capable compiler,
-CMake and ninja-build. Just execute the following command in
+CMake. Just execute the following command in
 the repository root folder:
 
-    pip install .
+```bash
+pip install .
+```
 
 To modify the build options (like parallelization) have a look
-at the `setupy.py` and the [next paragraph](#build-c). The options
+at the [next paragraph](#building-the-c-library--executable). The options
 are modified by setting the environment variables before executing
 the `pip install .` command, e.g.:
 
-    export POLYHEDRAL_GRAVITY_PARALLELIZATION="TBB"
-    pip install .
-
+```bash
+export POLYHEDRAL_GRAVITY_PARALLELIZATION="TBB"
+pip install .
+```
 
 (Optional: For a faster build you can install all dependencies available
 for your system in your local python environment. That way, they
 won't be fetched from GitHub.)
 
-## Build C++
+## C++ Library & Executable
+
+### Building the C++ Library & Executable
 
 The program is build by using CMake. So first make sure that you installed
 CMake and then follow these steps:
 
-    mkdir build
-    cd build
-    cmake .. <options>
-    cmake --build .
+```bash
+mkdir build
+cd build
+cmake .. <options>
+cmake --build .
+```
 
 The following options are available:
 
 |                             Name (Default) | Options                                                                                    |
 |-------------------------------------------:|:-------------------------------------------------------------------------------------------|
 | POLYHEDRAL_GRAVITY_PARALLELIZATION (`CPP`) | `CPP` = Serial Execution / `OMP` or `TBB` = Parallel Execution with OpenMP or Intel\'s TBB |
 |                        LOGGING_LEVEL (`2`) | `0` = TRACE/ `1` = DEBUG/ `2` = INFO / `3` = WARN/ `4` = ERROR/ `5` = CRITICAL/ `6` = OFF  |
@@ -121,90 +332,75 @@
 
 During testing POLYHEDRAL_GRAVITY_PARALLELIZATION=`TBB` has been the most performant.
 It is further not recommend to change the LOGGING_LEVEL to something else than `INFO=2`.
 
 The recommended CMake command would look like this (we only need to change `PARALLELIZATION_DEVICE`, since
 the defaults of the others are already correctly set):
 
-    cmake .. -POLYHEDRAL_GRAVITY_PARALLELIZATION="TBB"
-
-## Execution C++
+```bash
+cmake .. -POLYHEDRAL_GRAVITY_PARALLELIZATION="TBB"
+```
 
-### Overview
+### Running the C++ Executable
 
 After the build, the gravity model can be run by executing:
 
+```bash
     ./polyhedralGravity <YAML-Configuration-File>
+```
 
 where the YAML-Configuration-File contains the required parameters.
 Examples for Configuration Files and Polyhedral Source Files can be
 found in this repository in the folder `/example-config/`.
 
-### Config File
+#### Input Configuration File
 
 The configuration should look similar to the given example below.
 It is required to specify the source-files of the polyhedron's mesh (more info
-about the supported file in the [next paragraph](#polyhedron-source-files)), the density
+about the supported file in the [documentation](https://esa.github.io/polyhedral-gravity-model/quickstart/supported_input.html)), the density
 of the polyhedron, and the wished computation points where the
 gravity tensor shall be computed.
 Further one must specify the name of the .csv output file.
 
 ````yaml
 ---
 gravityModel:
   input:
     polyhedron: #polyhedron source-file(s)
       - "../example-config/data/tsoulis.node"   # .node contains the vertices
       - "../example-config/data/tsoulis.face"   # .face contains the triangular faces
-    density: 2670.0                             # constant density in [kg/m^3]
+    density: 2670.0                             # constant density, units must match with the mesh (see section below)
     points: # Location of the computation point(s) P
       - [ 0, 0, 0 ]                             # Here it is situated at the origin
-    check_mesh: true                            # Fully optional, enables input checking (not given: false)
+    check_mesh: true                            # Fully optional, enables mesh autodetect+repair of 
+                                                # the polyhedron's vertex ordering (not given: true)
   output:
     filename: "gravity_result.csv"              # The name of the output file 
 
 ````
 
-### Polyhedron Source Files
+#### Output
 
-The implementation supports multiple common mesh formats for
-the polyhedral source. These include:
+The executable produces a CSV file containing $V$, $V_x$, $V_y$, $V_z$,
+$V_{xx}$, $V_{yy}$, $V_{zz}$, $V_{xy}$, $V_{xz}$, $V_{yz}$ for every
+computation point *P*.
 
-|     File Suffix     |                        Name                        | Comment                                                                                                                                          |
-|:-------------------:|:--------------------------------------------------:|--------------------------------------------------------------------------------------------------------------------------------------------------|
-| `.node` and `.face` |                   TetGen's files                   | These two files need to be given as a pair to the input. [Documentation of TetGen's files](https://wias-berlin.de/software/tetgen/fformats.html) |
-|       `.mesh`       |                 Medit's mesh files                 | Single file containing every needed mesh information.                                                                                            |
-|       `.ply`        | The Polygon File format/ Stanfoard Triangle format | Single file containing every needed mesh information. Blender File Format.                                                                       |
-|       `.off`        |                 Object File Format                 | Single file containing every needed mesh information.                                                                                            |
-|       `.stl`        |              Stereolithography format              | Single file containing every needed mesh information. Blender File Format.                                                                       |                                         
-
-**Notice!** Only the ASCII versions of those respective files are supported! This is especially
-important for e.g. the `.ply` files which also can be in binary format.
-
-Good tools to convert your Polyhedron to a supported format (also for interchanging
-ASCII and binary format) are e.g.:
-
-- [Meshio](https://github.com/nschloe/meshio) for Python
-- [OpenMesh](https://openmesh-python.readthedocs.io/en/latest/readwrite.html) for Python
-
-The vertices in the input mesh file must be ordered so that the plane unit normals point outwards of the polyhedron for
-every face.
-One can use the program input-checking procedure to ensure the correct format. This method is activated via the
-corresponding configuration option and uses the Möller–Trumbore intersection algorithm. Notice that this algorithm is a
-quadratic complexity, so the check should only be utilized in case of uncertainty.
+## Testing
 
-### Output
+The project uses GoogleTest for testing. In oder to execute those
+tests just execute the following command in the build directory:
 
-The calculation outputs the following parameters for every Computation Point _P_:
+```bash
+ctest
+```
 
-|             Name             |      Unit       |                              Comment                              |
-|:----------------------------:|:---------------:|:-----------------------------------------------------------------:|
-|              V               | m^2/s^2 or J/kg |           The potential or also called specific energy            |
-|          Vx, Vy, Vz          |      m/s^2      | The gravitational accerleration in the three cartesian directions |
-| Vxx, Vyy, Vzz, Vxy, Vxz, Vyz |      1/s^2      |   The spatial rate of change of the gravitational accleration    |
+For the Python test suite, please execute the following command in the repository root folder:
 
-## Testing C++
+```bash
+pytest
+```
 
-The project uses GoogleTest for testing. In oder to execute those
-tests just execute the following command in the build directory:
+## Contributing
 
-    ctest
+We are happy to accept contributions to the project in the form of
+suggestions, bug reports and pull requests. Please have a look at
+the [contributing guidelines](CONTRIBUTING.md) for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `polyhedral_gravity-2.1/cmake/gtest.cmake` & `polyhedral_gravity-3.0rc3/cmake/gtest.cmake`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/cmake/spdlog.cmake` & `polyhedral_gravity-3.0rc3/cmake/spdlog.cmake`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/cmake/tetgen.cmake` & `polyhedral_gravity-3.0rc3/cmake/tetgen.cmake`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/cmake/thrust.cmake` & `polyhedral_gravity-3.0rc3/cmake/thrust.cmake`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/cmake/yaml.cmake` & `polyhedral_gravity-3.0rc3/cmake/yaml.cmake`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/polyhedral_gravity.egg-info/SOURCES.txt` & `polyhedral_gravity-3.0rc3/polyhedral_gravity.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,30 +16,28 @@
 polyhedral_gravity.egg-info/SOURCES.txt
 polyhedral_gravity.egg-info/dependency_links.txt
 polyhedral_gravity.egg-info/not-zip-safe
 polyhedral_gravity.egg-info/top_level.txt
 src/CMakeLists.txt
 src/main.cpp
 src/polyhedralGravity/CMakeLists.txt
-src/polyhedralGravity/calculation/GravityEvaluable.cpp
-src/polyhedralGravity/calculation/GravityEvaluable.h
-src/polyhedralGravity/calculation/GravityModel.cpp
-src/polyhedralGravity/calculation/GravityModel.h
-src/polyhedralGravity/calculation/GravityModelDetail.cpp
-src/polyhedralGravity/calculation/GravityModelDetail.h
-src/polyhedralGravity/calculation/MeshChecking.cpp
-src/polyhedralGravity/calculation/MeshChecking.h
-src/polyhedralGravity/calculation/PolyhedronTransform.h
 src/polyhedralGravity/input/ConfigSource.h
 src/polyhedralGravity/input/DataSource.h
 src/polyhedralGravity/input/TetgenAdapter.cpp
 src/polyhedralGravity/input/TetgenAdapter.h
 src/polyhedralGravity/input/YAMLConfigReader.cpp
 src/polyhedralGravity/input/YAMLConfigReader.h
+src/polyhedralGravity/model/GravityEvaluable.cpp
+src/polyhedralGravity/model/GravityEvaluable.h
+src/polyhedralGravity/model/GravityModel.cpp
+src/polyhedralGravity/model/GravityModel.h
 src/polyhedralGravity/model/GravityModelData.h
+src/polyhedralGravity/model/GravityModelDetail.cpp
+src/polyhedralGravity/model/GravityModelDetail.h
+src/polyhedralGravity/model/Polyhedron.cpp
 src/polyhedralGravity/model/Polyhedron.h
 src/polyhedralGravity/output/CSVWriter.cpp
 src/polyhedralGravity/output/CSVWriter.h
 src/polyhedralGravity/output/Logging.cpp
 src/polyhedralGravity/output/Logging.h
 src/polyhedralGravity/util/UtilityConstants.h
 src/polyhedralGravity/util/UtilityContainer.h
```

### Comparing `polyhedral_gravity-2.1/setup.py` & `polyhedral_gravity-3.0rc3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 import re
 import subprocess
+import shutil
 import sys
 
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 
 # ---------------------------------------------------------------------------------
 # Modify these variables to customize the build of the polyhedral gravity interface
 # All variables can be overwritten by setting equally named env variables
 # ---------------------------------------------------------------------------------
-# The generator used for CMake
-CMAKE_GENERATOR = "Ninja"
 # The other CMake options
 CMAKE_OPTIONS = {
     # The Build Type (Should be release!)
     "CMAKE_BUILD_TYPE": "Release",
     # Modify to change the parallelization (Default value: TBB)
     "POLYHEDRAL_GRAVITY_PARALLELIZATION": "TBB",
     # Default value (INFO=2)
@@ -33,14 +32,33 @@
     # Should be of course ON!
     "BUILD_POLYHEDRAL_GRAVITY_PYTHON_INTERFACE": "ON",
     # Build static libs by default (On conda-forge we build shared libs by setting this to ON)
     "BUILD_SHARED_LIBS": "OFF"
 }
 # ---------------------------------------------------------------------------------
 
+
+def is_ninja_installed():
+    """Returns true if ninja build tool is installed. False otherwise."""
+    return shutil.which("ninja") is not None
+
+
+def get_cmake_generator():
+    """Returns the CMake generator if specified as environment variable.
+    If not, returns "Ninja" if ninja build is installed.
+    Otherwise, none is returned.
+    """
+    os_env_generator = os.environ.get("CMAKE_GENERATOR", None)
+    if os_env_generator is not None:
+        return os_env_generator
+    elif is_ninja_installed():
+        return "Ninja"
+    else:
+        return None
+
 # -----------------------------------------------------------------------------------------
 # The following is adapted from https://github.com/pybind/cmake_example/blob/master/setup.py
 # -----------------------------------------------------------------------------------------
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
@@ -91,23 +109,24 @@
         if os.environ.get("_LIBCPP_DISABLE_AVAILABILITY"):
             cmake_args += [
                 "-D_LIBCPP_DISABLE_AVAILABILITY=ON"
             ]
 
         # Sets the CMake Generator if specified (this is separate from the other variables since it is given to
         # CMake vie the -G prefix
-        final_generator = os.environ.get("CMAKE_GENERATOR", CMAKE_GENERATOR)
-        cmake_args += [
-            f"-G{final_generator}"
-        ]
+        cmake_generator = get_cmake_generator()
+        if cmake_generator is not None:
+            cmake_args += [
+                f"-G{cmake_generator}"
+            ]
 
         # MSVC special cases
         if self.compiler.compiler_type == "msvc":
             # Single config generators are handled "normally"
-            single_config = any(x in CMAKE_GENERATOR for x in {"NMake", "Ninja"})
+            single_config = any(x in cmake_generator for x in {"NMake", "Ninja"})
             # Multi-config generators have a different way to specify configs
             if not single_config:
                 cmake_args += [
                     f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{CMAKE_OPTIONS['CMAKE_BUILD_TYPE'].upper()}={extdir}"
                 ]
                 build_args += ["--config", CMAKE_OPTIONS['CMAKE_BUILD_TYPE']]
 
@@ -138,30 +157,55 @@
         subprocess.check_call(["cmake", ext.sourcedir] + cmake_args, cwd=build_temp)
         subprocess.check_call(["cmake", "--build", "."] + build_args, cwd=build_temp)
 
 
 # -----------------------------------------------------------------------------------------
 
 
+picture_in_readme = '''<p align="center">
+  <img src="paper/figures/eros_010.png" width="50%">
+  <br>
+  <em>
+    <a href="https://github.com/gomezzz/geodesyNets/blob/master/3dmeshes/eros_lp.pk">Mesh of (433) Eros</a> with 739 vertices and 1474 faces
+  </em>
+</p>'''
+
+
 # --------------------------------------------------------------------------------
 # Modify these entries to customize the package metadata of the polyhedral gravity
 # --------------------------------------------------------------------------------
 setup(
     name="polyhedral_gravity",
-    version="2.1",
+    version="3.0rc3",
     author="Jonas Schuhmacher",
     author_email="jonas.schuhmacher@tum.de",
-    description="Package to compute full gravity tensor of a given constant density polyhedron for arbitrary points",
-    long_description="""
-        The package polyhedral_gravity provides a simple to use interface for the evaluation of the full gravity
-        tensor of a constant density polyhedron at given computation points. It is based on a fast, parallelized
-        backbone in C++ capable of evaluating the gravity at thousands of computation points in the fraction of a second.
-    """,
+    description="Package to compute full gravity tensor of a given constant density polyhedron for arbitrary points "
+                "according to the geodetic convention",
+    long_description=open("README.md").read().replace(picture_in_readme, ''),
+    long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension("polyhedral_gravity")],
     cmdclass={"build_ext": CMakeBuild},
     license="GPLv3",
     license_file="LICENSE",
     zip_safe=False,
     python_requires=">=3.6",
     include_package_data=True,
+    project_urls={
+        "Homepage": "https://github.com/esa/polyhedral-gravity-model",
+        "Source": "https://github.com/esa/polyhedral-gravity-model",
+        "Documentation": "https://esa.github.io/polyhedral-gravity-model/",
+        "Issues": "https://github.com/esa/polyhedral-gravity-model/issues",
+        "Changelog": "https://github.com/esa/polyhedral-gravity-model/releases",
+    },
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Programming Language :: C++",
+        "Programming Language :: Python",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS",
+        "Operating System :: POSIX :: Linux",
+        "Intended Audience :: Science/Research",
+        "Topic :: Scientific/Engineering :: Physics",
+    ],
 )
 # --------------------------------------------------------------------------------
```

### Comparing `polyhedral_gravity-2.1/src/CMakeLists.txt` & `polyhedral_gravity-3.0rc3/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/src/main.cpp` & `polyhedral_gravity-3.0rc3/src/main.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,35 @@
 #include <chrono>
 #include "polyhedralGravity/input/ConfigSource.h"
 #include "polyhedralGravity/input/YAMLConfigReader.h"
-#include "polyhedralGravity/calculation/GravityModel.h"
-#include "polyhedralGravity/calculation/MeshChecking.h"
+#include "polyhedralGravity/model/GravityModel.h"
 #include "polyhedralGravity/output/Logging.h"
 #include "polyhedralGravity/output/CSVWriter.h"
 
 int main(int argc, char *argv[]) {
     using namespace polyhedralGravity;
     if (argc != 2) {
         SPDLOG_LOGGER_INFO(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(), "Wrong program call! "
                                                                                 "Please use the program like this:\n"
                                                                                 "./polyhedralGravity [YAML-Configuration-File]\n");
         return 0;
     }
 
     try {
-
         std::shared_ptr<ConfigSource> config = std::make_shared<YAMLConfigReader>(argv[1]);
-        auto poly = config->getDataSource()->getPolyhedron();
+        auto polyhedralSource = config->getDataSource()->getPolyhedralSource();
         auto density = config->getDensity();
         auto computationPoints = config->getPointsOfInterest();
         auto outputFileName = config->getOutputFileName();
-        bool checkPolyhedralInput = config->getMeshInputCheckStatus();
-
-        // Checking that the vertices are correctly set-up in the input if activated
-        if (checkPolyhedralInput) {
-            SPDLOG_LOGGER_INFO(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(), "Checking mesh...");
-            if (!MeshChecking::checkTrianglesNotDegenerated(poly)) {
-                throw std::runtime_error{
-                        "At least on triangle in the mesh is degenerated and its surface area equals zero!"};
-            } else if (!MeshChecking::checkNormalsOutwardPointing(poly)) {
-                throw std::runtime_error{
-                        "The plane unit normals are not pointing outwards! Please check the order "
-                        "of the vertices in the polyhedral input source!"};
-            }  else {
-                SPDLOG_LOGGER_INFO(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(), "The mesh is fine.");
-            }
-        }
+        PolyhedronIntegrity checkPolyhedralInput = config->getMeshInputCheckStatus() ? PolyhedronIntegrity::HEAL : PolyhedronIntegrity::DISABLE;
 
         SPDLOG_LOGGER_INFO(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(), "The calculation started...");
         auto start = std::chrono::high_resolution_clock::now();
-        auto result = GravityModel::evaluate(poly, density, computationPoints);
+        Polyhedron polyhedron{polyhedralSource, density, NormalOrientation::OUTWARDS, checkPolyhedralInput};
+        auto result = GravityModel::evaluate(polyhedron, computationPoints, true);
         auto end = std::chrono::high_resolution_clock::now();
         auto duration = end - start;
         auto ms = std::chrono::duration_cast<std::chrono::microseconds>(duration);
         SPDLOG_LOGGER_INFO(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(),
                            "The calculation finished. It took {} microseconds.", ms.count());
         SPDLOG_LOGGER_INFO(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(),
                            "Or on average {} microseconds/point",
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityEvaluable.cpp` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityEvaluable.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -31,23 +31,21 @@
 
     template<bool Parallelization>
     GravityModelResult GravityEvaluable::evaluate(const Array3 &computationPoint) const {
         using namespace GravityModel::detail;
         using namespace util;
         SPDLOG_LOGGER_DEBUG(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(),
                             "Evaluation for computation point P = [{}, {}, {}] started, given density = {} kg/m^3",
-                            computationPoint[0], computationPoint[1], computationPoint[2], _density);
+                            computationPoint[0], computationPoint[1], computationPoint[2], _polyhedron.getDensity());
         /*
          * Calculate V and Vx, Vy, Vz and Vxx, Vyy, Vzz, Vxy, Vxz, Vyz
          */
-        auto polyhedronIterator = transformPolyhedron(_polyhedron, computationPoint);
-        auto zip1 = util::zip(polyhedronIterator.first, _segmentVectors.begin(), _planeUnitNormals.begin(),
-                              _segmentUnitNormals.begin());
-        auto zip2 = util::zip(polyhedronIterator.second, _segmentVectors.end(), _planeUnitNormals.end(),
-                              _segmentUnitNormals.end());
+        const auto &[polyBegin, polyEnd] = _polyhedron.transformIterator(computationPoint);
+        auto zip1 = util::zip(polyBegin, _segmentVectors.begin(), _planeUnitNormals.begin(), _segmentUnitNormals.begin());
+        auto zip2 = util::zip(polyEnd, _segmentVectors.end(), _planeUnitNormals.end(), _segmentUnitNormals.end());
 
         SPDLOG_LOGGER_DEBUG(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(),
                             "Starting to iterate over the planes...");
         GravityModelResult result{};
         auto &[potential, acceleration, gradiometricTensor] = result;
 
         if constexpr (Parallelization) {
@@ -58,19 +56,19 @@
                                               util::operator+ < double, Array3, Array6 > );
         }
 
         SPDLOG_LOGGER_DEBUG(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger(),
                             "Finished the sums. Applying final prefix and eliminating rounding errors.");
 
         //9. Step: Compute prefix consisting of GRAVITATIONAL_CONSTANT * density
-        const double prefix = util::GRAVITATIONAL_CONSTANT * _density;
+        const double prefix = util::GRAVITATIONAL_CONSTANT * _polyhedron.getDensity() * _polyhedron.getOrientationFactor();
 
         //10. Step: Final expressions after application of the prefix (and a division by 2 for the potential)
         potential = (potential * prefix) / 2.0;
-        acceleration = acceleration * prefix;
+        acceleration = acceleration * (-1.0 * prefix);
         gradiometricTensor = gradiometricTensor * prefix;
         return result;
     }
 
     // Explicit template instantiation of the single point evaluate method
     template GravityModelResult GravityEvaluable::evaluate<true>(const Array3 &computationPoints) const;
 
@@ -90,14 +88,15 @@
                                   return this->evaluate<false>(computationPoint);
                               });
         }
         return result;
     }
 
     // Explicit template instantiation of the multipoint evaluate method
+
     template std::vector<GravityModelResult>
     GravityEvaluable::evaluate<true>(const std::vector<Array3> &computationPoints) const;
 
     template std::vector<GravityModelResult>
     GravityEvaluable::evaluate<false>(const std::vector<Array3> &computationPoints) const;
 
     GravityModelResult
@@ -228,19 +227,19 @@
         // Equation (12): N_p * sum
         // Equation (13): already done above, just concat the two components for later summation
         return std::make_tuple(planeNormalOrientation * planeDistance * planeSumPotentialAcceleration,
                                planeUnitNormal * planeSumPotentialAcceleration, concat(first, second));
     }
 
     std::string GravityEvaluable::toString() const {
-        std::stringstream ss;
-        ss << "<polyhedral_gravity.GravityEvaluable, density=" << _density << ", vertices= "
+        std::stringstream sstream;
+        sstream << "<polyhedral_gravity.GravityEvaluable, density=" << _polyhedron.getDensity() << ", vertices= "
            << _polyhedron.countVertices() << ", faces= " << _polyhedron.countFaces() << ">";
-        return ss.str();
+        return sstream.str();
     }
 
-    std::tuple<Polyhedron, double, std::vector<Array3Triplet>, std::vector<Array3>, std::vector<Array3Triplet>>
+    std::tuple<Polyhedron, std::vector<Array3Triplet>, std::vector<Array3>, std::vector<Array3Triplet>>
     GravityEvaluable::getState() const {
-        return std::make_tuple(_polyhedron, _density, _segmentVectors, _planeUnitNormals, _segmentUnitNormals);
+        return std::make_tuple(_polyhedron, _segmentVectors, _planeUnitNormals, _segmentUnitNormals);
     }
 
 }
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityEvaluable.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityEvaluable.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #pragma once
 
 #include <tuple>
 #include <variant>
 #include <string>
+#include <optional>
 #include <sstream>
 
 #include "thrust/transform.h"
 #include "thrust/execution_policy.h"
 
-#include "polyhedralGravity/calculation/GravityModelDetail.h"
+#include "GravityModelDetail.h"
+#include "polyhedralGravity/util/UtilityContainer.h"
 #include "polyhedralGravity/input/TetgenAdapter.h"
-#include "polyhedralGravity/model/GravityModelData.h"
-#include "polyhedralGravity/model/Polyhedron.h"
+#include "GravityModelData.h"
+#include "Polyhedron.h"
 
 
 namespace polyhedralGravity {
 
     /**
      * Class for evaluating the polyhedrale gravity model for a given constant density polyhedron.
      * Caches the polyhedron and data which is independent of the computation point P.
@@ -23,77 +25,60 @@
      * at computation point P and choosing between parallel and serial evaluation.
      */
     class GravityEvaluable {
 
         /** The constant density polyhedron consisting of vertices and triangular faces */
         const Polyhedron _polyhedron;
 
-        /** The constant density of the polyhedron in [kg/m^3] */
-        const double _density;
-
         /** Cache for the segment vectors (segments between vertices of a polyhedral face) */
-        mutable std::vector<Array3Triplet> _segmentVectors;
+        mutable std::vector<Array3Triplet> _segmentVectors{};
 
         /** Cache for the plane unit normals (unit normals of the polyhedral faces) */
-        mutable std::vector<Array3> _planeUnitNormals;
+        mutable std::vector<Array3> _planeUnitNormals{};
 
         /** Cache for the segment unit normals (unit normals of each the polyhedral faces' segments) */
-        mutable std::vector<Array3Triplet> _segmentUnitNormals;
-
+        mutable std::vector<Array3Triplet> _segmentUnitNormals{};
 
     public:
-
         /**
          * Instantiates a GravityEvaluable with a given constant density polyhedron.
-         * @param polyhedron - the polyhedron
-         * @param density - the constant density in [kg/m^3]
+         * In contrast to the {@link GravityModel::evaluate}, this evaluate method on the {@link GravityEvaluable}
+         * caches intermediate results and input data and subsequent evaluations will be faster.
          *
-         * @note This is a separate constructor since the polyhedron as a class it not exposed to the user via
-         * the Python Interface. Thus, this constructor is only available via the C++ interface.
-         */
-        GravityEvaluable(const Polyhedron &polyhedron, double density) : _polyhedron{polyhedron}, _density{density} {
-            this->prepare();
-        }
-
-        /**
-         * Instantiates a GravityEvaluable with a given constant density polyhedron.
-         * @param polyhedralSource - the vertices & faces of the polyhedron as tuple or the filenames of the files
-         * @param density - the constant density in [kg/m^3]
+         * @param polyhedron the constant density polyhedron
          */
-        GravityEvaluable(const PolyhedralSource &polyhedralSource, double density) : _polyhedron{
-                std::holds_alternative<std::tuple<std::vector<Array3>, std::vector<IndexArray3>>>(polyhedralSource)
-                ? Polyhedron{std::get<std::tuple<std::vector<Array3>, std::vector<IndexArray3>>>(polyhedralSource)}
-                : TetgenAdapter(std::get<std::vector<std::string>>(polyhedralSource)).getPolyhedron()},
-                                                                                     _density{density} {
+        explicit GravityEvaluable(const Polyhedron &polyhedron) :
+            _polyhedron{polyhedron} {
             this->prepare();
         }
 
         /**
          * Instantiates a GravityEvaluable with a given constant density polyhedron and caches.
          * This is for restoring a GravityEvaluable from a previous state.
-         * @param polyhedron - the polyhedron
-         * @param density - the constant density in [kg/m^3]
-         * @param segmentVectors - the segment vectors
-         * @param planeUnitNormals - the plane unit normals
-         * @param segmentUnitNormals - the segment unit normals
+         * @param polyhedron the polyhedron
+         * @param segmentVectors the segment vectors
+         * @param planeUnitNormals the plane unit normals
+         * @param segmentUnitNormals the segment unit normals
          */
-        GravityEvaluable(const Polyhedron &polyhedron, double density, const std::vector<Array3Triplet> &segmentVectors,
+        GravityEvaluable(const Polyhedron &polyhedron,
+                         const std::vector<Array3Triplet> &segmentVectors,
                          const std::vector<Array3> &planeUnitNormals,
-                         const std::vector<Array3Triplet> &segmentUnitNormals) : _polyhedron{polyhedron},
-                                                                                 _density{density},
-                                                                                 _segmentVectors{segmentVectors},
-                                                                                 _planeUnitNormals{planeUnitNormals},
-                                                                                 _segmentUnitNormals{
-                                                                                         segmentUnitNormals} {}
+                         const std::vector<Array3Triplet> &segmentUnitNormals) :
+            _polyhedron{polyhedron},
+            _segmentVectors{segmentVectors},
+            _planeUnitNormals{planeUnitNormals},
+            _segmentUnitNormals{
+                    segmentUnitNormals} {
+        }
 
         /**
          * Evaluates the polyhedrale gravity model for a given constant density polyhedron at computation
          * point P. Wrapper for evaluate<parallelization>.
-         * @param computationPoints - the computation point P or multiple computation points in a vector
-         * @param parallelization - if true, the calculation is parallelized
+         * @param computationPoints the computation point P or multiple computation points in a vector
+         * @param parallelization if true, the calculation is parallelized
          * @return the GravityModelResult containing the potential, acceleration and second derivative
          */
         inline std::variant<GravityModelResult, std::vector<GravityModelResult>>
         operator()(const std::variant<Array3, std::vector<Array3>> &computationPoints,
                    bool parallelization = true) const {
             if (parallelization) {
                 if (std::holds_alternative<Array3>(computationPoints)) {
@@ -110,60 +95,59 @@
             }
         }
 
         /**
          * Returns a string representation of the GravityEvaluable.
          * @return string representation of the GravityEvaluable
          */
-        std::string toString() const;
+        [[nodiscard]] std::string toString() const;
 
         /**
          * Returns the polyhedron, the density and the internal caches.
          *
          * @return tuple of polyhedron, density, segmentVectors, planeUnitNormals and segmentUnitNormals
          */
-        std::tuple<Polyhedron, double, std::vector<Array3Triplet>, std::vector<Array3>, std::vector<Array3Triplet>>
-        getState() const;
+        std::tuple<Polyhedron, std::vector<Array3Triplet>, std::vector<Array3>, std::vector<Array3Triplet>> getState() const;
 
     private:
 
         /**
          * Prepares the polyhedron for the evaluation by calculating the segment vectors, the plane unit normals
          * and the segment unit normals.
          * Called by the constructor once.
          */
         void prepare() const;
 
         /**
         * Evaluates the polyhedrale gravity model for a given constant density polyhedron at computation
         * point P.
-        * @tparam Parallelization - if true, the calculation is parallelized
-        * @param computationPoint - the computation Point P
+        * @tparam Parallelization if true, the calculation is parallelized
+        * @param computationPoint the computation Point P
         * @return the GravityModelResult containing the potential, the acceleration and the change of acceleration
         * at computation Point P
         */
         template<bool Parallelization = true>
-        GravityModelResult evaluate(const Array3 &computationPoint) const;
+        [[nodiscard]] GravityModelResult evaluate(const Array3 &computationPoint) const;
 
 
         /**
          * Evaluates the polyhedrale gravity model for a given constant density polyhedron at computation
          * at multiple computation points.
-         * @tparam Parallelization - if true, the calculation is parallelized
-         * @param computationPoints - the computation Points
+         * @tparam Parallelization if true, the calculation is parallelized
+         * @param computationPoints the computation Points
          * @return vector of GravityModelResults containing the potential, the acceleration and the change of acceleration
          */
         template<bool Parallelization = true>
-        std::vector<GravityModelResult> evaluate(const std::vector<Array3> &computationPoints) const;
+        [[nodiscard]] std::vector<GravityModelResult> evaluate(const std::vector<Array3> &computationPoints) const;
 
         /**
          * Evaluates the polyhedrale gravity model for a given constant density polyhedron at computation a certain face.
-         * @param tuple - consisting of face, segmentVectors, planeUnitNormal and segmentUnitNormals
+         * @param tuple consisting of face, segmentVectors, planeUnitNormal and segmentUnitNormals
          * @return the GravityModelResult containing the potential, the acceleration and the change of acceleration which
          * this face contributes to the computation point
          */
         static GravityModelResult
         evaluateFace(const thrust::tuple<Array3Triplet, Array3Triplet, Array3, Array3Triplet> &tuple);
 
     };
 
-} // namespace polyhedralGravity
+}// namespace polyhedralGravity
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityModel.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModel.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 #pragma once
 
-#include <utility>
 #include <array>
 #include <vector>
-#include <algorithm>
-#include <variant>
 
-#include "polyhedralGravity/calculation/GravityEvaluable.h"
+#include "polyhedralGravity/model/GravityEvaluable.h"
 #include "polyhedralGravity/model/GravityModelData.h"
 #include "polyhedralGravity/model/Polyhedron.h"
 
 /**
  * Namespace containing the methods used to evaluate the polyhedrale Gravity Model
  * @note Naming scheme corresponds to the following:
  * evaluate()           --> main Method for evaluating the gravity model
  * *()                  --> Methods calculating one property for the evaluation
  */
 namespace polyhedralGravity::GravityModel {
 
     /**
      * Evaluates the polyhedrale gravity model for a given constant density polyhedron at computation
      * point P.
-     * @param polyhedron - the polyhedron consisting of vertices and triangular faces
-     * @param density - the constant density in [kg/m^3]
-     * @param computationPoint - the computation Point P
-     * @param parallel - whether to evaluate in parallel or serial
+     * @param polyhedron the polyhedron consisting of vertices and triangular faces
+     * @param computationPoint the computation Point P
+     * @param parallel whether to evaluate in parallel or serial
      * @return the GravityModelResult containing the potential, the acceleration and the change of acceleration
      * at computation Point P
      */
-    GravityModelResult evaluate(const PolyhedronOrSource &polyhedron, double density, const Array3 &computationPoint, bool parallel = true);
+    GravityModelResult evaluate(const Polyhedron &polyhedron, const Array3 &computationPoint, bool parallel = true);
 
     /**
      * Evaluates the polyhedral gravity model for a given constant density polyhedron at multiple computation
      * points.
-     * @param polyhedron - the polyhedron consisting of vertices and triangular faces
-     * @param density - the constant density in [kg/m^3]
-     * @param computationPoints - vector of computation points
-     * @param parallel - whether to evaluate in parallel or serial
+     * @param polyhedron the polyhedron consisting of vertices and triangular faces
+     * @param computationPoints vector of computation points
+     * @param parallel whether to evaluate in parallel or serial
      * @return the GravityModelResult containing the potential, the acceleration and the change of acceleration
      * foreach computation Point P
      */
     std::vector<GravityModelResult>
-    evaluate(const PolyhedronOrSource &polyhedron, double density, const std::vector<Array3> &computationPoints, bool parallel = true);
+    evaluate(const Polyhedron &polyhedron, const std::vector<Array3> &computationPoints, bool parallel = true);
 
-}
+}
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityModelDetail.cpp` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModelDetail.cpp`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/calculation/GravityModelDetail.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModelDetail.h`

 * *Files 7% similar despite different names*

```diff
@@ -11,197 +11,196 @@
 #include "thrust/iterator/transform_iterator.h"
 #include "thrust/iterator/counting_iterator.h"
 #include "thrust/transform.h"
 #include "thrust/transform_reduce.h"
 #include "thrust/execution_policy.h"
 #include "xsimd/xsimd.hpp"
 
-#include "polyhedralGravity/calculation/PolyhedronTransform.h"
+#include "Polyhedron.h"
+#include "GravityModelData.h"
 #include "polyhedralGravity/input/TetgenAdapter.h"
-#include "polyhedralGravity/model/Polyhedron.h"
-#include "polyhedralGravity/model/GravityModelData.h"
 #include "polyhedralGravity/util/UtilityConstants.h"
 #include "polyhedralGravity/util/UtilityContainer.h"
 #include "polyhedralGravity/util/UtilityThrust.h"
 #include "polyhedralGravity/output/Logging.h"
 
 namespace polyhedralGravity::GravityModel::detail {
 
     /**
- * Computes the segment vectors G_ij for one plane of the polyhedron according to Tsoulis (18).
- * The segment vectors G_ij represent the vector from one vertex of the face to the neighboring vertex and
- * depict every line segment of the triangular face (A-B-C)
- * @param vertex0 - the first vertex A
- * @param vertex1 - the second vertex B
- * @param vertex2 - the third vertex C
- * @return the segment vectors for a plane
- */
+     * Computes the segment vectors G_ij for one plane of the polyhedron according to Tsoulis (18).
+     * The segment vectors G_ij represent the vector from one vertex of the face to the neighboring vertex and
+     * depict every line segment of the triangular face (A-B-C)
+     * @param vertex0 the first vertex A
+     * @param vertex1 the second vertex B
+     * @param vertex2 the third vertex C
+     * @return the segment vectors for a plane
+     */
     Array3Triplet buildVectorsOfSegments(const Array3 &vertex0, const Array3 &vertex1, const Array3 &vertex2);
 
     /**
      * Computes the plane unit normal N_p for one plane p of the polyhedron according to Tsoulis (19).
      * The plane unit normal is the outward pointing normal of the face from the polyhedron.
-     * @param segmentVector1 - first edge
-     * @param segmentVector2 - second edge
+     * @param segmentVector1 first edge
+     * @param segmentVector2 second edge
      * @return plane unit normal
      */
     Array3 buildUnitNormalOfPlane(const Array3 &segmentVector1, const Array3 &segmentVector2);
 
     /**
      * Computes the segment unit normals n_pq for one plane p of the polyhedron according to Tsoulis (20).
      * The segment unit normal n_pq represent the normal of one line segment of a polyhedrale face.
-     * @param segmentVectors - the segment vectors of the face G_p(0-2)
-     * @param planeUnitNormal - the plane unit normal N_p
+     * @param segmentVectors the segment vectors of the face G_p(0-2)
+     * @param planeUnitNormal the plane unit normal N_p
      * @return segment unit normals n_pq for plane p with q = {0, 1, 2}
      */
     Array3Triplet buildUnitNormalOfSegments(const Array3Triplet &segmentVectors, const Array3 &planeUnitNormal);
 
     /**
      * Computes the plane unit normal orientation/ direction sigma_p for one plane p of the polyhedron
      * according to Tsoulis (21).
      * The plane unit normal orientation values represents the relative position of computation point P
      * with respect to the pointing direction of N_p. E. g. if N_p points to the half-space containing P, the
      * inner product of N_p and -G_i1 will be positive, leading to a negative sigma_p.
      * If sigma_p is zero than P and P' lie geometrically in the same plane --> P == P'.
-     * @param planeUnitNormal - the plane unit normal N_p
-     * @param vertex0 - the first vertex of the plane
+     * @param planeUnitNormal the plane unit normal N_p
+     * @param vertex0 the first vertex of the plane
      * @return plane normal orientation
      */
     double computeUnitNormalOfPlaneDirection(const Array3 &planeUnitNormal, const Array3 &vertex0);
 
     /**
      * Calculates the Hessian Plane form spanned by three given points p, q, and r.
-     * @param p - first point on the plane
-     * @param q - second point on the plane
-     * @param r - third point on the plane
+     * @param p first point on the plane
+     * @param q second point on the plane
+     * @param r third point on the plane
      * @return HessianPlane
      * @related Cross-Product method https://tutorial.math.lamar.edu/classes/calciii/eqnsofplanes.aspx
      */
     HessianPlane computeHessianPlane(const Array3 &p, const Array3 &q, const Array3 &r);
 
     /**
      * Calculates the (plane) distances h_p of computation point P to the plane S_p given in Hessian Form
      * according to the following equation:
      * h_p = D / sqrt(A^2+B^2+C^2)
-     * @param hessianPlane - Hessian Plane Form of S_p
+     * @param hessianPlane Hessian Plane Form of S_p
      * @return plane distance h_p
      */
     double distanceBetweenOriginAndPlane(const HessianPlane &hessianPlane);
 
     /**
      * Computes P' for a given plane p according to equation (22) of Tsoulis paper.
      * P' is the orthogonal projection of the computation point P onto the plane S_p.
-     * @param planeUnitNormal - the plane unit normal N_p
-     * @param planeDistance - the distance from P to the plane h_p
-     * @param hessianPlane - the Hessian Plane Form
+     * @param planeUnitNormal the plane unit normal N_p
+     * @param planeDistance the distance from P to the plane h_p
+     * @param hessianPlane the Hessian Plane Form
      * @return P' for this plane
      */
     Array3 projectPointOrthogonallyOntoPlane(const Array3 &planeUnitNormal, double planeDistance,
                                              const HessianPlane &hessianPlane);
 
     /**
      * Computes the segment normal orientations/ directions sigma_pq for a given plane p.
      * If sigma_pq is negative, this denotes that n_pq points to the half-plane containing P'. Nn case
      * sigma_pq is positive, P' resides in the other half-plane and if sigma_pq is zero, then P' lies directly
      * on the segment pq.
-     * @param vertices - the vertices of this plane
-     * @param projectionPointOnPlane - the projection point P' for this plane
-     * @param segmentUnitNormalsForPlane - the segment unit normals sigma_pq for this plane
+     * @param vertices the vertices of this plane
+     * @param projectionPointOnPlane the projection point P' for this plane
+     * @param segmentUnitNormalsForPlane the segment unit normals sigma_pq for this plane
      * @return the segment normal orientations for the plane p
      */
     Array3 computeUnitNormalOfSegmentsDirections(const Array3Triplet &vertices, const Array3 &projectionPointOnPlane,
                                                  const Array3Triplet &segmentUnitNormalsForPlane);
 
     /**
      * Computes the orthogonal projection Points P'' foreach segment q of a given plane p.
-     * @param projectionPointOnPlane - the projection Point P'
-     * @param segmentNormalOrientations - the segment normal orientations sigma_pq for this plane p
-     * @param face - the vertices of the plane p
+     * @param projectionPointOnPlane the projection Point P'
+     * @param segmentNormalOrientations the segment normal orientations sigma_pq for this plane p
+     * @param face the vertices of the plane p
      * @return the orthogonal projection points of P on the segment P'' foreach segment q of p
      */
     Array3Triplet
     projectPointOrthogonallyOntoSegments(const Array3 &projectionPointOnPlane, const Array3 &segmentNormalOrientations,
                                          const Array3Triplet &face);
 
     /**
      * Calculates the point P'' for a given Segment consisting of vertices v1 and v2 and the orthogonal projection
      * point P' for the plane consisting of those vertices. Solves the three equations given in (24), (25) and (26).
-     * @param vertex1 - first endpoint of segment
-     * @param vertex2 - second endpoint of segment
-     * @param orthogonalProjectionPointOnPlane - the orthogonal projection P' of P on this plane
+     * @param vertex1 first endpoint of segment
+     * @param vertex2 second endpoint of segment
+     * @param orthogonalProjectionPointOnPlane the orthogonal projection P' of P on this plane
      * @return P'' for this segment
      * @note If sigma_pq is zero then P'' == P', this is not checked by this method, but has to be assured first
      */
     Array3 projectPointOrthogonallyOntoSegment(const Array3 &vertex1, const Array3 &vertex2,
                                                const Array3 &orthogonalProjectionPointOnPlane);
 
     /**
      * Computes the (segment) distances h_pq between P' for a given plane p and P'' for a given segment q of plane p.
-     * @param orthogonalProjectionPointOnPlane - the orthogonal projection point P' for p
-     * @param orthogonalProjectionPointOnSegments - the orthogonal projection points P'' for each segment q of p
+     * @param orthogonalProjectionPointOnPlane the orthogonal projection point P' for p
+     * @param orthogonalProjectionPointOnSegments the orthogonal projection points P'' for each segment q of p
      * @return distances h_pq for plane p
      */
     Array3 distancesBetweenProjectionPoints(const Array3 &orthogonalProjectionPointOnPlane,
                                             const Array3Triplet &orthogonalProjectionPointOnSegments);
 
     /**
      * Computes the 3D distances l1_pq and l2_pq between the computation point P and the line
      * segment endpoints of each polyhedral segment for one plane.
      * Computes the 1D distances s1_pq and s2_pq between orthogonal projection of P on the line
      * segment P''_pq and the line segment endpoints for each polyhedral segment for one plane
-     * @param segmentVectorsForPlane - the segment vectors G_pq for plane p
-     * @param orthogonalProjectionPointsOnSegmentForPlane - the orthogonal projection Points P'' for plane p
-     * @param face - the vertices of plane p
+     * @param segmentVectorsForPlane the segment vectors G_pq for plane p
+     * @param orthogonalProjectionPointsOnSegmentForPlane the orthogonal projection Points P'' for plane p
+     * @param face the vertices of plane p
      * @return distances l1_pq and l2_pq and s1_pq and s2_pq foreach segment q of plane p
      */
     std::array<Distance, 3> distancesToSegmentEndpoints(const Array3Triplet &segmentVectorsForPlane,
                                                         const Array3Triplet &orthogonalProjectionPointsOnSegmentForPlane,
                                                         const Array3Triplet &face);
 
     /**
      * Calculates the Transcendental Expressions LN_pq and AN_pq for every line segment of the polyhedron for
      * a given plane p.
      * LN_pq is calculated according to (14) using the natural logarithm and AN_pq is calculated according
      * to (15) using the arctan.
-     * @param distancesForPlane - the distances l1, l2, s1, s2 foreach segment q of plane p
-     * @param planeDistance - the plane distance h_p for plane p
-     * @param segmentDistancesForPlane - the segment distance h_pq for segment q of plane p
-     * @param segmentNormalOrientationsForPlane - the segment normal orientations n_pq for a plane p
-     * @param orthogonalProjectionPointOnPlane - the orthogonal projection point P' for plane p
-     * @param face - the vertices of plane p
+     * @param distancesForPlane the distances l1, l2, s1, s2 foreach segment q of plane p
+     * @param planeDistance the plane distance h_p for plane p
+     * @param segmentDistancesForPlane the segment distance h_pq for segment q of plane p
+     * @param segmentNormalOrientationsForPlane the segment normal orientations n_pq for a plane p
+     * @param orthogonalProjectionPointOnPlane the orthogonal projection point P' for plane p
+     * @param face the vertices of plane p
      * @return LN_pq and AN_pq foreach segment q of plane p
      */
     std::array<TranscendentalExpression, 3>
     computeTranscendentalExpressions(const std::array<Distance, 3> &distancesForPlane, double planeDistance,
                                      const Array3 &segmentDistancesForPlane,
                                      const Array3 &segmentNormalOrientationsForPlane,
                                      const Array3 &projectionPointVertexNorms);
 
     /**
      * Calculates the singularities (correction) terms according to the Flow text for a given plane p.
-     * @param segmentVectorsForPlane - the segment vectors for a given plane
-     * @param segmentNormalOrientationForPlane - the segment orientation sigma_pq
-     * @param projectionPointVertexNorms - the projection point P'
-     * @param planeUnitNormal - the plane unit normal N_p
-     * @param planeDistance - the plane distance h_p
-     * @param planeNormalOrientation - the plane normal orientation sigma_p
-     * @param face - the vertices of plane p
+     * @param segmentVectorsForPlane the segment vectors for a given plane
+     * @param segmentNormalOrientationForPlane the segment orientation sigma_pq
+     * @param projectionPointVertexNorms the projection point P'
+     * @param planeUnitNormal the plane unit normal N_p
+     * @param planeDistance the plane distance h_p
+     * @param planeNormalOrientation the plane normal orientation sigma_p
+     * @param face the vertices of plane p
      * @return the singularities for a plane p
      */
     std::pair<double, Array3>
     computeSingularityTerms(const Array3Triplet &segmentVectorsForPlane, const Array3 &segmentNormalOrientationForPlane,
                             const Array3 &projectionPointVertexNorms, const Array3 &planeUnitNormal,
                             double planeDistance, double planeNormalOrientation);
 
 
     /**
      * Computes the L2 norms of the orthogonal projection point P' on a plane p with each vertex of that plane p.
      * The values are later used to determine if P' is situated at a vertex.
-     * @param orthogonalProjectionPointOnPlane - the orthogonal projection point P'
-     * @param face - the vertices of plane p
+     * @param orthogonalProjectionPointOnPlane the orthogonal projection point P'
+     * @param face the vertices of plane p
      * @return the norms of p and each vertex
      */
     Array3
     computeNormsOfProjectionPointAndVertices(const Array3 &orthogonalProjectionPointOnPlane, const Array3Triplet &face);
 
 
 } // namespace polyhedralGravity::GravityModel::detail
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/input/ConfigSource.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/ConfigSource.h`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         /**
          * Returns the specified output file name.
          * @return a std::string with the filename
          */
         virtual std::string getOutputFileName() = 0;
 
         /**
-         * Returns the constant density rho of the given polyhedron in [kg/m^3].
+         * Returns the constant density rho of the given polyhedron.
+         * The unit must match to the mesh, e.g., mesh in @f$[m]@f$ requires density in @f$[kg/m^3]@f$.
          * The density is required for the calculation.
          * @return density as double
          */
         virtual double getDensity() = 0;
 
         /**
          * The vector contains the points for which the polyhedral gravity model should
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/input/TetgenAdapter.cpp` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/TetgenAdapter.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #include "TetgenAdapter.h"
 
 namespace polyhedralGravity {
 
-    Polyhedron TetgenAdapter::getPolyhedron() {
+    std::tuple<std::vector<Array3>, std::vector<IndexArray3>> TetgenAdapter::getPolyhedralSource() {
         //1. Step: Read in from files
         for (const auto &fileName: _fileNames) {
             size_t pos = fileName.find_last_of('.');
             std::string name = fileName.substr(0, pos);
             std::string suffix = fileName.substr(pos + 1);
             _suffixToOperation.at(suffix)(name);
         }
 
         //2. Convert tetgenio to Polyhedron
-        return {_vertices, _faces};
+        return std::make_tuple(_vertices, _faces);
     }
 
     void TetgenAdapter::readNode(const std::string &filename) {
         SPDLOG_LOGGER_DEBUG(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger() , "Reading the file {}.node", filename);
         this->checkIntegrity(filename, 'v');
         try {
             _tetgenio.load_node(const_cast<char *>(filename.c_str()));
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/input/TetgenAdapter.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/TetgenAdapter.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 /**
  * An adapter to the Tetgen Library. This is the interface between tetgen's data structures and I/O
  * capabilities and the here implemented polyhedral gravity model.
  * The adapter always converts tetgen's datastructure into the structure utilized by the Polyhedral Gravity Model.
  *
  * The Adapter further keeps en eye on the already read in files in order to give feedback if data is in conflict.
  */
-    class TetgenAdapter : public DataSource {
+    class TetgenAdapter final : public DataSource {
 
         /**
          * The default exception message
          */
         static constexpr char DEFAULT_EXCEPTION_MSG[] =
                 "The mesh was not read because of an error in Tetgen! This could indicate several "
                 "issues, e. g. issues with the node assignment like they appear if either no nodes were "
@@ -53,30 +53,30 @@
         std::vector<std::array<size_t, 3>> _faces;
 
     public:
 
         /**
          * Constructs a new TetgenAdapter from a vector of filenames. These filenames should end on the supported
          * suffixes
-         * @param fileNames - vector of filenames
+         * @param fileNames vector of filenames
          */
         explicit TetgenAdapter(std::vector<std::string> fileNames)
                 : _tetgenio{},
                   _fileNames{std::move(fileNames)},
                   _vertices{},
                   _faces{} {};
 
         /**
          * Use this function to get a Polyhedron.
          * This functions consists of two steps. First, the Adapter will delegate I/O to the tetgen library and
          * read in the Polyhedron data in the library's datastructure. Second, tetgen's datastructure is then
          * converted to a Polyhedron.
          * @return a Polyhedron
          */
-        Polyhedron getPolyhedron() override;
+        std::tuple<std::vector<Array3>, std::vector<IndexArray3>> getPolyhedralSource() override;
 
         /**
          * Reads nodes from a .node file
          * @param filename of the input source without suffix
          * @throws an exception if the nodes already have been defined
          */
         void readNode(const std::string &filename);
@@ -130,16 +130,16 @@
                 {"ply",  [this](const std::string &name) { this->readPly(name); }},
                 {"stl",  [this](const std::string &name) { this->readStl(name); }},
                 {"mesh", [this](const std::string &name) { this->readMesh(name); }}
         };
 
         /**
          * Checks if the polyhedron is integer and not already defined by other properties
-         * @param filename - string with the current read file, for more detailed exceptions
-         * @param what - what to check: f = faces, v = vertices, a = all
+         * @param filename string with the current read file, for more detailed exceptions
+         * @param what what to check: f = faces, v = vertices, a = all
          * @throws an exception if not
          */
         void checkIntegrity(const std::string &filename, char what) const;
 
         /**
          * Adds the Vertices of the tetgenio structure to the resulting polyhedron's vertices.
          */
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/input/YAMLConfigReader.cpp` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/YAMLConfigReader.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     bool YAMLConfigReader::getMeshInputCheckStatus() {
         SPDLOG_LOGGER_DEBUG(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger() ,
                             "Reading the activation of the input mesh sanity check from the configuration file.");
         if (_file[ROOT][INPUT] && _file[ROOT][INPUT][INPUT_CHECK]) {
             return _file[ROOT][INPUT][INPUT_CHECK].as<bool>();
         } else {
-            return false;
+            return true;
         }
     }
 
     std::shared_ptr<DataSource> YAMLConfigReader::getDataSource() {
         SPDLOG_LOGGER_DEBUG(PolyhedralGravityLogger::DEFAULT_LOGGER.getLogger() ,
                             "Reading the data sources (file names) from the configuration file.");
         if (_file[ROOT][INPUT] && _file[ROOT][INPUT][INPUT_POLYHEDRON]) {
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/input/YAMLConfigReader.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/input/YAMLConfigReader.h`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 namespace polyhedralGravity {
 
     /**
      * The YAMLConfigReader serves as Interface between yaml-cpp and the Polyhedral Gravity Model and
      * reads in the input from an yaml configuration file.
      */
-    class YAMLConfigReader : public ConfigSource {
+    class YAMLConfigReader final : public ConfigSource {
 
         /*
          * The following static variables contain the names of the YAML nodes.
          * Note: C++20 would allow constexpr std::string which would be more appropriate instead of char[]
          */
         static constexpr char ROOT[] = "gravityModel";
         static constexpr char INPUT[] = "input";
@@ -34,27 +34,27 @@
          */
         const YAML::Node _file;
 
     public:
 
         /**
          * Creates a new YAML Config Reader.
-         * @param filename - a reference to a string
+         * @param filename a reference to a string
          * @throws an exception if the file is malformed or cannot be loaded or if the ROOT node is not found
          */
         explicit YAMLConfigReader(const std::string &filename)
                 : _file{YAML::LoadFile(filename)} {
             if (!_file[ROOT]) {
                 throw std::runtime_error{"The YAML file does not contain a specification for the \"gravityModel\"!"};
             }
         }
 
         /**
          * Creates a new YAML Config Reader.
-         * @param filename - a movable string
+         * @param filename a movable string
          * @throws an exception if the file is malformed or cannot be loaded or if the ROOT node is not found
          */
         explicit YAMLConfigReader(std::string &&filename)
                 : _file{YAML::LoadFile(filename)} {
             if (!_file[ROOT]) {
                 throw std::runtime_error{"The YAML file does not contain a specification for the \"gravityModel\"!"};
             }
@@ -77,15 +77,15 @@
          * Reads the computation points from the yaml configuration file.
          * @return vector of computation points
          */
         std::vector<std::array<double, 3>> getPointsOfInterest() override;
 
         /**
          * Reads the enablement of the input sanity check from the yaml file.
-         * @return true if explicitly enabled, otherwise per-default false
+         * @return true or false if explicitly enabled, otherwise per-default true
          */
         bool getMeshInputCheckStatus() override;
 
         /**
          * Reads the DataSource from the yaml configuration file.
          * @return shared_ptr to the DataSource Object created
          */
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/model/GravityModelData.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/model/GravityModelData.h`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
      *
      * The second order derivatives or also called gradiometric Tensor in [1/s^2].
      * The array contains the second order derivatives in the following order xx, yy, zz, xy, xz, yz.
      * @related Equation (3) and (13) of Tsoulis Paper, here referred as Vxx, Vyy, Vzz, Vxy, Vxz, Vyz
      */
     using GravityModelResult = std::tuple<double, Array3, Array6>;
 
+
     /**
      * Contains the 3D distances l1_pq and l2_pq between P and the endpoints of segment pq and
      * the 1D distances s1_pq and s2_pq between P'' and the segment endpoints.
      * @note This struct is basically a named tuple
      */
     struct Distance {
         /**
@@ -73,39 +74,39 @@
          * line segment pq
          */
         double s2;
 
         /**
          * Checks two Distance structs for equality.
          * @warning This method compares doubles! So only exact copies will evaluate to true.
-         * @param rhs - the other Distance struct
+         * @param rhs the other Distance struct
          * @return true if equal
          *
          * @note Just used for testing purpose
          */
         bool operator==(const Distance &rhs) const {
             return l1 == rhs.l1 && l2 == rhs.l2 && s1 == rhs.s1 && s2 == rhs.s2;
         }
 
         /**
          * Checks two Distance structs for inequality.
          * @warning This method compares doubles! So only exact copies will evaluate to false.
-         * @param rhs - the other Distance struct
+         * @param rhs the other Distance struct
          * @return false if unequal
          *
          * @note Just used for testing purpose
          */
         bool operator!=(const Distance &rhs) const {
             return !(rhs == *this);
         }
 
         /**
          * Pretty prints this struct on the given ostream.
-         * @param os - ostream
-         * @param distance - a Distance struct
+         * @param os ostream
+         * @param distance a Distance struct
          * @return os
          */
         friend std::ostream &operator<<(std::ostream &os, const Distance &distance) {
             os << "l1: " << distance.l1 << " l2: " << distance.l2 << " s1: " << distance.s1 << " s2: " << distance.s2;
             return os;
         }
     };
@@ -127,39 +128,39 @@
          * @note see Tsoulis Paper Equation (15)
          */
         double an;
 
         /**
          * Checks two TranscendentalExpressions for equality.
          * @warning This method compares doubles! So only exact copies will evaluate to true.
-         * @param rhs - the other TranscendentalExpressions
+         * @param rhs the other TranscendentalExpressions
          * @return true if equal
          *
          * @note Just used for testing purpose
          */
         bool operator==(const TranscendentalExpression &rhs) const {
             return ln == rhs.ln && an == rhs.an;
         }
 
         /**
          * Checks two TranscendentalExpressions for inequality.
          * @warning This method compares doubles! So only exact copies will evaluate to false.
-         * @param rhs - the other TranscendentalExpressions
+         * @param rhs the other TranscendentalExpressions
          * @return false if unequal
          *
          * @note Just used for testing purpose
          */
         bool operator!=(const TranscendentalExpression &rhs) const {
             return !(rhs == *this);
         }
 
         /**
          * Pretty output of this struct on the given ostream.
-         * @param os - the ostream
-         * @param expression - a TranscendentalExpression
+         * @param os the ostream
+         * @param expression a TranscendentalExpression
          * @return os
          */
         friend std::ostream &operator<<(std::ostream &os, const TranscendentalExpression &expression) {
             os << "ln: " << expression.ln << " an: " << expression.an;
             return os;
         }
     };
@@ -188,27 +189,27 @@
          * the signed distance to the plane from the origin along the normal
          */
         double d;
 
         /**
          * Checking the equality of two this Hessian Plane with another one by comparing their members.
          * @warning This method compares doubles! So only exact copies will evaluate to true.
-         * @param rhs - other HessianPlane
+         * @param rhs other HessianPlane
          * @return true if equal
          *
          * @note Just used for testing purpose
          */
         bool operator==(const HessianPlane &rhs) const {
             return a == rhs.a && b == rhs.b && c == rhs.c && d == rhs.d;
         }
 
         /**
          * Checking the inequality of two this Hessian Plane with another one by comparing their members.
          * @warning This method compares doubles! So only exact copies will evaluate to false.
-         * @param rhs - other HessianPlane
+         * @param rhs other HessianPlane
          * @return true if unequal
          *
          * @note Just used for testing purpose
          */
         bool operator!=(const HessianPlane &rhs) const {
             return !(rhs == *this);
         }
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/output/CSVWriter.cpp` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/CSVWriter.cpp`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/output/CSVWriter.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/CSVWriter.h`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
          * Results are written to "polyhedralGravityModel.csv".
          */
         CSVWriter() : CSVWriter("polyhedralGravityModel.csv") {}
 
         /**
          * Creates a new CSVWriter.
          * Results are written to file with filename as name.
-         * @param filename - a string
+         * @param filename a string
          */
         explicit CSVWriter(const std::string &filename)
                 : _logger{
                 spdlog::basic_logger_mt<spdlog::synchronous_factory>("CSVWriter_" + filename, filename, true)} {
             _logger->set_pattern("%v");
         }
 
@@ -48,16 +48,16 @@
          */
         ~CSVWriter() {
             spdlog::drop(_logger->name());
         }
 
         /**
          * Prints the result to the specified file
-         * @param computationPoints - vector of computation points
-         * @param gravityResults - vector of gravity results
+         * @param computationPoints vector of computation points
+         * @param gravityResults vector of gravity results
          */
         void printResult(const std::vector<std::array<double, 3>> &computationPoints,
                          const std::vector<GravityModelResult> &gravityResults) const;
 
     };
 
 }
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/output/Logging.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/output/Logging.h`

 * *Files identical despite different names*

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/util/UtilityConstants.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/util/UtilityConstants.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,13 @@
     /**
      * The gravitational constant G in [m^3/(kg*s^2)].
      * @related in his paper above Equation (4)
      */
     constexpr double GRAVITATIONAL_CONSTANT = 6.67430e-11;
 
     /**
-     * The assumed constant density rho for a polyhedron after Tsoulis paper in [kg/m^3].
+     * The assumed constant density rho for a polyhedron after Tsoulis paper in @f$[kg/m^3]@f$.
      * @related in his paper above Equation (4)
      */
     constexpr double DEFAULT_CONSTANT_DENSITY = 2670.0;
 
 }
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/util/UtilityContainer.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/util/UtilityContainer.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 #pragma once
 
 #include <array>
+#include <set>
 #include <numeric>
 #include <utility>
 #include <algorithm>
 #include <functional>
 #include <cmath>
 #include <string>
 #include <iostream>
 
 namespace polyhedralGravity::util {
 
     /**
      * Alias for two-dimensional array with size M and N.
      * M is the major size.
      */
-    template<typename T, size_t M, size_t N> using Matrix = std::array<std::array<T, N>, M>;
+    template<typename T, size_t M, size_t N>
+    using Matrix = std::array<std::array<T, N>, M>;
 
     /**
      * Applies a binary function to elements of two containers piece by piece. The objects must
      * be iterable and should have the same size!
-     * @tparam Container - an iterable object like an array or vector
-     * @tparam BinOp - a binary function to apply
-     * @param lhs - the first container
-     * @param rhs - the second container
-     * @param binOp - a binary function like +, -, *, /
+     * @tparam Container an iterable object like an array or vector
+     * @tparam BinOp a binary function to apply
+     * @param lhs the first container
+     * @param rhs the second container
+     * @param binOp a binary function like +, -, *, /
      * @return a container containing the result
      */
     template<typename Container, typename BinOp>
     Container applyBinaryFunction(const Container &lhs, const Container &rhs, BinOp binOp) {
         Container ret = lhs;
         std::transform(std::begin(lhs), std::end(lhs), std::begin(rhs), std::begin(ret), binOp);
         return ret;
     }
 
     /**
      * Applies a binary function to elements of one container piece by piece. The objects must
      * be iterable. The resulting container consist of the containers' object after the application
      * of the binary function with the scalar as parameter.
-     * @tparam Container - a iterable object like an array or vector
-     * @tparam Scalar - a scalar to use on each element
-     * @tparam BinOp - a binary function to apply
-     * @param lhs - the first container
-     * @param scalar - a scalar to use on each element
-     * @param binOp - a binary function like +, -, *, /
+     * @tparam Container a iterable object like an array or vector
+     * @tparam Scalar a scalar to use on each element
+     * @tparam BinOp a binary function to apply
+     * @param lhs the first container
+     * @param scalar a scalar to use on each element
+     * @param binOp a binary function like +, -, *, /
      * @return a container containing the result
      */
     template<typename Container, typename Scalar, typename BinOp>
     Container applyBinaryFunction(const Container &lhs, const Scalar &scalar, BinOp binOp) {
         Container ret = lhs;
         std::transform(std::begin(lhs), std::end(lhs), std::begin(ret), [&binOp, &scalar](const Scalar &element) {
             return binOp(element, scalar);
@@ -55,164 +57,164 @@
         return ret;
     }
 
     /**
      * Applies the Operation Minus to two Containers piece by piece.
      * @example {1, 2, 3} - {1, 1, 1} = {0, 1, 2}
      * @tparam Container
-     * @param lhs - minuend
-     * @param rhs - subtrahend
+     * @param lhs minuend
+     * @param rhs subtrahend
      * @return the difference
      */
     template<typename Container>
     Container operator-(const Container &lhs, const Container &rhs) {
         return applyBinaryFunction(lhs, rhs, std::minus<>());
     }
 
     /**
     * Applies the Operation Plus to two Containers piece by piece.
     * @example {1, 2, 3} + {1, 1, 1} = {2, 3, 4}
     * @tparam Container
-    * @param lhs - addend
-    * @param rhs - addend
+    * @param lhs addend
+    * @param rhs addend
     * @return the sum
     */
     template<typename Container>
     Container operator+(const Container &lhs, const Container &rhs) {
         return applyBinaryFunction(lhs, rhs, std::plus<>());
     }
 
     /**
     * Applies the Operation * to two Containers piece by piece.
     * @example {1, 2, 3} * {2, 2, 2} = {2, 4, 6}
     * @tparam Container
-    * @param lhs - multiplicand
-    * @param rhs - multiplicand
+    * @param lhs multiplicand
+    * @param rhs multiplicand
     * @return the product
     */
     template<typename Container>
     Container operator*(const Container &lhs, const Container &rhs) {
         return applyBinaryFunction(lhs, rhs, std::multiplies<>());
     }
 
     /**
     * Applies the Operation / to two Containers piece by piece.
     * @example {1, 2, 3} * {1, 2, 3} = {1, 1, 1}
     * @tparam Container
-    * @param lhs - multiplicand
-    * @param rhs - multiplicand
+    * @param lhs multiplicand
+    * @param rhs multiplicand
     * @return the product
     */
     template<typename Container>
     Container operator/(const Container &lhs, const Container &rhs) {
         return applyBinaryFunction(lhs, rhs, std::divides<>());
     }
 
     /**
     * Applies the Operation + to a Container and a Scalar.
     * @example {1, 2, 3} + 2 = {3, 4, 5}
     * @tparam Container
     * @tparam Scalar
-    * @param lhs - addend
-    * @param scalar - addend
+    * @param lhs addend
+    * @param scalar addend
     * @return a Container
     */
     template<typename Container, typename Scalar>
     Container operator+(const Container &lhs, const Scalar &scalar) {
         return applyBinaryFunction(lhs, scalar, std::plus<>());
     }
 
     /**
-    * Applies the Operation - to a Container and a Scalar.
-    * @example {1, 2, 3} - 2 = {-1, 0, 1}
+    * Applies the Operation to a Container and a Scalar.
+    * @example {1, 2, 3} 2 = {-1, 0, 1}
     * @tparam Container
     * @tparam Scalar
-    * @param lhs - minuend
-    * @param scalar - subtrahend
+    * @param lhs minuend
+    * @param scalar subtrahend
     * @return a Container
      * TODO This method causes issues with the MVSC 19.31.31107.0? Although it is never used...
     */
-//    template<typename Container, typename Scalar>
-//    Container operator-(const Container &lhs, const Scalar &scalar) {
-//        return applyBinaryFunction(lhs, scalar, std::minus<>());
-//    }
+    //    template<typename Container, typename Scalar>
+    //    Container operator-(const Container &lhs, const Scalar &scalar) {
+    //        return applyBinaryFunction(lhs, scalar, std::minus<>());
+    //    }
 
     /**
-    * Applies the Operation - to a Container and a Scalar.
+    * Applies the Operation to a Container and a Scalar.
     * @example {1, 2, 3} * 2 = {2, 4, 6}
     * @tparam Container
     * @tparam Scalar
-    * @param lhs - multiplicand
-    * @param scalar - multiplicand
+    * @param lhs multiplicand
+    * @param scalar multiplicand
     * @return a Container
     */
     template<typename Container, typename Scalar>
     Container operator*(const Container &lhs, const Scalar &scalar) {
         return applyBinaryFunction(lhs, scalar, std::multiplies<>());
     }
 
     /**
      * Applies the Operation / to a Container and a Scalar.
      * @example {2, 4, 6} / 2 = {1, 2, 3}
      * @tparam Container
      * @tparam Scalar
-     * @param lhs - the dividend
-     * @param scalar - the divisor
+     * @param lhs the dividend
+     * @param scalar the divisor
      * @return a Container
      */
     template<typename Container, typename Scalar>
     Container operator/(const Container &lhs, const Scalar &scalar) {
         return applyBinaryFunction(lhs, scalar, std::divides<>());
     }
 
     /**
      * Applies the euclidean norm/ L2-norm to a Container (e.g. a vector)
-     * @tparam Container - must be iterable
-     * @param container - e.g. a vector
+     * @tparam Container must be iterable
+     * @param container e.g. a vector
      * @return an double containing the L2 norm
      */
     template<typename Container>
     double euclideanNorm(const Container &container) {
         return std::sqrt(std::inner_product(std::begin(container), std::end(container), std::begin(container), 0.0));
     }
 
     /**
      * Computes the absolute value for each value in the given container
-     * @tparam Container - a iterable container, containing numerical values
-     * @param container - the container
+     * @tparam Container a iterable container, containing numerical values
+     * @param container the container
      * @return a container with the modified values
      */
     template<typename Container>
     Container abs(const Container &container) {
         Container ret = container;
         std::transform(std::begin(container), std::end(container), std::begin(ret),
                        [](const auto &element) { return std::abs(element); });
         return ret;
     }
 
     /**
      * Computes the determinant with the Sarrus rule for a 3x3 matrix.
      * Notice that for square matrices det(A) = det(A^T).
-     * @tparam T - a numerical value
-     * @param matrix - the 3x3 matrix
+     * @tparam T a numerical value
+     * @param matrix the 3x3 matrix
      * @return the determinant
      */
     template<typename T>
     T det(const Matrix<T, 3, 3> &matrix) {
         return matrix[0][0] * matrix[1][1] * matrix[2][2] + matrix[0][1] * matrix[1][2] * matrix[2][0] +
                matrix[0][2] * matrix[1][0] * matrix[2][1] - matrix[0][2] * matrix[1][1] * matrix[2][0] -
                matrix[0][0] * matrix[1][2] * matrix[2][1] - matrix[0][1] * matrix[1][0] * matrix[2][2];
     }
 
     /**
      * Computes the transposed of a mxn matrix.
-     * @tparam T - the type of the matrix elements
-     * @tparam M - the row number
-     * @tparam N - the column number
-     * @param matrix - the matrix to transpose
+     * @tparam T the type of the matrix elements
+     * @tparam M the row number
+     * @tparam N the column number
+     * @param matrix the matrix to transpose
      * @return the transposed
      */
     template<typename T, size_t M, size_t N>
     Matrix<T, M, N> transpose(const Matrix<T, M, N> &matrix) {
         Matrix<T, N, M> transposed;
         for (size_t i = 0; i < M; ++i) {
             for (size_t j = 0; j < N; ++j) {
@@ -220,74 +222,74 @@
             }
         }
         return transposed;
     }
 
     /**
     * Returns the cross product of two cartesian vectors.
-    * @tparam T - a number
-    * @param lhs - left vector
-    * @param rhs - right vector
+    * @tparam T a number
+    * @param lhs left vector
+    * @param rhs right vector
     * @return cross product
     */
     template<typename T>
     std::array<T, 3> cross(const std::array<T, 3> &lhs, const std::array<T, 3> &rhs) {
         std::array<T, 3> result{};
         result[0] = lhs[1] * rhs[2] - lhs[2] * rhs[1];
         result[1] = lhs[2] * rhs[0] - lhs[0] * rhs[2];
         result[2] = lhs[0] * rhs[1] - lhs[1] * rhs[0];
         return result;
     }
 
     /**
      * Calculates the normal N as (first * second) / |first * second| with * being the cross product and first, second
      * as cartesian vectors.
-     * @tparam T - numerical type
-     * @param first - first cartesian vector
-     * @param second - second cartesian vector
+     * @tparam T numerical type
+     * @param first first cartesian vector
+     * @param second second cartesian vector
      * @return the normal (normed)
      */
     template<typename T>
     std::array<T, 3> normal(const std::array<T, 3> &first, const std::array<T, 3> &second) {
         const std::array<T, 3> crossProduct = cross(first, second);
         const double norm = euclideanNorm(crossProduct);
         return crossProduct / norm;
     }
 
     /**
     * Returns the dot product of two cartesian vectors.
-    * @tparam T - a number
-    * @param lhs - left vector
-    * @param rhs - right vector
+    * @tparam T a number
+    * @param lhs left vector
+    * @param rhs right vector
     * @return dot product
     */
     template<typename T>
     T dot(const std::array<T, 3> &lhs, const std::array<T, 3> &rhs) {
         return lhs[0] * rhs[0] + lhs[1] * rhs[1] + lhs[2] * rhs[2];
     }
 
     /**
      * Implements the signum function with a certain EPSILON to absorb rounding errors.
-     * @tparam T - a numerical (floating point) value
-     * @param val - the value itself
-     * @param cutoffEpsilon - the cut-off radius around zero to return 0
+     * @tparam T a numerical (floating point) value
+     * @param val the value itself
+     * @param cutoffEpsilon the cut-off radius around zero to return 0
      * @return -1, 0, 1 depending on the sign an the given EPSILON
      */
     template<typename T>
     int sgn(T val, double cutoffEpsilon) {
         return val < -cutoffEpsilon ? -1 : val > cutoffEpsilon ? 1 : 0;
     }
 
     /**
      * Concatenates two std::array of different sizes to one array.
-     * @tparam T - the shared type of the arrays
-     * @tparam M - the size of the first container
-     * @tparam N  - the size of the second container
-     * @param first - the first array
-     * @param second - the second array
+     * @tparam T the shared type of the arrays
+     * @tparam M the size of the first container
+     * @tparam N  the size of the second container
+     * @param first the first array
+     * @param second the second array
      * @return a new array of size M+N with type T
      */
     template<typename T, size_t M, size_t N>
     std::array<T, M + N> concat(const std::array<T, M> &first, const std::array<T, N> &second) {
         std::array<T, M + N> result{};
         size_t index = 0;
         for (const auto &el: first) {
@@ -297,87 +299,131 @@
             result[index++] = el;
         }
         return result;
     }
 
     /**
      * Calculates the surface area of a triangle consisting of three cartesian vertices.
-     * @tparam T - numerical type
+     * @tparam T numerical type
      * @return surface area
      */
     template<typename T>
     T surfaceArea(const Matrix<T, 3, 3> &triangle) {
         return 0.5 * euclideanNorm(cross(triangle[1] - triangle[0], triangle[2] - triangle[0]));
     }
 
     /**
      * Calculates the magnitude between two values and return true if the magnitude
      * between the exponents in greater than 17.
-     * @tparam T - numerical type
-     * @param first - first number
-     * @param second - second number
+     * @tparam T numerical type
+     * @param first first number
+     * @param second second number
      * @return true if the difference is too be huge, so that floating point absorption will happen
      */
     template<typename T>
     bool isCriticalDifference(const T &first, const T &second) {
         // 50 is the (log2) exponent of the floating point (1 / 1e-15)
         constexpr int maxExponentDifference = 50;
         int x, y;
         std::frexp(first, &x);
         std::frexp(second, &y);
         return std::abs(x - y) > maxExponentDifference;
     }
 
+    /**
+    * A utility struct that creates an overload set out of all the function objects it inherits from.
+    * It allows a lambda function to be used with std::visit in a variant.
+    * The lambda function needs to be able to handle all types contained in the variant,
+    * and this struct allows it to do so by inheriting the function-call operator from each type.
+    * @tparam Ts A template parameter pack representing all types for which the struct should be able to handle.
+    *
+    * @ref https://en.cppreference.com/w/cpp/utility/variant/visit
+    */
+    template<class... Ts>
+    struct overloaded : Ts... {
+        using Ts::operator()...;
+    };
+
+    /**
+    * This function template provides deduction guides for the overloaded struct.
+    * It deduces the template arguments for overloaded based on its constructor arguments
+    * thus saving you from explicitly mentioning them while instantiation.
+    * @tparam Ts A template parameter pack representing all types that will be passed to the overloaded struct.
+    * @param Ts Variable numbers of parameters to pass to the overloaded struct.
+    * @return This doesn't return a value, but rather assists in the creation of an overloaded object.
+    *          The type of the object will be overloaded<Ts...>.
+    *
+    * @ref https://en.cppreference.com/w/cpp/utility/variant/visit
+    */
+    template<class... Ts>
+    overloaded(Ts...) -> overloaded<Ts...>;
+
     namespace detail {
 
         /**
          * Helper method for the tuple operator+, which expands the tuple into a parameter pack.
-         * @tparam Ts - types of the tuple
-         * @tparam Is - indices of the tuple
-         * @param t1 - first tuple
-         * @param t2 - second tuple
+         * @tparam Ts types of the tuple
+         * @tparam Is indices of the tuple
+         * @param t1 first tuple
+         * @param t2 second tuple
          * @return a new tuple with the added values
          */
         template<typename... Ts, size_t... Is>
         auto tuple_add(const std::tuple<Ts...> &t1, const std::tuple<Ts...> &t2, std::index_sequence<Is...>) {
             return std::make_tuple(std::get<Is>(t1) + std::get<Is>(t2)...);
         }
 
     }
 
     /**
      * Adds the contents of two tuples of the same size and types with the operator +.
-     * @tparam Ts - types of the tuples
-     * @param t1 - first tuple
-     * @param t2 - second tuple
+     * @tparam Ts types of the tuples
+     * @param t1 first tuple
+     * @param t2 second tuple
      * @return a new tuple with the added values
      */
     template<typename... Ts>
     auto operator+(const std::tuple<Ts...> &t1, const std::tuple<Ts...> &t2) {
         return detail::tuple_add(t1, t2, std::index_sequence_for<Ts...>{});
     }
 
     /**
      * Operator << for an array of any size.
-     * @tparam T - type of the array, must have an << operator overload
-     * @tparam N - size of the array
-     * @param os - the ostream
-     * @param array - the array itself
+     * @tparam T type of the array, must have an << operator overload
+     * @tparam N size of the array
+     * @param os the ostream
+     * @param array the array itself
      * @return ostream
      */
     template<typename T, size_t N>
     std::ostream &operator<<(std::ostream &os, const std::array<T, N> &array) {
-        os << "[";
-        auto it = array.begin();
-        auto end = array.end() - 1;
-        while (it != end) {
-            os << *it << " ";
-            ++it;
-        }
-        os << *it << "]";
+        os.operator<<('[');
+        os.operator<<(' ');
+        std::for_each(array.cbegin(), array.cend(), [&os](const auto& arg) {
+            os << arg << ' ';
+        });
+        os.operator<<(']');
+        return os;
+    }
+
+    /**
+     * Operator << for a set.
+     * @tparam T type of the set, must have an << operator overload
+     * @param os the ostream
+     * @param set the set itself
+     * @return ostream
+     */
+    template<typename T>
+    std::ostream &operator<<(std::ostream &os, const std::set<T> &set) {
+        os.operator<<('[');
+        os.operator<<(' ');
+        std::for_each(set.cbegin(), set.cend(), [&os](const auto& arg) {
+            os << arg << ' ';
+        });
+        os.operator<<(']');
         return os;
     }
 
     template<typename T>
     struct is_stdarray : std::false_type {
     };
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravity/util/UtilityThrust.h` & `polyhedral_gravity-3.0rc3/src/polyhedralGravity/util/UtilityThrust.h`

 * *Files 3% similar despite different names*

```diff
@@ -3,49 +3,49 @@
 #include <utility>
 #include "thrust/iterator/zip_iterator.h"
 
 namespace polyhedralGravity::util {
 
     /**
      * Returns a zip iterator for a pack of Iterators
-     * @tparam Iterator - should be a iterator
-     * @param args - can be any number of iterators
+     * @tparam Iterator should be a iterator
+     * @param args can be any number of iterators
      * @return a thrust::zip_iterator
      */
     template<typename ...Iterator>
     auto zip(const Iterator&... args) {
         return thrust::make_zip_iterator(thrust::make_tuple(args...));
     }
 
     /**
      * Returns a zip iterator for a pack of Containers
-     * @tparam Container - should be a container on which one can call std::begin()
-     * @param args - can be any number of containers
+     * @tparam Container should be a container on which one can call std::begin()
+     * @param args can be any number of containers
      * @return a thrust::zip_iterator for the beginning of all containers
      */
     template<typename ...Container>
     auto zipBegin(const Container&... args) {
         return zip(std::begin(args)...);
     }
 
     /**
      * Returns a zip iterator for a pack of Containers
-     * @tparam Container - should be a container on which one can call std::end()
-     * @param args - can be any number of containers
+     * @tparam Container should be a container on which one can call std::end()
+     * @param args can be any number of containers
      * @return a thrust::zip_iterator for the end of all containers
      */
     template<typename ...Container>
     auto zipEnd(const Container&... args) {
         return zip(std::end(args)...);
     }
 
     /**
      * Returns a zip iterator pair for a pack of Containers
-     * @tparam Container - should be a container on which one can call std::begin() and std::end()
-     * @param args - can be any number of containers
+     * @tparam Container should be a container on which one can call std::begin() and std::end()
+     * @param args can be any number of containers
      * @return a pair of thrust::zip_iterator for the beginning and end of all containers
      */
     template<typename ...Container>
     auto zipPair(const Container&... args) {
         auto begin = zipBegin(args...);
         auto end = zipEnd(args...);
         return std::make_pair(begin, end);
```

### Comparing `polyhedral_gravity-2.1/src/polyhedralGravityPython/CMakeLists.txt` & `polyhedral_gravity-3.0rc3/src/polyhedralGravityPython/CMakeLists.txt`

 * *Files identical despite different names*

