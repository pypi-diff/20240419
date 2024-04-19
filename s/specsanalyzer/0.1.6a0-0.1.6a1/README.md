# Comparing `tmp/specsanalyzer-0.1.6a0.tar.gz` & `tmp/specsanalyzer-0.1.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsanalyzer-0.1.6a0.tar", max compression
+gzip compressed data, was "specsanalyzer-0.1.6a1.tar", max compression
```

## Comparing `specsanalyzer-0.1.6a0.tar` & `specsanalyzer-0.1.6a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1067 2024-04-05 11:47:33.377485 specsanalyzer-0.1.6a0/LICENSE
--rw-r--r--   0        0        0     4279 2024-04-05 11:47:33.377485 specsanalyzer-0.1.6a0/README.md
--rw-r--r--   0        0        0     2631 2024-04-05 11:47:57.769663 specsanalyzer-0.1.6a0/pyproject.toml
--rwxr-xr-x   0        0        0      145 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/__init__.py
--rw-r--r--   0        0        0      695 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/config/default.yaml
--rwxr-xr-x   0        0        0      411 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/config/phoibos150.calib2d
--rwxr-xr-x   0        0        0     8973 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/config.py
--rwxr-xr-x   0        0        0    19345 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/convert.py
--rwxr-xr-x   0        0        0    22117 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/core.py
--rwxr-xr-x   0        0        0     4103 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/img_tools.py
--rwxr-xr-x   0        0        0    18805 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsanalyzer/io.py
--rwxr-xr-x   0        0        0      133 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/__init__.py
--rwxr-xr-x   0        0        0    15200 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/config/NXmpes_arpes_config.json
--rw-r--r--   0        0        0      556 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/config/default.yaml
--rw-r--r--   0        0        0     3434 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/config/example_config_FHI.yaml
--rwxr-xr-x   0        0        0    21413 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/core.py
--rw-r--r--   0        0        0    20070 2024-04-05 11:47:33.381485 specsanalyzer-0.1.6a0/specsscan/helpers.py
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a0/setup.py
--rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a0/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/LICENSE
+-rw-r--r--   0        0        0     4279 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/README.md
+-rw-r--r--   0        0        0     2631 2024-04-19 19:39:30.235787 specsanalyzer-0.1.6a1/pyproject.toml
+-rwxr-xr-x   0        0        0      145 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/config/default.yaml
+-rwxr-xr-x   0        0        0      411 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/config/phoibos150.calib2d
+-rwxr-xr-x   0        0        0     8973 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/config.py
+-rwxr-xr-x   0        0        0    19345 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/convert.py
+-rwxr-xr-x   0        0        0    29609 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/core.py
+-rwxr-xr-x   0        0        0     4250 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/img_tools.py
+-rwxr-xr-x   0        0        0    18805 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/io.py
+-rwxr-xr-x   0        0        0      133 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/__init__.py
+-rwxr-xr-x   0        0        0    15200 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/config/NXmpes_arpes_config.json
+-rw-r--r--   0        0        0      556 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/config/default.yaml
+-rw-r--r--   0        0        0     3347 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/config/example_config_FHI.yaml
+-rwxr-xr-x   0        0        0    22754 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/core.py
+-rw-r--r--   0        0        0    20015 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/helpers.py
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a1/setup.py
+-rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a1/PKG-INFO
```

### Comparing `specsanalyzer-0.1.6a0/LICENSE` & `specsanalyzer-0.1.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/README.md` & `specsanalyzer-0.1.6a1/README.md`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/pyproject.toml` & `specsanalyzer-0.1.6a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "specsanalyzer"
 packages = [
     {include = "specsanalyzer"},
     {include = "specsscan"},
 ]
-version = "0.1.6a0"
+version = "0.1.6a1"
 description = "Python package for loading and converting SPECS Phoibos analyzer data."
 authors = [
     "Laurenz Rettig <rettig@fhi-berlin.mpg.de>",
     "Michele Puppin <michele.puppin@epfl.ch>",
     "Abeer Arora <arora@fhi-berlin.mpg.de>",
 ]
 readme = "README.md"
```

