# Comparing `tmp/xmipy-1.4.0.tar.gz` & `tmp/xmipy-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmipy-1.4.0.tar", last modified: Tue Sep 19 08:34:48 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `xmipy-1.4.0.tar` & `xmipy-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-09-19 08:34:48.869450 xmipy-1.4.0/
--rw-rw-rw-   0        0        0     7169 2023-03-23 10:39:36.000000 xmipy-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     2039 2023-09-19 08:34:48.867342 xmipy-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      887 2023-03-23 10:39:36.000000 xmipy-1.4.0/README.md
--rw-rw-rw-   0        0        0     1741 2023-09-19 08:21:24.000000 xmipy-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-19 08:34:48.869772 xmipy-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0       96 2023-03-23 10:39:36.000000 xmipy-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-19 08:34:48.843267 xmipy-1.4.0/tests/
--rw-rw-rw-   0        0        0     3313 2023-09-19 08:21:24.000000 xmipy-1.4.0/tests/test_logger.py
--rw-rw-rw-   0        0        0    13035 2023-06-01 14:45:07.000000 xmipy-1.4.0/tests/test_mf6_dis_bmi.py
--rw-rw-rw-   0        0        0      501 2023-09-19 08:21:24.000000 xmipy-1.4.0/tests/test_mf6_dis_errors.py
--rw-rw-rw-   0        0        0     1216 2023-06-01 14:45:07.000000 xmipy-1.4.0/tests/test_mf6_dis_utils.py
--rw-rw-rw-   0        0        0     1620 2023-06-01 14:45:07.000000 xmipy-1.4.0/tests/test_mf6_dis_xmi.py
--rw-rw-rw-   0        0        0     2329 2023-06-01 14:45:07.000000 xmipy-1.4.0/tests/test_mf6_disu_bmi.py
--rw-rw-rw-   0        0        0     1298 2023-06-01 14:45:07.000000 xmipy-1.4.0/tests/test_timers.py
--rw-rw-rw-   0        0        0     1818 2023-09-19 08:21:24.000000 xmipy-1.4.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-09-19 08:34:48.852269 xmipy-1.4.0/xmipy/
--rw-rw-rw-   0        0        0      175 2023-09-19 08:34:14.000000 xmipy-1.4.0/xmipy/__init__.py
--rw-rw-rw-   0        0        0      349 2023-03-23 10:39:36.000000 xmipy-1.4.0/xmipy/errors.py
--rw-rw-rw-   0        0        0     1933 2023-09-19 08:21:24.000000 xmipy-1.4.0/xmipy/logger.py
-drwxrwxrwx   0        0        0        0 2023-09-19 08:34:48.864875 xmipy-1.4.0/xmipy/timers/
--rw-rw-rw-   0        0        0        0 2023-03-23 10:39:36.000000 xmipy-1.4.0/xmipy/timers/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-03-23 10:39:36.000000 xmipy-1.4.0/xmipy/timers/timer.py
--rw-rw-rw-   0        0        0     2813 2023-03-23 10:39:36.000000 xmipy-1.4.0/xmipy/timers/timers.py
--rw-rw-rw-   0        0        0     1397 2023-09-19 08:21:24.000000 xmipy-1.4.0/xmipy/utils.py
--rw-rw-rw-   0        0        0     4803 2023-09-19 08:21:24.000000 xmipy-1.4.0/xmipy/xmi.py
--rw-rw-rw-   0        0        0    25697 2023-09-19 08:34:14.000000 xmipy-1.4.0/xmipy/xmiwrapper.py
-drwxrwxrwx   0        0        0        0 2023-09-19 08:34:48.860345 xmipy-1.4.0/xmipy.egg-info/
--rw-rw-rw-   0        0        0     2039 2023-09-19 08:34:48.000000 xmipy-1.4.0/xmipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-09-19 08:34:48.000000 xmipy-1.4.0/xmipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-19 08:34:48.000000 xmipy-1.4.0/xmipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-09-19 08:34:48.000000 xmipy-1.4.0/xmipy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       98 2023-09-19 08:34:48.000000 xmipy-1.4.0/xmipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-09-19 08:34:48.000000 xmipy-1.4.0/xmipy.egg-info/top_level.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 xmipy-1.5.0/.coveragerc
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xmipy-1.5.0/.typos.toml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 xmipy-1.5.0/codecov.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 xmipy-1.5.0/guide-to-publish.md
+-rw-r--r--   0        0        0   541146 2020-02-02 00:00:00.000000 xmipy-1.5.0/pixi.lock
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 xmipy-1.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 xmipy-1.5.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 xmipy-1.5.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 xmipy-1.5.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_logger.py
+-rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_mf6_dis_bmi.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_mf6_dis_errors.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_mf6_dis_utils.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_mf6_dis_xmi.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_mf6_disu_bmi.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_timers.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 xmipy-1.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/errors.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/py.typed
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/utils.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/xmi.py
+-rw-r--r--   0        0        0    27529 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/xmiwrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/timers/__init__.py
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/timers/timer.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 xmipy-1.5.0/xmipy/timers/timers.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 xmipy-1.5.0/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 xmipy-1.5.0/LICENSE
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 xmipy-1.5.0/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 xmipy-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xmipy-1.5.0/PKG-INFO
```

### Comparing `xmipy-1.4.0/LICENSE` & `xmipy-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/PKG-INFO` & `xmipy-1.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-Metadata-Version: 2.1
-Name: xmipy
-Version: 1.4.0
-Summary: xmipy is an extension to the bmipy Python package
-Author-email: Martijn Russcher <Martijn.Russcher@deltares.nl>, Julian Hofer <Julian.Hofer@deltares.nl>, "Joseph D. Hughes" <jdhughes@usgs.gov>
-License: CC0
-Project-URL: Documentation, https://deltares.github.io/xmipy/xmipy.html
-Project-URL: Source, https://github.com/Deltares/xmipy
-Keywords: BMI,Basic Model Interface
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: bmipy
-Requires-Dist: numpy
-Provides-Extra: tests
-Requires-Dist: flopy>=3.3.6; extra == "tests"
-Requires-Dist: pytest; extra == "tests"
-Requires-Dist: pytest-cov; extra == "tests"
-Requires-Dist: requests; extra == "tests"
-Provides-Extra: lint
-Requires-Dist: black; extra == "lint"
-Requires-Dist: ruff; extra == "lint"
-Requires-Dist: mypy; extra == "lint"
-Provides-Extra: docs
-Requires-Dist: pdoc; extra == "docs"
-
-# xmipy
-
-![Continuous integration](https://github.com/Deltares/xmipy/workflows/Continuous%20integration/badge.svg)
-[![codecov](https://codecov.io/gh/Deltares/xmipy/branch/develop/graph/badge.svg)](https://codecov.io/gh/Deltares/xmipy)
-
-
-`xmipy` is an extension to [bmipy](https://pypi.org/project/bmipy/) including an implementation of the abstract methods.
-The extended interface is required to couple certain hydrological kernels, particularly MODFLOW 6. Currently it is a joint development of the USGS and Deltares. The [imod_coupler](https://github.com/Deltares/imod_coupler) uses it, for example, to couple Modflow 6 and MetaSWAP.
-
-`xmipy` can be installed by running
-```
-pip install xmipy
-```
-
-# Contributing
-
-In order to develop on `xmipy` locally, execute the following line inside your virtual environment
-
-```bash
-pip install -e ".[tests, lint, docs]"
-```
+Metadata-Version: 2.3
+Name: xmipy
+Version: 1.5.0
+Summary: xmipy is an extension to the bmipy Python package
+Project-URL: Documentation, https://deltares.github.io/xmipy/xmipy.html
+Project-URL: Source, https://github.com/Deltares/xmipy
+Author-email: Martijn Russcher <Martijn.Russcher@deltares.nl>, Julian Hofer <Julian.Hofer@deltares.nl>, "Joseph D. Hughes" <jdhughes@usgs.gov>
+License: CC0
+License-File: LICENSE
+Keywords: BMI,Basic Model Interface
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Requires-Python: >=3.9
+Requires-Dist: bmipy
+Requires-Dist: numpy
+Provides-Extra: docs
+Requires-Dist: pdoc; extra == 'docs'
+Provides-Extra: lint
+Requires-Dist: mypy; extra == 'lint'
+Requires-Dist: ruff; extra == 'lint'
+Provides-Extra: tests
+Requires-Dist: flopy>=3.3.6; extra == 'tests'
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-cov; extra == 'tests'
+Requires-Dist: requests; extra == 'tests'
+Description-Content-Type: text/markdown
+
+# xmipy
+
+![Continuous integration](https://github.com/Deltares/xmipy/workflows/Continuous%20integration/badge.svg)
+[![codecov](https://codecov.io/gh/Deltares/xmipy/branch/develop/graph/badge.svg)](https://codecov.io/gh/Deltares/xmipy)
+
+
+`xmipy` is an extension to [bmipy](https://pypi.org/project/bmipy/) including an implementation of the abstract methods.
+The extended interface is required to couple certain hydrological kernels, particularly MODFLOW 6. Currently it is a joint development of the USGS and Deltares. The [imod_coupler](https://github.com/Deltares/imod_coupler) uses it, for example, to couple MODFLOW 6 and MetaSWAP.
+
+`xmipy` can be downloaded from [conda-forge](https://anaconda.org/conda-forge/xmipy) or [PyPI](https://pypi.org/project/xmipy/).
+
+# Contributing
+
+In order to develop on `xmipy`, you have to download pixi.
+Pixi can be downloaded at [pixi.sh](https://pixi.sh/latest/).
+
+In order to run the test suite, execute:
+
+```bash
+pixi run tests
+```
```

### Comparing `xmipy-1.4.0/README.md` & `xmipy-1.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # xmipy
 
 ![Continuous integration](https://github.com/Deltares/xmipy/workflows/Continuous%20integration/badge.svg)
 [![codecov](https://codecov.io/gh/Deltares/xmipy/branch/develop/graph/badge.svg)](https://codecov.io/gh/Deltares/xmipy)
 
 
 `xmipy` is an extension to [bmipy](https://pypi.org/project/bmipy/) including an implementation of the abstract methods.
-The extended interface is required to couple certain hydrological kernels, particularly MODFLOW 6. Currently it is a joint development of the USGS and Deltares. The [imod_coupler](https://github.com/Deltares/imod_coupler) uses it, for example, to couple Modflow 6 and MetaSWAP.
+The extended interface is required to couple certain hydrological kernels, particularly MODFLOW 6. Currently it is a joint development of the USGS and Deltares. The [imod_coupler](https://github.com/Deltares/imod_coupler) uses it, for example, to couple MODFLOW 6 and MetaSWAP.
 
-`xmipy` can be installed by running
-```
-pip install xmipy
-```
+`xmipy` can be downloaded from [conda-forge](https://anaconda.org/conda-forge/xmipy) or [PyPI](https://pypi.org/project/xmipy/).
 
 # Contributing
 
-In order to develop on `xmipy` locally, execute the following line inside your virtual environment
+In order to develop on `xmipy`, you have to download pixi.
+Pixi can be downloaded at [pixi.sh](https://pixi.sh/latest/).
+
+In order to run the test suite, execute:
 
 ```bash
-pip install -e ".[tests, lint, docs]"
+pixi run tests
 ```
```

### Comparing `xmipy-1.4.0/tests/test_logger.py` & `xmipy-1.5.0/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
-import os.path
+from pathlib import Path
 
 import xmipy.logger
 from xmipy import XmiWrapper
 
 
 def test_logger_defaults(caplog, modflow_lib_path):
     mf6 = XmiWrapper(modflow_lib_path)
 
     assert mf6.logger.level == logging.NOTSET
-    assert mf6.logger.name == os.path.basename(modflow_lib_path)
+    assert mf6.logger.name == Path(modflow_lib_path).name
 
     mf6.logger.debug("not shown")
     assert len(caplog.record_tuples) == 0
 
     mf6.logger.info("also not shown")
     assert len(caplog.record_tuples) == 0
```

### Comparing `xmipy-1.4.0/tests/test_mf6_dis_bmi.py` & `xmipy-1.5.0/tests/test_mf6_dis_bmi.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,24 +122,14 @@
 def test_get_var_stringarray(flopy_dis_mf6):
     flopy_dis, mf6 = flopy_dis_mf6
     mf6.initialize()
 
     # boundary names are not set until _rp, so we need this update()
     mf6.update()
 
-    bnd_name_tag = mf6.get_var_address("BOUNDNAME_CST", flopy_dis.model_name, "CHD_0")
-    var_shape = mf6.get_var_shape(bnd_name_tag)
-    assert var_shape == [2]
-
-    var_nbytes = mf6.get_var_nbytes(bnd_name_tag)
-    assert var_nbytes == 2 * 40  # NB: LENBOUNDNAME = 40
-    ilen = var_nbytes // var_shape[0]
-    assert mf6.get_var_type(bnd_name_tag) == f"STRING LEN={ilen} (2)"
-    assert mf6.get_value(bnd_name_tag).tolist() == ["BNDA", "BNDB"]
-
     # test var with rank 1 and shape [0]
     name_tag = mf6.get_var_address("AUXNAME_CST", flopy_dis.model_name, "CHD_0")
     assert mf6.get_var_rank(name_tag) == 1
     assert mf6.get_var_shape(name_tag) == [0]
     assert mf6.get_var_nbytes(name_tag) == 0
     assert mf6.get_var_type(name_tag) == "STRING LEN=16 (0)"
     assert mf6.get_value(name_tag).tolist() == []
@@ -357,18 +347,15 @@
 
 
 def test_get_grid_rank(flopy_dis_mf6):
     """Tests if the the grid rank can be extracted"""
     flopy_dis, mf6 = flopy_dis_mf6
     mf6.initialize()
 
-    if flopy_dis.nlay == 1:
-        prescribed_grid_rank = 2
-    else:
-        prescribed_grid_rank = 3
+    prescribed_grid_rank = 2 if flopy_dis.nlay == 1 else 3
 
     # Getting the grid id from the model, requires specifying one variable
     k11_tag = mf6.get_var_address("K11", flopy_dis.model_name, "NPF")
     grid_id = mf6.get_var_grid(k11_tag)
 
     assert prescribed_grid_rank == mf6.get_grid_rank(grid_id)
```

### Comparing `xmipy-1.4.0/tests/test_mf6_dis_utils.py` & `xmipy-1.5.0/tests/test_mf6_dis_utils.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/tests/test_mf6_dis_xmi.py` & `xmipy-1.5.0/tests/test_mf6_dis_xmi.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     mf6 = flopy_dis_mf6[1]
     mf6.initialize()
 
     # Prepare solve
     mf6.prepare_solve(*sol_id)
 
     max_iter = 25
-    for kiter in range(max_iter):
+    for _ in range(max_iter):
         has_converged = mf6.solve(*sol_id)
 
         if has_converged:
             break
 
     assert has_converged
```

### Comparing `xmipy-1.4.0/tests/test_mf6_disu_bmi.py` & `xmipy-1.5.0/tests/test_mf6_disu_bmi.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/tests/test_timers.py` & `xmipy-1.5.0/tests/test_timers.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/tests/test_utils.py` & `xmipy-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/xmipy/logger.py` & `xmipy-1.5.0/xmipy/logger.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/xmipy/timers/timer.py` & `xmipy-1.5.0/xmipy/timers/timer.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/xmipy/timers/timers.py` & `xmipy-1.5.0/xmipy/timers/timers.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/xmipy/utils.py` & `xmipy-1.5.0/xmipy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,11 @@
         elif isinstance(arg, ctypes._SimpleCData):
             return repr(arg)
         else:
             return repr(arg)
 
     items = []
     for arg in args:
-        if hasattr(arg, "_obj"):
-            # Format byref() with "&" prefix
-            item = "&" + format_arg(arg._obj)
-        else:
-            item = format_arg(arg)
+        # Format byref() with "&" prefix
+        item = "&" + format_arg(arg._obj) if hasattr(arg, "_obj") else format_arg(arg)
         items.append(item)
     return f"{function}({', '.join(items)})"
```

### Comparing `xmipy-1.4.0/xmipy/xmi.py` & `xmipy-1.5.0/xmipy/xmi.py`

 * *Files identical despite different names*

### Comparing `xmipy-1.4.0/xmipy/xmiwrapper.py` & `xmipy-1.5.0/xmipy/xmiwrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     c_char_p,
     c_double,
     c_int,
     c_void_p,
     create_string_buffer,
 )
 from enum import Enum, IntEnum, unique
+from os import PathLike
 from pathlib import Path
 from typing import Any, Callable, Tuple, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from xmipy.errors import InputError, TimerError, XMIError
@@ -39,45 +40,80 @@
 
 
 class XmiWrapper(Xmi):
     """The implementation of the XMI"""
 
     def __init__(
         self,
-        lib_path: Union[str, Path],
-        lib_dependency: Union[str, Path, None] = None,
-        working_directory: Union[str, Path, None] = None,
+        lib_path: Union[str, PathLike[Any]],
+        lib_dependency: Union[str, PathLike[Any], None] = None,
+        working_directory: Union[str, PathLike[Any], None] = None,
         timing: bool = False,
         logger_level: Union[str, int] = 0,
     ):
-        """Constructor
+        """
+        Constructor of `XmiWrapper`
+
+        Next to wrapping C functions of a library exposing XMI,
+        it also adds timing and logging functionality.
+        An example for logging can be seen below.
+
+        ```
+        In [1]: from xmipy import XmiWrapper
+
+        In [2]: mf6 = XmiWrapper("/path/to/libmf6.so", working_directory="/path/to/sim", logger_level="DEBUG")
+
+        In [3]: mf6.initialize()
+        DEBUG:libmf6.so: execute function: initialize(b'') returned 0
+
+        In [4]: mf6.get_start_time()
+        DEBUG:libmf6.so: execute function: get_start_time(&c_double(0.0)) returned 0
+        Out[4]: 0.0
+
+        In [5]: mf6.get_end_time()
+        DEBUG:libmf6.so: execute function: get_end_time(&c_double(504.0)) returned 0
+        Out[5]: 504.0
+
+        In [6]: mf6.get_grid_rank(1)
+        DEBUG:libmf6.so: execute function: get_grid_rank(&c_int(1), &c_int(2)) returned 0
+        Out[6]: 2
+
+        In [7]: mf6.get_value('SLN_1/MXITER')
+        DEBUG:libmf6.so: execute function: get_var_rank(c_char_p(b'SLN_1/MXITER'), &c_int(0)) returned 0
+        DEBUG:libmf6.so: execute function: get_var_type(c_char_p(b'SLN_1/MXITER'), &c_char_Array_51(b'INTEGER')) returned 0
+        DEBUG:libmf6.so: execute function: get_var_type(c_char_p(b'SLN_1/MXITER'), &c_char_Array_51(b'INTEGER')) returned 0
+        DEBUG:libmf6.so: execute function: get_value_ptr_int(c_char_p(b'SLN_1/MXITER'), &ndpointer_<i4_1d_1_C) returned 0
+        DEBUG:libmf6.so: execute function: get_var_type(c_char_p(b'SLN_1/MXITER'), &c_char_Array_51(b'INTEGER')) returned 0
+        DEBUG:libmf6.so: execute function: get_value_ptr_int(c_char_p(b'SLN_1/MXITER'), &ndpointer_<i4_1d_1_C) returned 0
+        Out[7]: array([25], dtype=int32)
+        ```
 
         Parameters
         ----------
-        lib_path : Union[str, Path]
+        lib_path : Union[str, PathLike]
             Path to the shared library
 
-        lib_dependency : Union[str, Path, None], optional
+        lib_dependency : Union[str, PathLike, None], optional
             Path to the dependencies of the shared library, by default None
 
-        working_directory : Union[str, Path, None], optional
+        working_directory : Union[str, PathLike, None], optional
             The working directory the shared library expects when being called,
             by default None
 
         timing : bool, optional
             Whether timing should be activated, by default False
 
         logger_level : str, int, optional
             Logger level, default 0 ("NOTSET"). Accepted values are
             "DEBUG" (10), "INFO" (20), "WARNING" (30), "ERROR" (40) or
             "CRITICAL" (50).
         """
 
         self._state = State.UNINITIALIZED
-        self.libname = os.path.basename(lib_path)
+        self.libname = Path(lib_path).name
         self.logger = get_logger(self.libname, logger_level)
 
         if lib_dependency:
             self._add_lib_dependency(lib_dependency)
         # LoadLibraryEx flag (py38+): LOAD_WITH_ALTERED_SEARCH_PATH 0x08
         # -> uses the altered search path for resolving dll dependencies
         # `winmode` has no effect while running on Linux or macOS
@@ -98,15 +134,15 @@
             )
 
     def __del__(self) -> None:
         if self._state == State.INITIALIZED:
             self.finalize()
 
     @staticmethod
-    def _add_lib_dependency(lib_dependency: Union[str, Path]) -> None:
+    def _add_lib_dependency(lib_dependency: Union[str, PathLike[Any]]) -> None:
         lib_dependency = str(Path(lib_dependency).absolute())
         if platform.system() == "Windows":
             os.environ["PATH"] = lib_dependency + os.pathsep + os.environ["PATH"]
         else:
             # Assume a Unix-like system
             if "LD_LIBRARY_PATH" in os.environ:
                 os.environ["LD_LIBRARY_PATH"] = (
@@ -132,18 +168,18 @@
         c_var = c_int.in_dll(self.lib, name)
         return c_var.value
 
     def set_int(self, name: str, value: int) -> None:
         c_var = c_int.in_dll(self.lib, name)
         c_var.value = value
 
-    def initialize(self, config_file: str = "") -> None:
+    def initialize(self, config_file: Union[str, PathLike[Any]] = "") -> None:
         if self._state == State.UNINITIALIZED:
             with cd(self.working_directory):
-                self._execute_function(self.lib.initialize, config_file.encode())
+                self._execute_function(self.lib.initialize, os.fsencode(config_file))
                 self._state = State.INITIALIZED
         else:
             raise InputError("The library is already initialized")
 
     def initialize_mpi(self, value: int) -> None:
         if self._state == State.UNINITIALIZED:
             with cd(self.working_directory):
@@ -315,17 +351,16 @@
     def get_time_units(self) -> str:
         raise NotImplementedError
 
     def get_value(
         self, name: str, dest: Union[NDArray[Any], None] = None
     ) -> NDArray[Any]:
         # make sure that optional array is of correct layout:
-        if dest is not None:
-            if not dest.flags["C"]:
-                raise InputError("Array should have C layout")
+        if dest is not None and not dest.flags["C"]:
+            raise InputError("Array should have C layout")
 
         # first deal with scalars
         rank = self.get_var_rank(name)
         var_type = self.get_var_type(name)
         var_type_lower = var_type.lower()
 
         if rank == 0:
```

