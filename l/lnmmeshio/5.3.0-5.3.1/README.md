# Comparing `tmp/lnmmeshio-5.3.0.tar.gz` & `tmp/lnmmeshio-5.3.1.tar.gz`

## Comparing `lnmmeshio-5.3.0.tar` & `lnmmeshio-5.3.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/.isort.cfg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/pytest.ini
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/requirements-dev.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/requirements.txt
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/.github/workflows/build_and_test.yml
--rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/__init__.py
--rw-r--r--   0        0        0    11170 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/discretization.py
--rw-r--r--   0        0        0    13496 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/ensightio.py
--rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/fiber.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/ioutils.py
--rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/meshio_to_discretization.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/mimics_stlio.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/node.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/nodeset.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/progress.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/__init__.py
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/element.py
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/element_container.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/hex20.py
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/hex27.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/hex8.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/line2.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/line3.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/parse_element.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/pyramid5.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/quad4.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/quad8.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/quad9.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/tet10.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/tet4.py
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/tri3.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/tri6.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/vertex.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/element/wedge6.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/functions/__init__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/functions/component.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/functions/function.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/functions/linear_interpolation_variable.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/functions/variable.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/src/lnmmeshio/functions/variablereader.py
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_disc.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_discretization.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_ele_container.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_element_factory.py
--rw-r--r--   0        0        0    20936 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_eles.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_ensight.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_fibers.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_integration.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_meshio2discretization.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_mimics_stlio.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_override.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/test_write_data.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/data/cube.mesh
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/data/cube.stl
--rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/data/dummy.dat
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/data/dummy.mesh
--rw-r--r--   0        0        0   928184 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/data/dummy.stl
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/data/dummy2.dat
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/test_lnmmeshio/data/full.dat
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/LICENSE
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lnmmeshio-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.isort.cfg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/pytest.ini
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/requirements-dev.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/requirements.txt
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.github/workflows/build_and_test.yml
+-rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/__init__.py
+-rw-r--r--   0        0        0    11170 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/discretization.py
+-rw-r--r--   0        0        0    13496 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/ensightio.py
+-rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/fiber.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/ioutils.py
+-rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/meshio_to_discretization.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/mimics_stlio.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/node.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/nodeset.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/progress.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/__init__.py
+-rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/element.py
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/element_container.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/hex20.py
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/hex27.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/hex8.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/line2.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/line3.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/parse_element.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/pyramid5.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/quad4.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/quad8.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/quad9.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tet10.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tet4.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tri3.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tri6.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/vertex.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/wedge6.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/__init__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/component.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/function.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/linear_interpolation_variable.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/variable.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/variablereader.py
+-rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_disc.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_discretization.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_ele_container.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_element_factory.py
+-rw-r--r--   0        0        0    20936 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_eles.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_ensight.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_fibers.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_integration.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_meshio2discretization.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_mimics_stlio.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_override.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_write_data.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/cube.mesh
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/cube.stl
+-rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.dat
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.mesh
+-rw-r--r--   0        0        0   928184 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.stl
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy2.dat
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/full.dat
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/LICENSE
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/PKG-INFO
```

### Comparing `lnmmeshio-5.3.0/.github/workflows/build_and_test.yml` & `lnmmeshio-5.3.1/.github/workflows/build_and_test.yml`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/__init__.py` & `lnmmeshio-5.3.1/src/lnmmeshio/__init__.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/discretization.py` & `lnmmeshio-5.3.1/src/lnmmeshio/discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/ensightio.py` & `lnmmeshio-5.3.1/src/lnmmeshio/ensightio.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/fiber.py` & `lnmmeshio-5.3.1/src/lnmmeshio/fiber.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/ioutils.py` & `lnmmeshio-5.3.1/src/lnmmeshio/ioutils.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/meshio_to_discretization.py` & `lnmmeshio-5.3.1/src/lnmmeshio/meshio_to_discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/mimics_stlio.py` & `lnmmeshio-5.3.1/src/lnmmeshio/mimics_stlio.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This file is mainly based on the stl-reader by meshio (https://github.com/nschloe/meshio).
 
 Copyright (c) 2015-2021 Nico Schlömer et al.
 
 I/O for the STL format, cf.
 <https://en.wikipedia.org/wiki/STL_(file_format)>.
 """
+
 import io
 import logging
 import struct
 
 import numpy
 from meshio import Mesh
```

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/node.py` & `lnmmeshio-5.3.1/src/lnmmeshio/node.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/nodeset.py` & `lnmmeshio-5.3.1/src/lnmmeshio/nodeset.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/progress.py` & `lnmmeshio-5.3.1/src/lnmmeshio/progress.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/element.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/element.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/element_container.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/element_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,34 @@
     Class holding all elements in different categories. Current implemented categories are
 
     ElementContainer.structure
     ElementContainer.fluid
     ElementContainer.ale
     ElementContainer.transport
     ElementContainer.thermo