### Comparing `specsanalyzer-0.1.6a0/specsanalyzer/config/default.yaml` & `specsanalyzer-0.1.6a1/specsanalyzer/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/specsanalyzer/config.py` & `specsanalyzer-0.1.6a1/specsanalyzer/config.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/specsanalyzer/convert.py` & `specsanalyzer-0.1.6a1/specsanalyzer/convert.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/specsanalyzer/img_tools.py` & `specsanalyzer-0.1.6a1/specsanalyzer/img_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,39 +57,41 @@
 
     Returns:
         np.ndarray: The chosen image data. Default is the filtered real image.
     """
 
     # Do Fourier Transform of the (real-valued) image
     image_fft = np.fft.rfft2(image)
+    # shift fft axis to have 0 in the center
+    image_fft = np.fft.fftshift(image_fft, axes=0)
     mask = np.ones(image_fft.shape)
     xgrid, ygrid = np.meshgrid(
         range(image_fft.shape[0]),
         range(image_fft.shape[1]),
         indexing="ij",
         sparse=True,
     )
     for peak in peaks:
         try:
             mask -= peak["amplitude"] * gauss2d(
                 xgrid,
                 ygrid,
-                peak["pos_x"],
+                image_fft.shape[0] / 2 + peak["pos_x"],
                 peak["pos_y"],
                 peak["sigma_x"],
                 peak["sigma_y"],
             )
         except KeyError as exc:
             raise KeyError(
                 f"The peaks input is supposed to be a list of dicts with the "
                 "following structure: pos_x, pos_y, sigma_x, sigma_y, amplitude.",
             ) from exc
 
     # apply mask to the FFT, and transform back
-    filtered = np.fft.irfft2(image_fft * mask)
+    filtered = np.fft.irfft2(np.fft.ifftshift(image_fft * mask, axes=0))
     # strip negative values
     filtered = filtered.clip(min=0)
     if ret == "filtered":
         return filtered
     if ret == "fft":
         return image_fft
     if ret == "mask":
```

### Comparing `specsanalyzer-0.1.6a0/specsanalyzer/io.py` & `specsanalyzer-0.1.6a1/specsanalyzer/io.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/specsscan/config/NXmpes_arpes_config.json` & `specsanalyzer-0.1.6a1/specsscan/config/NXmpes_arpes_config.json`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/specsscan/config/default.yaml` & `specsanalyzer-0.1.6a1/specsscan/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a0/specsscan/config/example_config_FHI.yaml` & `specsanalyzer-0.1.6a1/specsscan/config/example_config_FHI.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -87,31 +87,26 @@
   fft_filter_peaks:
     - amplitude: 1
       pos_x: 79
       pos_y: 0
       sigma_x: 8
       sigma_y: 8
     - amplitude: 1
-      pos_x: 176
+      pos_x: -80
       pos_y: 0
       sigma_x: 8
       sigma_y: 8
     - amplitude: 1
       pos_x: 0
       pos_y: 109
       sigma_x: 5
       sigma_y: 8
     - amplitude: 1
       pos_x: 78
       pos_y: 109
       sigma_x: 5
       sigma_y: 5
     - amplitude: 1
-      pos_x: 175
+      pos_x: -81
       pos_y: 108
       sigma_x: 5
       sigma_y: 5
-    - amplitude: 1
-      pos_x: 254
-      pos_y: 109
-      sigma_x: 5
-      sigma_y: 8
```

### Comparing `specsanalyzer-0.1.6a0/specsscan/core.py` & `specsanalyzer-0.1.6a1/specsscan/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,28 +220,38 @@
                 ),
             )
             if dim in ["polar", "tilt", "azimuth"]:
                 res_xarray = res_xarray.transpose("Angle", dim, "Ekin")
             else:
                 res_xarray = res_xarray.transpose("Angle", "Ekin", dim)
 
+        slow_axes = {dim} if dim else set()
+        fast_axes = set(res_xarray.dims) - slow_axes
+        projection = "reciprocal" if "Angle" in fast_axes else "real"
         conversion_metadata = res_xarray.attrs.pop("conversion_parameters")
 
         # rename coords and store mapping information, if available
         coordinate_mapping = self._config.get("coordinate_mapping", {})
         coordinate_depends = self._config.get("coordinate_depends", {})
         rename_dict = {
             k: coordinate_mapping[k] for k in coordinate_mapping.keys() if k in res_xarray.dims
         }
         depends_dict = {
             rename_dict[k]: coordinate_depends[k]
             for k in coordinate_depends.keys()
             if k in res_xarray.dims
         }
         res_xarray = res_xarray.rename(rename_dict)
+        for k, v in coordinate_mapping.items():
+            if k in fast_axes:
+                fast_axes.remove(k)
+                fast_axes.add(v)
+            if k in slow_axes:
+                slow_axes.remove(k)
+                slow_axes.add(v)
         self._scan_info["coordinate_depends"] = depends_dict
 
         axis_dict = {
             "/entry/sample/transformations/sample_polar": "Polar",
             "/entry/sample/transformations/sample_tilt": "Tilt",
             "/entry/sample/transformations/sample_azimuth": "Azimuth",
         }
@@ -258,16 +268,17 @@
                 pass
 
         self.metadata.update(
             **handle_meta(
                 df_lut,
                 self._scan_info,
                 self.config,
-                fast_axis="Angle" if "Angle" in res_xarray.dims else "Position",
-                slow_axis=dim,
+                fast_axes=list(fast_axes),  # type: ignore
+                slow_axes=list(slow_axes),
+                projection=projection,
                 metadata=copy.deepcopy(metadata),
                 collect_metadata=collect_metadata,
             ),
             **{"loader": loader_dict},
             **{"conversion_parameters": conversion_metadata},
         )
 
@@ -308,14 +319,35 @@
             self._scan_info["LensMode"],
             self._scan_info["KineticEnergy"],
             self._scan_info["PassEnergy"],
             self._scan_info["WorkFunction"],
             **kwds,
         )
 
+    def fft_tool(self, scan: int = None, path: Path | str = "", **kwds):
+        matplotlib.use("module://ipympl.backend_nbagg")
+        if scan is not None:
+            scan_path = get_scan_path(path, scan, self._config["data_path"])
+
+            data = load_images(
+                scan_path=scan_path,
+                tqdm_enable_nested=self._config["enable_nested_progress_bar"],
+            )
+            image = data[0]
+        else:
+            try:
+                image = self.metadata["loader"]["raw_data"][0]
+            except KeyError as exc:
+                raise ValueError("No image loaded, load image first!") from exc
+
+        self.spa.fft_tool(
+            image,
+            **kwds,
+        )
+
     def check_scan(
         self,
         scan: int,
         delays: Sequence[int] | int,
         path: str | Path = "",
         metadata: dict = {},
         collect_metadata: bool = False,
@@ -407,21 +439,26 @@
         res_xarray = res_xarray.transpose("Angle", "Ekin", "Iteration")
         for name in res_xarray.dims:
             try:
                 res_xarray[name].attrs["unit"] = self._config["units"][name]
             except KeyError:
                 pass
 
+        slow_axes = {"Iteration"}
+        fast_axes = set(res_xarray.dims) - slow_axes
+        projection = "reciprocal" if "Angle" in fast_axes else "real"
+
         self.metadata.update(
             **handle_meta(
                 df_lut,
                 self._scan_info,
                 self.config,
-                fast_axis="Angle" if "Angle" in res_xarray.dims else "Position",
-                slow_axis=dims[1],
+                fast_axes=list(fast_axes),  # type: ignore
+                slow_axes=list(slow_axes),
+                projection=projection,
                 metadata=metadata,
                 collect_metadata=collect_metadata,
             ),
             **{"loader": loader_dict},
             **{"conversion_parameters": conversion_metadata},
         )
         if metadata is not None:
```

### Comparing `specsanalyzer-0.1.6a0/specsscan/helpers.py` & `specsanalyzer-0.1.6a1/specsscan/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,28 +344,29 @@
     return info_dict
 
 
 def handle_meta(
     df_lut: pd.DataFrame,
     scan_info: dict,
     config: dict,
-    fast_axis: str,
-    slow_axis: str,
+    fast_axes: list[str],
+    slow_axes: list[str],
+    projection: str,
     metadata: dict = None,
     collect_metadata: bool = False,
 ) -> dict:
     """Helper function for the handling metadata from different files
 
     Args:
         df_lut (pd.DataFrame): Pandas dataframe containing the contents of LUT.txt as obtained
             from ``parse_lut_to_df()``
         scan_info (dict): scan_info class dict containing containing the contents of info.txt file
         config (dict): config dictionary containing the contents of config.yaml file
