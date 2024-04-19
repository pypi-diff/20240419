# Comparing `tmp/specsanalyzer-0.1.6a1.tar.gz` & `tmp/specsanalyzer-0.1.6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsanalyzer-0.1.6a1.tar", max compression
+gzip compressed data, was "specsanalyzer-0.1.6a2.tar", max compression
```

## Comparing `specsanalyzer-0.1.6a1.tar` & `specsanalyzer-0.1.6a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1067 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/LICENSE
--rw-r--r--   0        0        0     4279 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/README.md
--rw-r--r--   0        0        0     2631 2024-04-19 19:39:30.235787 specsanalyzer-0.1.6a1/pyproject.toml
--rwxr-xr-x   0        0        0      145 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/__init__.py
--rw-r--r--   0        0        0      695 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/config/default.yaml
--rwxr-xr-x   0        0        0      411 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/config/phoibos150.calib2d
--rwxr-xr-x   0        0        0     8973 2024-04-19 19:39:18.879731 specsanalyzer-0.1.6a1/specsanalyzer/config.py
--rwxr-xr-x   0        0        0    19345 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/convert.py
--rwxr-xr-x   0        0        0    29609 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/core.py
--rwxr-xr-x   0        0        0     4250 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/img_tools.py
--rwxr-xr-x   0        0        0    18805 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsanalyzer/io.py
--rwxr-xr-x   0        0        0      133 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/__init__.py
--rwxr-xr-x   0        0        0    15200 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/config/NXmpes_arpes_config.json
--rw-r--r--   0        0        0      556 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/config/default.yaml
--rw-r--r--   0        0        0     3347 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/config/example_config_FHI.yaml
--rwxr-xr-x   0        0        0    22754 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/core.py
--rw-r--r--   0        0        0    20015 2024-04-19 19:39:18.883731 specsanalyzer-0.1.6a1/specsscan/helpers.py
--rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a1/setup.py
--rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a1/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2024-04-19 20:27:14.045019 specsanalyzer-0.1.6a2/LICENSE
+-rw-r--r--   0        0        0     4279 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/README.md
+-rw-r--r--   0        0        0     2631 2024-04-19 20:27:30.884882 specsanalyzer-0.1.6a2/pyproject.toml
+-rwxr-xr-x   0        0        0      145 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/specsanalyzer/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/specsanalyzer/config/default.yaml
+-rwxr-xr-x   0        0        0      411 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/specsanalyzer/config/phoibos150.calib2d
+-rwxr-xr-x   0        0        0     8973 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/specsanalyzer/config.py
+-rwxr-xr-x   0        0        0    19345 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/specsanalyzer/convert.py
+-rwxr-xr-x   0        0        0    30409 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/specsanalyzer/core.py
+-rwxr-xr-x   0        0        0     4250 2024-04-19 20:27:14.049020 specsanalyzer-0.1.6a2/specsanalyzer/img_tools.py
+-rwxr-xr-x   0        0        0    18805 2024-04-19 20:27:14.053020 specsanalyzer-0.1.6a2/specsanalyzer/io.py
+-rwxr-xr-x   0        0        0      133 2024-04-19 20:27:14.053020 specsanalyzer-0.1.6a2/specsscan/__init__.py
+-rwxr-xr-x   0        0        0    15200 2024-04-19 20:27:14.053020 specsanalyzer-0.1.6a2/specsscan/config/NXmpes_arpes_config.json
+-rw-r--r--   0        0        0      556 2024-04-19 20:27:14.053020 specsanalyzer-0.1.6a2/specsscan/config/default.yaml
+-rw-r--r--   0        0        0     3347 2024-04-19 20:27:14.053020 specsanalyzer-0.1.6a2/specsscan/config/example_config_FHI.yaml
+-rwxr-xr-x   0        0        0    23671 2024-04-19 20:27:14.053020 specsanalyzer-0.1.6a2/specsscan/core.py
+-rw-r--r--   0        0        0    20015 2024-04-19 20:27:14.053020 specsanalyzer-0.1.6a2/specsscan/helpers.py
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a2/setup.py
+-rw-r--r--   0        0        0     5771 1970-01-01 00:00:00.000000 specsanalyzer-0.1.6a2/PKG-INFO
```

### Comparing `specsanalyzer-0.1.6a1/LICENSE` & `specsanalyzer-0.1.6a2/LICENSE`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/README.md` & `specsanalyzer-0.1.6a2/README.md`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/pyproject.toml` & `specsanalyzer-0.1.6a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "specsanalyzer"
 packages = [
     {include = "specsanalyzer"},
     {include = "specsscan"},
 ]