+    ElementContainer.artery
     """
 
     TypeStructure: str = "structure"
     TypeFluid: str = "fluid"
     TypeALE: str = "ale"
     TypeTransport: str = "transport"
     TypeThermo: str = "thermo"
+    TypeArtery: str = "artery"
 
     def __init__(self):
         """
         Initialize element contained
         """
         self.structure: Optional[List[Element]] = None
         self.fluid: Optional[List[Element]] = None
         self.ale: Optional[List[Element]] = None
         self.transport: Optional[List[Element]] = None
         self.thermo: Optional[List[Element]] = None
+        self.artery: Optional[List[Element]] = None
 
     def get_num_structure(self) -> int:
         """
         Returns the number of structural elements in the discretization
 
         Returns:
             int: Number of structural parameters in the discretization
@@ -91,14 +94,26 @@
             int: Number of thermo parameters in the discretization
         """
         if self.thermo is None:
             return 0
 
         return len(self.thermo)
 
+    def get_num_artery(self) -> int:
+        """
+        Returns the number of artery elements in the discretization
+
+        Returns:
+            int: Number of artery parameters in the discretization
+        """
+        if self.artery is None:
+            return 0
+
+        return len(self.artery)
+
     def write(self, dest):
         """
         Write the corresponding sections into the stream like variable dest
 
         Args:
             dest: Stream like variable, where to write the corresponding sections
         """
@@ -113,23 +128,26 @@
 
         if self.transport is not None:
             ElementContainer.__write_section(dest, "TRANSPORT ELEMENTS", self.transport)
 
         if self.thermo is not None:
             ElementContainer.__write_section(dest, "THERMO ELEMENTS", self.thermo)
 
+        if self.artery is not None:
+            ElementContainer.__write_section(dest, "ARTERY ELEMENTS", self.artery)
+
     def get_sections(self, out=True):
         """
         Returns an ordereddict of sections with the corresponding lines
         """
         d = OrderedDict()
         for key, elements in self.items():
-            d[
-                ElementContainer.get_section_name(key)
-            ] = ElementContainer.__get_section_lines(elements, out=out)
+            d[ElementContainer.get_section_name(key)] = (
+                ElementContainer.__get_section_lines(elements, out=out)
+            )
 
         return d
 
     def values(self):
         """
         Returns a list of List[Elements] for the different element types
 
@@ -144,14 +162,16 @@
             ele_list.append(self.fluid)
         if self.ale is not None:
             ele_list.append(self.ale)
         if self.transport is not None:
             ele_list.append(self.transport)
         if self.thermo is not None:
             ele_list.append(self.thermo)
+        if self.artery is not None:
+            ele_list.append(self.artery)
 
         return ele_list
 
     def items(self):
         """
         Returns a list of tuples with key and values for each element type
 
@@ -175,14 +195,16 @@
             ele_keys.append(self.TypeFluid)
         if self.ale is not None:
             ele_keys.append(self.TypeALE)
         if self.transport is not None:
             ele_keys.append(self.TypeTransport)
         if self.thermo is not None:
             ele_keys.append(self.TypeThermo)
+        if self.artery is not None:
+            ele_keys.append(self.TypeArtery)
 
         return ele_keys
 
     def __getitem__(self, key):
         """
         Returns the list of elements belonging to a type of discretization
 