-        fast_axis (str): The fast-axis dimension of the scan
-        slow_axis (str): The slow-axis dimension of the scan
+        fast_axes (list[str]): The fast-axis dimensions of the scan
+        slow_axes (list[str]): The slow-axis dimensions of the scan
         metadata (dict, optional): Metadata dictionary with additional metadata for the scan.
             Defaults to empty dictionary.
         collect_metadata (bool, optional): Option to collect further metadata e.g. from EPICS
             archiver needed for NeXus conversion. Defaults to False.
 
     Returns:
         dict: metadata dictionary containing additional metadata from the EPICS
@@ -466,22 +467,21 @@
                         f"Skipping over channels {channels_missing}.",
                     )
                     print("Error code: ", exc)
                     break
 
     metadata["scan_info"]["energy_scan_mode"] = energy_scan_mode
 
-    projection = "reciprocal" if fast_axis in {"Anlge", "angular0", "angular1"} else "real"
     metadata["scan_info"]["projection"] = projection
     metadata["scan_info"]["scheme"] = (
         "angular dispersive" if projection == "reciprocal" else "spatial dispersive"
     )
 
-    metadata["scan_info"]["slow_axes"] = slow_axis
-    metadata["scan_info"]["fast_axes"] = ["Ekin", fast_axis]
+    metadata["scan_info"]["slow_axes"] = slow_axes
+    metadata["scan_info"]["fast_axes"] = fast_axes
 
     print("Done!")
 
     return metadata
 
 
 def get_archiver_data(
```

### Comparing `specsanalyzer-0.1.6a0/setup.py` & `specsanalyzer-0.1.6a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 extras_require = \
 {'notebook': ['jupyter[notebook]>=1.0.0',
               'ipykernel[notebook]>=6.9.1',
               'jupyterlab-h5web[notebook]>=7.0.0']}
 
 setup_kwargs = {
     'name': 'specsanalyzer',
-    'version': '0.1.6a0',
+    'version': '0.1.6a1',
     'description': 'Python package for loading and converting SPECS Phoibos analyzer data.',
     'long_description': '[![Documentation Status](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/documentation.yml/badge.svg)](https://opencompes.github.io/specsanalyzer/)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/linting.yml/badge.svg)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/testing_multiversion.yml/badge.svg?branch=main)\n![](https://img.shields.io/pypi/pyversions/specsanalyzer)\n![](https://img.shields.io/pypi/l/specsanalyzer)\n[![](https://img.shields.io/pypi/v/specsanalyzer)](https://pypi.org/project/specsanalyzer)\n[![Coverage Status](https://coveralls.io/repos/github/OpenCOMPES/specsanalyzer/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/OpenCOMPES/specsanalyzer?branch=main)\n\n# specsanalyzer\nThis is the package `specsanalyzer` for conversion and handling of SPECS Phoibos analyzer data.\n\nThis package contains two modules:\n`specsanalyzer` is a package to import and convert MCP analyzer images from SPECS Phoibos analyzers into energy and emission angle/physical coordinates.\n`specsscan` is a Python package for loading Specs Phoibos scans accquired with the labview software developed at FHI/EPFL\n\nTutorials for usage and the API documentation can be found in the [Documentation](https://opencompes.github.io/specsanalyzer/)\n\n## Installation\n\n### Pip (for users)\n\n- Create a new virtual environment using either venv, pyenv, conda, etc. See below for an example.\n\n```bash\npython -m venv .specs-venv\n```\n\n- Activate your environment:\n\n```bash\nsource .specs-venv/bin/activate\n```\n\n- Install `specsanalyzer` from PyPI:\n\n```bash\npip install specsanalyzer\n```\n\n- This should install all the requirements to run `specsanalyzer` and `specsscan`in your environment.\n\n- If you intend to work with Jupyter notebooks, it is helpful to install a Jupyter kernel for your environment. This can be done, once your environment is activated, by typing:\n\n```bash\npython -m ipykernel install --user --name=specs_kernel\n```\n\n#### Configuration and calib2d file\nThe conversion procedures require to set up several configuration parameters in a config file. An example config file is provided as part of the package (see documentation). Configuration files can either be passed to the class constructures, or are read from system-wide or user-defined locations (see documentation).\n\nMost importantly, conversion of analyzer data to energy/angular coordinates requires detector calibration data provided by the manufacturer. The corresponding *.calib2d file (e.g. phoibos150.calbid2d) are provided together with the spectrometer software, and need to be set in the config file.\n\n### For Contributors\n\nTo contribute to the development of `specsanalyzer`, you can follow these steps:\n\n1. Clone the repository:\n\n```bash\ngit clone https://github.com/OpenCOMPES/specsanalyzer.git\ncd specsanalyzer\n```\n\n2. Check out test data (optional, requires access rights):\n\n```bash\ngit submodule sync --recursive\ngit submodule update --init --recursive\n```\n\n2. Install the repository in editable mode:\n\n```bash\npip install -e .\n```\n\nNow you have the development version of `specsanalyzer` installed in your local environment. Feel free to make changes and submit pull requests.\n\n### Poetry (for maintainers)\n\n- Prerequisites:\n  + Poetry: https://python-poetry.org/docs/\n\n- Create a virtual environment by typing:\n\n```bash\npoetry shell\n```\n\n- A new shell will be spawned with the new environment activated.\n\n- Install the dependencies from the `pyproject.toml` by typing:\n\n```bash\npoetry install --with dev, docs\n```\n\n- If you wish to use the virtual environment created by Poetry to work in a Jupyter notebook, you first need to install the optional notebook dependencies and then create a Jupyter kernel for that.\n\n  + Install the optional dependencies `ipykernel` and `jupyter`:\n\n  ```bash\n  poetry install -E notebook\n  ```\n\n  + Make sure to run the command below within your virtual environment (`poetry run` ensures this) by typing:\n\n  ```bash\n  poetry run ipython kernel install --user --name=specs_poetry\n  ```\n\n  + The new kernel will now be available in your Jupyter kernels list.\n',
     'author': 'Laurenz Rettig',
     'author_email': 'rettig@fhi-berlin.mpg.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mpes-kit/specsanalyzer',
```

### Comparing `specsanalyzer-0.1.6a0/PKG-INFO` & `specsanalyzer-0.1.6a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsanalyzer
-Version: 0.1.6a0
+Version: 0.1.6a1
 Summary: Python package for loading and converting SPECS Phoibos analyzer data.
 Home-page: https://github.com/mpes-kit/specsanalyzer
 License: MIT
 Keywords: specs,phoibos,arpes
 Author: Laurenz Rettig
 Author-email: rettig@fhi-berlin.mpg.de
 Requires-Python: >=3.8,<3.12
```