-version = "0.1.6a1"
+version = "0.1.6a2"
 description = "Python package for loading and converting SPECS Phoibos analyzer data."
 authors = [
     "Laurenz Rettig <rettig@fhi-berlin.mpg.de>",
     "Michele Puppin <michele.puppin@epfl.ch>",
     "Abeer Arora <arora@fhi-berlin.mpg.de>",
 ]
 readme = "README.md"
```

### Comparing `specsanalyzer-0.1.6a1/specsanalyzer/config/default.yaml` & `specsanalyzer-0.1.6a2/specsanalyzer/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsanalyzer/config.py` & `specsanalyzer-0.1.6a2/specsanalyzer/config.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsanalyzer/convert.py` & `specsanalyzer-0.1.6a2/specsanalyzer/convert.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsanalyzer/core.py` & `specsanalyzer-0.1.6a2/specsanalyzer/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -378,22 +378,25 @@
                 Defaults to False.
             **kwds: Keyword parameters for the crop tool:
 
                 - ek_range_min
                 - ek_range_max
                 - ang_range_min
                 - ang_range_max
+
+                Other parameters are passed to ``convert_image()``.
         """
         data_array = self.convert_image(
             raw_img=raw_img,
             lens_mode=lens_mode,
             kinetic_energy=kinetic_energy,
             pass_energy=pass_energy,
             work_function=work_function,
             crop=False,
+            **kwds,
         )
 
         matplotlib.use("module://ipympl.backend_nbagg")
         fig = plt.figure()
         ax = fig.add_subplot(111)
         try:
             mesh_obj = data_array.plot(ax=ax)
@@ -577,39 +580,37 @@
         the class config dict under fft_filter_peaks.
 
         Args:
             raw_image (np.ndarray): The source image
             apply (bool, optional): Option to directly apply the settings. Defaults to False.
             **kwds: Keyword arguments:
 
-                - fft_tool_params (dict): Dictionary of parameters for fft_tool, containing keys
-                  `amplitude`: Normalized amplitude of subtraction
-                  `pos_x`: horzontal spatial frequency of th mesh
-                  `pos_y`: vertical spatial frequency of the mesh
-                  `sigma_x`: horizontal frequency width
-                  `sigma_y`: vertical frequency width
+                - `amplitude`: Normalized amplitude of subtraction
+                - `pos_x`: horzontal spatial frequency of th mesh
+                - `pos_y`: vertical spatial frequency of the mesh
+                - `sigma_x`: horizontal frequency width
+                - `sigma_y`: vertical frequency width
         """
         matplotlib.use("module://ipympl.backend_nbagg")
-        try:
-            fft_tool_params = (
-                kwds["fft_tool_params"]
-                if "fft_tool_params" in kwds
-                else self._correction_matrix_dict["fft_tool_params"]
-            )
-            (amp, pos_x, pos_y, sig_x, sig_y) = (
-                fft_tool_params["amplitude"],
-                fft_tool_params["pos_x"],
-                fft_tool_params["pos_y"],
-                fft_tool_params["sigma_x"],
-                fft_tool_params["sigma_y"],
-            )
-        except KeyError:
-            (amp, pos_x, pos_y, sig_x, sig_y) = (0.95, 86, 116, 13, 22)
+        stored_parameters = self._correction_matrix_dict.get("fft_tool_params", {})
+        if not stored_parameters:
+            stored_parameters = {
+                "amplitude": 0.95,
+                "pos_x": 86,
+                "pos_y": 116,
+                "sigma_x": 13,
+                "sigma_y": 22,
+            }
+        amplitude = kwds.get("amplitude", stored_parameters["amplitude"])
+        pos_x = kwds.get("pos_x", stored_parameters["pos_x"])
+        pos_y = kwds.get("pos_y", stored_parameters["pos_y"])
+        sigma_x = kwds.get("sigma_x", stored_parameters["sigma_x"])
+        sigma_y = kwds.get("sigma_y", stored_parameters["sigma_y"])
 