@@ -198,14 +220,16 @@
             return self.fluid
         elif key == self.TypeALE and self.ale is not None:
             return self.ale
         elif key == self.TypeTransport and self.transport is not None:
             return self.transport
         elif key == self.TypeThermo and self.thermo is not None:
             return self.thermo
+        elif key == self.TypeArtery and self.artery is not None:
+            return self.artery
 
         raise KeyError("Key not found: {0}".format(key))
 
     def __contains__(self, key):
         """
         Returns the a boolean, whether the field type is available
 
@@ -221,14 +245,16 @@
             return True
         elif key == self.TypeALE and self.ale is not None:
             return True
         elif key == self.TypeTransport and self.transport is not None:
             return True
         elif key == self.TypeThermo and self.thermo is not None:
             return True
+        elif key == self.TypeArtery and self.artery is not None:
+            return True
 
         return False
 
     def __setitem__(self, key, value):
         """
         Returns the list of elements belonging to a type of discretization
 
@@ -242,14 +268,16 @@
             self.fluid = value
         elif key == self.TypeALE:
             self.ale = value
         elif key == self.TypeTransport:
             self.transport = value
         elif key == self.TypeThermo:
             self.thermo = value
+        elif key == self.TypeArtery:
+            self.artery = value
         else:
             raise KeyError("Key not found: {0}".format(key))
 
     @staticmethod
     def __write_section(dest, section_name: str, elements: List[Element]):
         """
         Writes the element section with section title and elements. If elements is None,
@@ -313,14 +341,19 @@
             )
 
         if "THERMO ELEMENTS" in sections:
             elec.thermo = ElementContainer.__read_elements(
                 nodes, sections["THERMO ELEMENTS"], out=out, fieldtype="Thermo elements"
             )
 
+        if "ARTERY ELEMENTS" in sections:
+            elec.thermo = ElementContainer.__read_elements(
+                nodes, sections["ARTERY ELEMENTS"], out=out, fieldtype="Artery elements"
+            )
+
         return elec
 
     @staticmethod
     def __read_elements(nodes: List[Node], lines: List[str], out=False, fieldtype=None):
         """
         Static method that reads the list of elements
 
@@ -371,7 +404,9 @@
             return "FLUID ELEMENTS"
         if fieldtype == ElementContainer.TypeALE:
             return "ALE ELEMENTS"
         if fieldtype == ElementContainer.TypeTransport:
             return "TRANSPORT ELEMENTS"
         if fieldtype == ElementContainer.TypeThermo:
             return "THERMO ELEMENTS"
+        if fieldtype == ElementContainer.TypeArtery:
+            return "ARTERY ELEMENTS"
```

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/hex20.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/hex20.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/hex27.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/hex27.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/hex8.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/hex8.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/line2.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/line2.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/line3.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/line3.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/parse_element.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/parse_element.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/pyramid5.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/pyramid5.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/quad4.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/quad4.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/quad8.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/quad8.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/quad9.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/quad9.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/tet10.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/tet10.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/tet4.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/tet4.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/tri3.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/tri3.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/tri6.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/tri6.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/vertex.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/vertex.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/element/wedge6.py` & `lnmmeshio-5.3.1/src/lnmmeshio/element/wedge6.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/functions/component.py` & `lnmmeshio-5.3.1/src/lnmmeshio/functions/component.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/functions/function.py` & `lnmmeshio-5.3.1/src/lnmmeshio/functions/function.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/functions/linear_interpolation_variable.py` & `lnmmeshio-5.3.1/src/lnmmeshio/functions/linear_interpolation_variable.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/src/lnmmeshio/functions/variablereader.py` & `lnmmeshio-5.3.1/src/lnmmeshio/functions/variablereader.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_disc.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_disc.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_discretization.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_ele_container.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_ele_container.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,20 +14,22 @@
         c = ElementContainer()
 
         self.assertFalse(ElementContainer.TypeStructure in c)
         self.assertFalse(ElementContainer.TypeFluid in c)
         self.assertFalse(ElementContainer.TypeALE in c)
         self.assertFalse(ElementContainer.TypeTransport in c)
         self.assertFalse(ElementContainer.TypeThermo in c)
+        self.assertFalse(ElementContainer.TypeArtery in c)
 
         self.assertRaises(KeyError, lambda: c[ElementContainer.TypeStructure])
         self.assertRaises(KeyError, lambda: c[ElementContainer.TypeFluid])
         self.assertRaises(KeyError, lambda: c[ElementContainer.TypeALE])
         self.assertRaises(KeyError, lambda: c[ElementContainer.TypeTransport])
         self.assertRaises(KeyError, lambda: c[ElementContainer.TypeThermo])
+        self.assertRaises(KeyError, lambda: c[ElementContainer.TypeArtery])
         self.assertRaises(KeyError, lambda: c["doesnotexist"])
         with self.assertRaises(KeyError) as _:
             c["doesnotexist"] = 1
 
         c[ElementContainer.TypeStructure] = [1]
         self.assertListEqual(c[ElementContainer.TypeStructure], [1])
         self.assertListEqual(c.structure, [1])
@@ -44,12 +46,17 @@
         self.assertListEqual(c[ElementContainer.TypeTransport], [4])
         self.assertListEqual(c.transport, [4])
 
         c[ElementContainer.TypeThermo] = [5]
         self.assertListEqual(c[ElementContainer.TypeThermo], [5])
         self.assertListEqual(c.thermo, [5])
 
+        c[ElementContainer.TypeArtery] = [5]
+        self.assertListEqual(c[ElementContainer.TypeArtery], [5])
+        self.assertListEqual(c.artery, [5])
+
         self.assertTrue(ElementContainer.TypeStructure in c)
         self.assertTrue(ElementContainer.TypeFluid in c)
         self.assertTrue(ElementContainer.TypeALE in c)
         self.assertTrue(ElementContainer.TypeTransport in c)
         self.assertTrue(ElementContainer.TypeThermo in c)
+        self.assertTrue(ElementContainer.TypeArtery in c)
```

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_element_factory.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_element_factory.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_eles.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_eles.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_ensight.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_ensight.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_fibers.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_fibers.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_integration.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_integration.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_meshio2discretization.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_meshio2discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_mimics_stlio.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_mimics_stlio.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_override.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_override.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/test_write_data.py` & `lnmmeshio-5.3.1/test_lnmmeshio/test_write_data.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/data/cube.stl` & `lnmmeshio-5.3.1/test_lnmmeshio/data/cube.stl`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/data/dummy.dat` & `lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.dat`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/data/dummy.stl` & `lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.stl`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/data/dummy2.dat` & `lnmmeshio-5.3.1/test_lnmmeshio/data/dummy2.dat`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/test_lnmmeshio/data/full.dat` & `lnmmeshio-5.3.1/test_lnmmeshio/data/full.dat`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/LICENSE` & `lnmmeshio-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/README.md` & `lnmmeshio-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.0/pyproject.toml` & `lnmmeshio-5.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lnmmeshio"
-version = "5.3.0"
+version = "5.3.1"
 authors = [
   { name="Amadeus Gebauer", email="amadeus.gebauer@tum.de" },
 ]
 description = "Import and export from and to various mesh formats including dat files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lnmmeshio-5.3.0/PKG-INFO` & `lnmmeshio-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lnmmeshio
-Version: 5.3.0
+Version: 5.3.1
 Summary: Import and export from and to various mesh formats including dat files
 Project-URL: Homepage, https://github.com/amgebauer/lnmmeshio
 Project-URL: Bug Tracker, https://github.com/amgebauer/lnmmeshio/issues
 Author-email: Amadeus Gebauer <amadeus.gebauer@tum.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