-        fft_filter_peaks = create_fft_params(amp, pos_x, pos_y, sig_x, sig_y)
+        fft_filter_peaks = create_fft_params(amplitude, pos_x, pos_y, sigma_x, sigma_y)
         try:
             img = fourier_filter_2d(raw_image, peaks=fft_filter_peaks, ret="fft")
             fft_filtered = fourier_filter_2d(raw_image, peaks=fft_filter_peaks, ret="filtered_fft")
 
             mask = fourier_filter_2d(raw_image, peaks=fft_filter_peaks, ret="mask")
 
             filtered = fourier_filter_2d(raw_image, peaks=fft_filter_peaks, ret="filtered")
@@ -642,59 +643,59 @@
         ax4.legend()
 
         ax5 = fig.add_subplot(3, 2, 6)
         (mdc,) = ax5.plot(np.sum(filtered, 1), label="MDC")
         ax5.legend()
         # plt.tight_layout()
 
-        posx_slider = ipw.FloatSlider(
+        pos_x_slider = ipw.FloatSlider(
             description="pos_x",
             value=pos_x,
             min=0,
             max=128,
             step=1,
         )
-        posy_slider = ipw.FloatSlider(
+        pos_y_slider = ipw.FloatSlider(
             description="pos_y",
             value=pos_y,
             min=0,
             max=150,
             step=1,
         )
-        sigx_slider = ipw.FloatSlider(
+        sigma_x_slider = ipw.FloatSlider(
             description="sig_x",
-            value=sig_x,
+            value=sigma_x,
             min=0,
             max=50,
             step=1,
         )
-        sigy_slider = ipw.FloatSlider(
+        sigma_y_slider = ipw.FloatSlider(
             description="sig_y",
-            value=sig_y,
+            value=sigma_y,
             min=0,
             max=50,
             step=1,
         )
-        amp_slider = ipw.FloatSlider(
+        amplitude_slider = ipw.FloatSlider(
             description="Amplitude",
-            value=amp,
+            value=amplitude,
             min=0,
             max=1,
             step=0.01,
         )
         clim_slider = ipw.FloatLogSlider(
             description="colorbar limits",
             value=int(np.abs(img).max() / 500),
             base=10,
             min=-1,
             max=int(np.log10(np.abs(img).max())) + 1,
         )
 
-        def update(v_vals, pos_x, pos_y, sig_x, sig_y, amp):
-            fft_filter_peaks = create_fft_params(amp, pos_x, pos_y, sig_x, sig_y)
+        def update(v_vals, pos_x, pos_y, sigma_x, sigma_y, amplitude):
+            fft_filter_peaks = create_fft_params(amplitude, pos_x, pos_y, sigma_x, sigma_y)
             msk = fourier_filter_2d(raw_image, peaks=fft_filter_peaks, ret="mask")
             filtered_new = fourier_filter_2d(raw_image, peaks=fft_filter_peaks, ret="filtered")
 
             fft_filtered_new = fourier_filter_2d(
                 raw_image,
                 peaks=fft_filter_peaks,
                 ret="filtered_fft",
@@ -714,73 +715,111 @@
             edc.set_ydata(np.sum(filtered_new, 0))
             mdc.set_ydata(np.sum(filtered_new, 1))
 
             fig.canvas.draw_idle()
 
         ipw.interact(
             update,
-            amp=amp_slider,
-            pos_x=posx_slider,
-            pos_y=posy_slider,
-            sig_x=sigx_slider,
-            sig_y=sigy_slider,
+            amplitude=amplitude_slider,
+            pos_x=pos_x_slider,
+            pos_y=pos_y_slider,
+            sigma_x=sigma_x_slider,
+            sigma_y=sigma_y_slider,
             v_vals=clim_slider,
         )
 
         def apply_fft(apply: bool):  # pylint: disable=unused-argument
-            amp = amp_slider.value
-            pos_x = posx_slider.value
-            pos_y = posy_slider.value
-            sig_x = sigx_slider.value
-            sig_y = sigy_slider.value
+            amplitude = amplitude_slider.value
+            pos_x = pos_x_slider.value
+            pos_y = pos_y_slider.value
+            sigma_x = sigma_x_slider.value
+            sigma_y = sigma_y_slider.value
             self._correction_matrix_dict["fft_tool_params"] = {
-                "amplitude": amp,
+                "amplitude": amplitude,
                 "pos_x": pos_x,
                 "pos_y": pos_y,
-                "sigma_x": sig_x,
-                "sigma_y": sig_y,
+                "sigma_x": sigma_x,
+                "sigma_y": sigma_y,
             }
             self.config["fft_filter_peaks"] = create_fft_params(
-                amp,
+                amplitude,
                 pos_x,
                 pos_y,
-                sig_x,
-                sig_y,
+                sigma_x,
+                sigma_y,
             )
-            amp_slider.close()
-            posx_slider.close()
-            posy_slider.close()
-            sigx_slider.close()
-            sigy_slider.close()
+            amplitude_slider.close()
+            pos_x_slider.close()
+            pos_y_slider.close()
+            sigma_x_slider.close()
+            sigma_y_slider.close()
             clim_slider.close()
             apply_button.close()
 
         apply_button = ipw.Button(description="Apply")
         display(apply_button)
         apply_button.on_click(apply_fft)
         plt.show()
         if apply:
             apply_fft(True)
 
 
-def create_fft_params(amp, pos_x, pos_y, sig_x, sig_y) -> list[dict]:
-    """Function to create fft filter peaks list using the
-    provided Gaussian peak parameters. The peaks are defined
-    relative to each other such that they are periodically
-    aranged in a 256 x 150 Fourier space.
+def create_fft_params(
+    amplitude: float,
+    pos_x: float,
+    pos_y: float,
+    sigma_x: float,
+    sigma_y: float,
+) -> list[dict]:
+    """Function to create fft filter peaks list using the provided Gaussian peak parameters.
+    The peaks are placed at +-x, y=0, and +-x, y=y, with width corresponding to the sigma
+    values.
+
     Args:
-        amp: Gaussian peak amplitude
-        pos_x: x-position
-        pos_y: y-position
-        sig_x: FWHM in x-axis
-        sig_y: FWHM in y-axis
-    """
+        amplitude (float): Gaussian peak amplitude
+        pos_x (float): horizontal spatial frequency
+        pos_y (float): vertical spatial frequency
+        sigma_x (float): horizontal width
+        sigma_y (float): vertical width
 
+    Returns:
+        list[dict]: A list of the defined filter parameters
+    """
     fft_filter_peaks = [
-        {"amplitude": amp, "pos_x": -pos_x, "pos_y": 0, "sigma_x": sig_x, "sigma_y": sig_y},
-        {"amplitude": amp, "pos_x": pos_x, "pos_y": 0, "sigma_x": sig_x, "sigma_y": sig_y},
-        {"amplitude": amp, "pos_x": 0, "pos_y": pos_y, "sigma_x": sig_x, "sigma_y": sig_y},
-        {"amplitude": amp, "pos_x": -pos_x, "pos_y": pos_y, "sigma_x": sig_x, "sigma_y": sig_y},
-        {"amplitude": amp, "pos_x": pos_x, "pos_y": pos_y, "sigma_x": sig_x, "sigma_y": sig_y},
+        {
+            "amplitude": amplitude,
+            "pos_x": -pos_x,
+            "pos_y": 0,
+            "sigma_x": sigma_x,
+            "sigma_y": sigma_y,
+        },
+        {
+            "amplitude": amplitude,
+            "pos_x": pos_x,
+            "pos_y": 0,
+            "sigma_x": sigma_x,
+            "sigma_y": sigma_y,
+        },
+        {
+            "amplitude": amplitude,
+            "pos_x": 0,
+            "pos_y": pos_y,
+            "sigma_x": sigma_x,
+            "sigma_y": sigma_y,
+        },
+        {
+            "amplitude": amplitude,
+            "pos_x": -pos_x,
+            "pos_y": pos_y,
+            "sigma_x": sigma_x,
+            "sigma_y": sigma_y,
+        },
+        {
+            "amplitude": amplitude,
+            "pos_x": pos_x,
+            "pos_y": pos_y,
+            "sigma_x": sigma_x,
+            "sigma_y": sigma_y,
+        },
     ]
 
     return fft_filter_peaks
```

### Comparing `specsanalyzer-0.1.6a1/specsanalyzer/img_tools.py` & `specsanalyzer-0.1.6a2/specsanalyzer/img_tools.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsanalyzer/io.py` & `specsanalyzer-0.1.6a2/specsanalyzer/io.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsscan/config/NXmpes_arpes_config.json` & `specsanalyzer-0.1.6a2/specsscan/config/NXmpes_arpes_config.json`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsscan/config/default.yaml` & `specsanalyzer-0.1.6a2/specsscan/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsscan/config/example_config_FHI.yaml` & `specsanalyzer-0.1.6a2/specsscan/config/example_config_FHI.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/specsscan/core.py` & `specsanalyzer-0.1.6a2/specsscan/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -320,14 +320,30 @@
             self._scan_info["KineticEnergy"],
             self._scan_info["PassEnergy"],
             self._scan_info["WorkFunction"],
             **kwds,
         )
 
     def fft_tool(self, scan: int = None, path: Path | str = "", **kwds):
+        """FFT tool to play around with the peak parameters in the Fourier plane. Built to filter
+        out the meshgrid appearing in the raw data images. The optimized parameters are stored in
+        the class config dict under fft_filter_peaks.
+
+        Args:
+            scan (int, optional): Scan number to load. Defaults to the previously loaded scan.
+            path (Path | str): Path from where to load the data. Defaults to config value.
+            **kwds: Keyword arguments passed to ``SpecsAnalyzer.fft_tool()``:
+
+                - `apply`: Option to directly apply the settings.
+                - `amplitude`: Normalized amplitude of subtraction
+                - `pos_x`: horzontal spatial frequency of th mesh
+                - `pos_y`: vertical spatial frequency of the mesh
+                - `sigma_x`: horizontal frequency width
+                - `sigma_y`: vertical frequency width
+        """
         matplotlib.use("module://ipympl.backend_nbagg")
         if scan is not None:
             scan_path = get_scan_path(path, scan, self._config["data_path"])
 
             data = load_images(
                 scan_path=scan_path,
                 tqdm_enable_nested=self._config["enable_nested_progress_bar"],
```

### Comparing `specsanalyzer-0.1.6a1/specsscan/helpers.py` & `specsanalyzer-0.1.6a2/specsscan/helpers.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.1.6a1/setup.py` & `specsanalyzer-0.1.6a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 extras_require = \
 {'notebook': ['jupyter[notebook]>=1.0.0',
               'ipykernel[notebook]>=6.9.1',
               'jupyterlab-h5web[notebook]>=7.0.0']}
 
 setup_kwargs = {
     'name': 'specsanalyzer',
-    'version': '0.1.6a1',
+    'version': '0.1.6a2',
     'description': 'Python package for loading and converting SPECS Phoibos analyzer data.',
     'long_description': '[![Documentation Status](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/documentation.yml/badge.svg)](https://opencompes.github.io/specsanalyzer/)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/linting.yml/badge.svg)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/testing_multiversion.yml/badge.svg?branch=main)\n![](https://img.shields.io/pypi/pyversions/specsanalyzer)\n![](https://img.shields.io/pypi/l/specsanalyzer)\n[![](https://img.shields.io/pypi/v/specsanalyzer)](https://pypi.org/project/specsanalyzer)\n[![Coverage Status](https://coveralls.io/repos/github/OpenCOMPES/specsanalyzer/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/OpenCOMPES/specsanalyzer?branch=main)\n\n# specsanalyzer\nThis is the package `specsanalyzer` for conversion and handling of SPECS Phoibos analyzer data.\n\nThis package contains two modules:\n`specsanalyzer` is a package to import and convert MCP analyzer images from SPECS Phoibos analyzers into energy and emission angle/physical coordinates.\n`specsscan` is a Python package for loading Specs Phoibos scans accquired with the labview software developed at FHI/EPFL\n\nTutorials for usage and the API documentation can be found in the [Documentation](https://opencompes.github.io/specsanalyzer/)\n\n## Installation\n\n### Pip (for users)\n\n- Create a new virtual environment using either venv, pyenv, conda, etc. See below for an example.\n\n```bash\npython -m venv .specs-venv\n```\n\n- Activate your environment:\n\n```bash\nsource .specs-venv/bin/activate\n```\n\n- Install `specsanalyzer` from PyPI:\n\n```bash\npip install specsanalyzer\n```\n\n- This should install all the requirements to run `specsanalyzer` and `specsscan`in your environment.\n\n- If you intend to work with Jupyter notebooks, it is helpful to install a Jupyter kernel for your environment. This can be done, once your environment is activated, by typing:\n\n```bash\npython -m ipykernel install --user --name=specs_kernel\n```\n\n#### Configuration and calib2d file\nThe conversion procedures require to set up several configuration parameters in a config file. An example config file is provided as part of the package (see documentation). Configuration files can either be passed to the class constructures, or are read from system-wide or user-defined locations (see documentation).\n\nMost importantly, conversion of analyzer data to energy/angular coordinates requires detector calibration data provided by the manufacturer. The corresponding *.calib2d file (e.g. phoibos150.calbid2d) are provided together with the spectrometer software, and need to be set in the config file.\n\n### For Contributors\n\nTo contribute to the development of `specsanalyzer`, you can follow these steps:\n\n1. Clone the repository:\n\n```bash\ngit clone https://github.com/OpenCOMPES/specsanalyzer.git\ncd specsanalyzer\n```\n\n2. Check out test data (optional, requires access rights):\n\n```bash\ngit submodule sync --recursive\ngit submodule update --init --recursive\n```\n\n2. Install the repository in editable mode:\n\n```bash\npip install -e .\n```\n\nNow you have the development version of `specsanalyzer` installed in your local environment. Feel free to make changes and submit pull requests.\n\n### Poetry (for maintainers)\n\n- Prerequisites:\n  + Poetry: https://python-poetry.org/docs/\n\n- Create a virtual environment by typing:\n\n```bash\npoetry shell\n```\n\n- A new shell will be spawned with the new environment activated.\n\n- Install the dependencies from the `pyproject.toml` by typing:\n\n```bash\npoetry install --with dev, docs\n```\n\n- If you wish to use the virtual environment created by Poetry to work in a Jupyter notebook, you first need to install the optional notebook dependencies and then create a Jupyter kernel for that.\n\n  + Install the optional dependencies `ipykernel` and `jupyter`:\n\n  ```bash\n  poetry install -E notebook\n  ```\n\n  + Make sure to run the command below within your virtual environment (`poetry run` ensures this) by typing:\n\n  ```bash\n  poetry run ipython kernel install --user --name=specs_poetry\n  ```\n\n  + The new kernel will now be available in your Jupyter kernels list.\n',
     'author': 'Laurenz Rettig',
     'author_email': 'rettig@fhi-berlin.mpg.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mpes-kit/specsanalyzer',
```

### Comparing `specsanalyzer-0.1.6a1/PKG-INFO` & `specsanalyzer-0.1.6a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsanalyzer
-Version: 0.1.6a1
+Version: 0.1.6a2
 Summary: Python package for loading and converting SPECS Phoibos analyzer data.
 Home-page: https://github.com/mpes-kit/specsanalyzer
 License: MIT
 Keywords: specs,phoibos,arpes
 Author: Laurenz Rettig
 Author-email: rettig@fhi-berlin.mpg.de
 Requires-Python: >=3.8,<3.12
```

