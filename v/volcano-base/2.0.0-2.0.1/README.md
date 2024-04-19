# Comparing `tmp/volcano_base-2.0.0.tar.gz` & `tmp/volcano_base-2.0.1.tar.gz`

## Comparing `volcano_base-2.0.0.tar` & `volcano_base-2.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.mise.local.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.mise.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.release-please-manifest.json
--rw-r--r--   0        0        0    18771 2020-02-02 00:00:00.000000 volcano_base-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.0/release-please-config.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 volcano_base-2.0.0/requirements-dev.lock
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 volcano_base-2.0.0/requirements.lock
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/release-please/release-please-config.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/release-please/release-please-manifest.json
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 volcano_base-2.0.0/assets/examples.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/__init__.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/config.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/cesm2.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/historic_so2.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/down/ob16.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/load/__init__.py
--rw-r--r--   0        0        0    24171 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/load/load_c2w_files.py
--rw-r--r--   0        0        0    31469 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/load/load_ob16.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/manipulate/__init__.py
--rw-r--r--   0        0        0    24352 2020-02-02 00:00:00.000000 volcano_base-2.0.0/src/volcano_base/manipulate/time_series.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-2.0.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-2.0.0/LICENSE
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-2.0.0/README.md
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 volcano_base-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.mise.local.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.mise.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.release-please-manifest.json
+-rw-r--r--   0        0        0    19832 2020-02-02 00:00:00.000000 volcano_base-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.1/release-please-config.json
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 volcano_base-2.0.1/requirements-dev.lock
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 volcano_base-2.0.1/requirements.lock
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.github/release-please/release-please-config.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.github/release-please/release-please-manifest.json
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 volcano_base-2.0.1/assets/examples.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/__init__.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/config.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/down/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/down/cesm2.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/down/historic_so2.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/down/ob16.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/load/__init__.py
+-rw-r--r--   0        0        0    24131 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/load/load_c2w_files.py
+-rw-r--r--   0        0        0    31646 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/load/load_ob16.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/manipulate/__init__.py
+-rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 volcano_base-2.0.1/src/volcano_base/manipulate/time_series.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 volcano_base-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 volcano_base-2.0.1/LICENSE
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 volcano_base-2.0.1/README.md
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 volcano_base-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 volcano_base-2.0.1/PKG-INFO
```

### Comparing `volcano_base-2.0.0/.mise.toml` & `volcano_base-2.0.1/.mise.toml`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/.pre-commit-config.yaml` & `volcano_base-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/CHANGELOG.md` & `volcano_base-2.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # Changelog
 
+## [2.0.1](https://github.com/engeir/volcano-base/compare/v2.0.0...v2.0.1) (2024-04-19)
+
+
+### Bug Fixes
+
+* **manipulate:** get_median accepts arbitrary dimensions provided one is time ([9197a72](https://github.com/engeir/volcano-base/commit/9197a7276d4f3423dcace0fdb434d76f39f57162))
+* **manipulate:** mean_flatten should copy the dims list input parameter ([9623f4a](https://github.com/engeir/volcano-base/commit/9623f4a9fa54b0743da80e2f4b5556aa83fdf6a4))
+
+
+### Styles
+
+* **ruff lint:** add preview mode ([131d843](https://github.com/engeir/volcano-base/commit/131d843930460790b98b4de9499fa0e7884bc755))
+* **ruff:** fix lint errors enforced by preview mode ([861a151](https://github.com/engeir/volcano-base/commit/861a151d98c4a7043891bc828e8caa6511697088))
+
+
+### Build System
+
+* **deps-dev:** bump ruff from 0.2.1 to 0.3.7 ([3d3ebf8](https://github.com/engeir/volcano-base/commit/3d3ebf86ce0cdcfaa8d1f51cf5559a642a17ca83))
+* **deps:** update all dependencies ([86a32f9](https://github.com/engeir/volcano-base/commit/86a32f9cd68790e9e5779a133212b6ee3c7df470))
+
 ## [2.0.0](https://github.com/engeir/volcano-base/compare/v1.8.4...v2.0.0) (2024-04-09)
 
 
 ### ⚠ BREAKING CHANGES
 
 * **cesm load:** use a regex class object to specify files to find
```

### Comparing `volcano_base-2.0.0/release-please-config.json` & `volcano_base-2.0.1/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/requirements-dev.lock` & `volcano_base-2.0.1/requirements-dev.lock`

 * *Files 8% similar despite different names*

```diff
@@ -22,56 +22,54 @@
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via dask
     # via pydoclint
 cloudpickle==3.0.0
     # via dask
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-dask==2024.2.0
+dask==2024.4.1
     # via volcano-base
-datetime==5.4
+datetime==5.5
     # via volcano-base
 distlib==0.3.8
     # via virtualenv
 docstring-parser-fork==0.0.5
     # via pydoclint
-filelock==3.13.1
+filelock==3.13.4
     # via virtualenv
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
-fsspec==2024.2.0
+fsspec==2024.3.1
     # via dask
 h5netcdf==1.3.0
     # via volcano-base
-h5py==3.10.0
+h5py==3.11.0
     # via h5netcdf
-identify==2.5.34
+identify==2.5.35
     # via pre-commit
-idna==3.6
+idna==3.7
     # via requests
-importlib-metadata==7.0.1
-    # via dask
 iniconfig==2.0.0
     # via pytest
 kiwisolver==1.4.5
     # via matplotlib
 locket==1.0.0
     # via partd
 markdown-it-py==3.0.0
     # via rich
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via nc-time-axis
     # via volcano-base
 mdurl==0.1.2
     # via markdown-it-py
-mypy==1.8.0
+mypy==1.9.0
 mypy-extensions==1.0.0
     # via mypy
 nc-time-axis==1.4.1
 nodeenv==1.8.0
     # via pre-commit
 numpy==1.26.4
     # via cftime
@@ -79,96 +77,94 @@
     # via h5py
     # via matplotlib
     # via nc-time-axis
     # via pandas
     # via scipy
     # via volcano-base
     # via xarray
-packaging==23.2
+packaging==24.0
     # via dask
     # via h5netcdf
     # via matplotlib
     # via pytest
     # via xarray
-pandas==2.2.0
+pandas==2.2.2
     # via xarray
 partd==1.4.1
     # via dask
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
 platformdirs==4.2.0
     # via virtualenv
 pluggy==1.4.0
     # via pytest
-pre-commit==3.6.1
-pre-commit-hooks==4.5.0
-pydantic==2.6.2
+pre-commit==3.7.0
+pre-commit-hooks==4.6.0
+pydantic==2.7.0
     # via volcano-base
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
-pydoclint==0.4.0
+pydoclint==0.4.1
 pydocstringformatter==0.7.3
 pygments==2.17.2
     # via rich
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
 pyqt5==5.15.10
 pyqt5-qt5==5.15.2
     # via pyqt5
 pyqt5-sip==12.13.0
     # via pyqt5
-pytest==8.0.0
-python-dateutil==2.8.2
+pytest==8.1.1
+python-dateutil==2.9.0.post0
     # via matplotlib
     # via pandas
 pytz==2024.1
     # via datetime
     # via pandas
-pyupgrade==3.15.0
+pyupgrade==3.15.2
 pyyaml==6.0.1
     # via dask
     # via pre-commit
 requests==2.31.0
     # via volcano-base
 returns==0.22.0
     # via volcano-base
-rich==13.7.0
+rich==13.7.1
     # via volcano-base
 ruamel-yaml==0.18.6
     # via pre-commit-hooks
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-ruff==0.2.1
-scipy==1.12.0
+ruff==0.4.0
+scipy==1.13.0
     # via volcano-base
 six==1.16.0
     # via python-dateutil
 soupsieve==2.5
     # via beautifulsoup4
 tokenize-rt==5.2.0
     # via pyupgrade
 toolz==0.12.1
     # via dask
     # via partd
-types-requests==2.31.0.20240125
-typing-extensions==4.9.0
+types-requests==2.31.0.20240406
+typing-extensions==4.11.0
     # via mypy
     # via pydantic
     # via pydantic-core
     # via returns
 tzdata==2024.1
     # via pandas
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
     # via types-requests
-virtualenv==20.25.0
+virtualenv==20.25.3
     # via pre-commit
-xarray==2024.1.1
+xarray==2024.3.0
     # via volcano-base
 xdoctest==1.1.3
-zipp==3.17.0
-    # via importlib-metadata
-zope-interface==6.2
+zope-interface==6.3
     # via datetime
-setuptools==69.1.0
+setuptools==69.5.1
     # via nodeenv
     # via zope-interface
```

### Comparing `volcano_base-2.0.0/requirements.lock` & `volcano_base-2.0.1/requirements.lock`

 * *Files 16% similar despite different names*

```diff
@@ -18,104 +18,100 @@
     # via volcano-base
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via dask
 cloudpickle==3.0.0
     # via dask
-contourpy==1.2.0
+contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-dask==2024.2.0
+dask==2024.4.1
     # via volcano-base
-datetime==5.4
+datetime==5.5
     # via volcano-base
-fonttools==4.49.0
+fonttools==4.51.0
     # via matplotlib
-fsspec==2024.2.0
+fsspec==2024.3.1
     # via dask
 h5netcdf==1.3.0
     # via volcano-base
-h5py==3.10.0
+h5py==3.11.0
     # via h5netcdf
-idna==3.6
+idna==3.7
     # via requests
-importlib-metadata==7.0.1
-    # via dask
 kiwisolver==1.4.5
     # via matplotlib
 locket==1.0.0
     # via partd
 markdown-it-py==3.0.0
     # via rich
-matplotlib==3.8.3
+matplotlib==3.8.4
     # via volcano-base
 mdurl==0.1.2
     # via markdown-it-py
 numpy==1.26.4
     # via cftime
     # via contourpy
     # via h5py
     # via matplotlib
     # via pandas
     # via scipy
     # via volcano-base
     # via xarray
-packaging==23.2
+packaging==24.0
     # via dask
     # via h5netcdf
     # via matplotlib
     # via xarray
-pandas==2.2.0
+pandas==2.2.2
     # via xarray
 partd==1.4.1
     # via dask
-pillow==10.2.0
+pillow==10.3.0
     # via matplotlib
-pydantic==2.6.2
+pydantic==2.7.0
     # via volcano-base
-pydantic-core==2.16.3
+pydantic-core==2.18.1
     # via pydantic
 pygments==2.17.2
     # via rich
-pyparsing==3.1.1
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via matplotlib
     # via pandas
 pytz==2024.1
     # via datetime
     # via pandas
 pyyaml==6.0.1
     # via dask
 requests==2.31.0
     # via volcano-base
 returns==0.22.0
     # via volcano-base
-rich==13.7.0
+rich==13.7.1
     # via volcano-base
-scipy==1.12.0
+scipy==1.13.0
     # via volcano-base
 six==1.16.0
     # via python-dateutil
 soupsieve==2.5
     # via beautifulsoup4
 toolz==0.12.1
     # via dask
     # via partd
-typing-extensions==4.9.0
+typing-extensions==4.11.0
     # via pydantic
     # via pydantic-core
     # via returns
 tzdata==2024.1
     # via pandas
-urllib3==2.2.0
+urllib3==2.2.1
     # via requests
-xarray==2024.1.1
+xarray==2024.3.0
     # via volcano-base
-zipp==3.17.0
-    # via importlib-metadata
-zope-interface==6.2
+zope-interface==6.3
     # via datetime
-setuptools==69.1.0
+setuptools==69.5.1
     # via zope-interface
```

### Comparing `volcano_base-2.0.0/.github/release-please/release-please-config.json` & `volcano_base-2.0.1/.github/release-please/release-please-config.json`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/.github/workflows/release.yml` & `volcano_base-2.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/assets/examples.py` & `volcano_base-2.0.1/assets/examples.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/src/volcano_base/config.py` & `volcano_base-2.0.1/src/volcano_base/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 
 def ask_then_create(file_path: pathlib.Path) -> None:
     """Ask before creating a directory."""
     if file_path.exists():
         return
     # Ask user if it is ok to create config file here.
     ans = input(f"Is it okay to create {file_path.resolve()}? [y/N] ").lower()
-    if ans in ["y", "yes"]:
+    if ans in {"y", "yes"}:
         file_path.mkdir(parents=True)
     else:
         print("Okay, I will not create anything.")
 
 
 def create_config() -> Result[pathlib.Path, str]:
     """Create the file where the configuration will be saved."""
     here = pathlib.Path(".")
     ask_then_create(_data := here / "downloaded_files")
     ask_then_create(_save := here / "generated_files")
     _cfg = here / "volcano-base.toml"
     if not _cfg.exists():
         ans = input(f"Is it okay to create {_cfg.resolve()}? [y/N] ").lower()
-        if ans not in ["y", "yes"]:
+        if ans not in {"y", "yes"}:
             return Failure("No config file exists.")
-        with open(_cfg.resolve(), mode="w") as cfg:
+        with open(_cfg.resolve(), mode="w", encoding="locale") as cfg:
             _config_content(cfg, here, _data, _save)
     return Success(_cfg)
 
 
 def _config_content(cfg, here, _data, _save):
     cfg.write("[volcano-base]\n")
     cfg.write("# Location of the repository\n")
```

### Comparing `volcano_base-2.0.0/src/volcano_base/down/cesm2.py` & `volcano_base-2.0.1/src/volcano_base/down/cesm2.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     path : pathlib.Path
         Path to the file to download.
     """
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     answer = input(
         f"Is it ok that I create the directory and download all CESM2 NIRD archive files to {path.resolve()}? [y/N] "
     ).lower()
-    if answer not in ["y", "yes"]:
+    if answer not in {"y", "yes"}:
         sys.exit(
             "Ok, I will not download anything. The files are needed to run the script,"
             f" and can be downloaded manually from {_URL}."
         )
     if not path.exists():
         path.mkdir(parents=False)
     for file in _find_files():
```

### Comparing `volcano_base-2.0.0/src/volcano_base/down/historic_so2.py` & `volcano_base-2.0.1/src/volcano_base/down/historic_so2.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             " sure you want to download it again."
         )
         return
     url = f"https://svn-ccsm-inputdata.cgd.ucar.edu/trunk/inputdata/atm/cam/volc/{file.name}"
     answer = input(
         f"Is it ok that I download {file.name} to {file.parent}? [y/N] "
     ).lower()
-    if answer not in ["y", "yes"]:
+    if answer not in {"y", "yes"}:
         sys.exit(
             "Ok, I will not download anything. The file is needed to run the script,"
             f" and can be downloaded manually from {url}."
         )
     progress = rich.progress.Progress(
         rich.progress.TextColumn("[progress.description]{task.description}"),
         rich.progress.SpinnerColumn(),
```

### Comparing `volcano_base-2.0.0/src/volcano_base/down/ob16.py` & `volcano_base-2.0.1/src/volcano_base/down/ob16.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/src/volcano_base/load/load_c2w_files.py` & `volcano_base-2.0.1/src/volcano_base/load/load_c2w_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,27 +200,23 @@
 
     Examples
     --------
     >>> ff = FindFiles()
 
     You find nothing since the date is wrong.
 
-    >>> files = ff.find(
-    ...     "h0", "e_BWma1850", "strong", "U", "ens1", "2x230828"
-    ... )
+    >>> files = ff.find("h0", "e_BWma1850", "strong", "U", "ens1", "2x230828")
     Traceback (most recent call last):
     ...
     AttributeError: ...
     >>> # [print(m) for m in files.get_files()]
 
     You still find nothing since there are two specifications of ensembles.
 
-    >>> files = ff.find(
-    ...     "h0", "e_BWma1850", "strong", "U", "ens1", "ens2"
-    ... )
+    >>> files = ff.find("h0", "e_BWma1850", "strong", "U", "ens1", "ens2")
     Traceback (most recent call last):
     ...
     AttributeError: ...
     >>> # [print(m) for m in files]
 
     Now, you find all files with simulation type "strong" and ensemble type "ens2" and
     "ens4"
@@ -235,18 +231,18 @@
     >>> matches = matches.remove("ens1", "ens5")
     >>> # matches.print_files()
     >>> # print(len(matches))
 
     Keep h0, e_BWma1850 or e_fSST1850, FLNT or TREFHT or AODVISstdn and ens1 or ens2.
 
     >>> matches = matches.keep(
-    ...    "h0",
-    ...    ("e_BWma1850", "e_fSST1850"),
-    ...    ["FLNT", "TREFHT", "AODVISstdn"],
-    ...    {"ens1", "ens2"},
+    ...     "h0",
+    ...     ("e_BWma1850", "e_fSST1850"),
+    ...     ["FLNT", "TREFHT", "AODVISstdn"],
+    ...     {"ens1", "ens2"},
     ... )
     >>> # matches.print_files()
     >>> # print(len(matches))
 
     Load the files into xarray objects
 
     >>> xarrs = matches.load()
```

### Comparing `volcano_base-2.0.0/src/volcano_base/load/load_ob16.py` & `volcano_base-2.0.1/src/volcano_base/load/load_ob16.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,16 +457,17 @@
                             progress.advance(task_find_files)
             if self.progress:
                 progress.stop_task(task_find_files)
         if len(arrs) != maxfiles:
             raise Ob16FileNotFound()
         return arrs[0], arrs[1], arrs[2], arrs[3], arrs[4]
 
+    @staticmethod
     def _load_nc(
-        self, files_: list[pathlib.Path], pattern: re.Pattern, search_group: str
+        files_: list[pathlib.Path], pattern: re.Pattern, search_group: str
     ) -> tuple[xr.DataArray, xr.DataArray, xr.DataArray, xr.DataArray, xr.DataArray]:
         arrs: list[xr.DataArray] = []
         for file in files_:
             if isinstance(search := pattern.search(str(file)), re.Match):
                 array = xr.open_dataset(file.resolve())
                 if search.groups()[0] == search_group:
                     arrs.append(array[search_group])
@@ -690,40 +691,44 @@
                     name="Mean stratospheric volcanic sulfate aerosol injections [Tg]",
                 )
                 so2_decay_start = so2_decay_start.assign_coords(
                     time=so2_decay_start.time.data + datetime.timedelta(days=14)
                 )
                 d1, d2, d3, d4 = 180, -31, 44, 58
                 # We hard-code the slices to avoid the time consuming xr.align process
-                sds_slice = slice(127429, -122)
-                ss_slice = slice(127551, None)
-                sr_slice = slice(127402, -149)
-                st_slice = slice(127327, -224)
-                rf_slice = slice(0, -1929)
-                temp_slice = slice(0, -1929)
+                slices = (
+                    slice(127429, -122),  # sds_slice
+                    slice(127551, None),  # ss_slice
+                    slice(127402, -149),  # sr_slice
+                    slice(127327, -224),  # st_slice
+                    slice(0, -1929),  # rf_slice
+                    slice(0, -1929),  # temp_slice
+                )
                 so2_rf_peak = so2_start.assign_coords(
                     time=so2_start.time.data + datetime.timedelta(days=d2)
                 )
                 so2_temp_peak = so2_start.assign_coords(
                     time=so2_start.time.data + datetime.timedelta(days=d3)
                 )
                 so2_decay_start = so2_decay_start.assign_coords(
                     time=so2_decay_start.time.data - datetime.timedelta(days=d4)
                 )
                 so2_start = so2_start.assign_coords(
                     time=so2_start.time.data - datetime.timedelta(days=d1)
                 )
             case "h0":
                 d1, d2, d3, d4 = 15, 15, 15, 15
-                sds_slice = slice(4190, -4)
-                ss_slice = slice(4194, None)
-                sr_slice = slice(4189, -5)
-                st_slice = slice(4184, -10)
-                rf_slice = slice(None, -64)
-                temp_slice = slice(None, -64)
+                slices = (
+                    slice(4190, -4),  # sds_slice
+                    slice(4194, None),  # ss_slice
+                    slice(4189, -5),  # sr_slice
+                    slice(4184, -10),  # st_slice
+                    slice(None, -64),  # rf_slice
+                    slice(None, -64),  # temp_slice
+                )
                 so2_rf_peak = so2_start.assign_coords(
                     time=xr.cftime_range(
                         "0500-12", "2010", freq="MS", calendar="noleap"
                     )[: len(so2_start)]
                     + datetime.timedelta(days=d2)
                 )
                 so2_temp_peak = so2_start.assign_coords(
@@ -749,20 +754,20 @@
 
         # Aligning the arrays takes a long time, so since we know the exact indices we
         # instead slice the arrays to the correct length. Basically zero time versus 15
         # seconds.
         # so2_decay_start, so2_start, so2_rf_peak, so2_temp_peak, rf, temp = xr.align(
         #     so2_decay_start, so2_start, so2_rf_peak, so2_temp_peak, rf, temp
         # )
-        so2_decay_start = so2_decay_start[sds_slice]
-        so2_start = so2_start[ss_slice]
-        so2_rf_peak = so2_rf_peak[sr_slice]
-        so2_temp_peak = so2_temp_peak[st_slice]
-        rf = rf[rf_slice]
-        temp = temp[temp_slice]
+        so2_decay_start = so2_decay_start[slices[0]]
+        so2_start = so2_start[slices[1]]
+        so2_rf_peak = so2_rf_peak[slices[2]]
+        so2_temp_peak = so2_temp_peak[slices[3]]
+        rf = rf[slices[4]]
+        temp = temp[slices[5]]
         return so2_decay_start, so2_start, so2_rf_peak, so2_temp_peak, rf, temp
 
     def _set_aligned_arrays(self) -> None:
         """Return Otto-Bliesner et al. 2016 SO2, RF and temperature peaks.
 
         The peaks are best estimates from the full time series.
         """
```

### Comparing `volcano_base-2.0.0/src/volcano_base/manipulate/__init__.py` & `volcano_base-2.0.1/src/volcano_base/manipulate/__init__.py`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/src/volcano_base/manipulate/time_series.py` & `volcano_base-2.0.1/src/volcano_base/manipulate/time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     Implement the subtract_mean_of_tail function, first for a single array, then pass it
     to data_array_operation.
 
     >>> def single_array_sub_tail(arr: xr.DataArray) -> xr.DataArray:
     ...     arr_ = arr[-120:]
     ...     arr.data = arr.data - arr_.mean().data
     ...     return arr
-    >>> data_array_operation([xr.DataArray([1, 2, 3]), xr.DataArray([4, 5, 6])], single_array_sub_tail)
+    >>> data_array_operation(
+    ...     [xr.DataArray([1, 2, 3]), xr.DataArray([4, 5, 6])], single_array_sub_tail
+    ... )
     """
     for i, arr in enumerate(arrays):
         arrays[i] = operation(arr)
     return arrays
 
 
 def approx_align(*a: xr.DataArray) -> tuple[xr.DataArray, ...]:
@@ -186,41 +188,40 @@
         The name that should be used for the latitude dimension. Default is 'lat'.
 
     Returns
     -------
     list[xr.DataArray] | xr.DataArray
         A list of averaged xarray Data Arrays.
     """
-    if dims is None:
-        dims = ["lon", "time"]
+    dims_ = ["lon", "time"] if dims is None else dims[:]
     try:
         # If latitude is included, it has to be treated with care to make up for
         # changes in grid cells.
-        dims.remove(lat)
+        dims_.remove(lat)
     except ValueError:
         include_lat = False
     else:
         include_lat = True
     if isinstance(arrays, xr.DataArray):
         if include_lat:
             tmp = _latitude_mean(arrays, lat)
             arrays = tmp.assign_attrs(arrays.attrs)
             tmp.close()
-        arrays = arrays.mean(dim=dims)
+        arrays = arrays.mean(dim=dims_)
         arrays = arrays.assign_attrs(arrays.attrs)
         return arrays
     array = arrays[:]
     for i, arr in enumerate(array):
         if include_lat:
             tmp = _latitude_mean(arr, lat)
             arr_ = tmp.assign_attrs(arr.attrs)
             tmp.close()
         else:
             arr_ = arr
-        array[i] = arr_.mean(dim=dims)
+        array[i] = arr_.mean(dim=dims_)
         array[i] = array[i].assign_attrs(arr_.attrs)
         arr.close()
         arr_.close()
     return array
 
 
 @overload
@@ -485,15 +486,16 @@
     Notes
     -----
     The arrays are assumed to be correctly aligned, consider running `shift_arrays` on
     them before obtaining the median from this function.
     """
     array = arrays[:]
     x_ax = array[0].time
-    y_ax = np.zeros((len(array), len(array[0].data)))
+    shape = (len(array),) + array[0].data.shape
+    y_ax = np.zeros(shape)
     for i, arr in enumerate(array):
         y_ax[i, :] = arr[:].data
     if xarray:
         out = array[0].copy()
         out.data = np.median(y_ax, axis=0)
         out = out.assign_coords(time=x_ax)
         out = out.assign_attrs(array[0].attrs)
@@ -748,20 +750,18 @@
         If the input date format is unknown.
     """
     match dates[0]:
         case float():
             return np.mean(np.diff(dates))
         case datetime.datetime():
             return np.mean(
-                np.diff(
-                    [
-                        eval(datetime.datetime.strftime(i, "%Y+%-m/12+%-d/365"))
-                        for i in dates
-                    ]
-                )
+                np.diff([
+                    eval(datetime.datetime.strftime(i, "%Y+%-m/12+%-d/365"))
+                    for i in dates
+                ])
             )
         case cftime._cftime.DatetimeNoLeap():
             cftime2float_ = dt2float(dates)
             return np.mean(np.diff(cftime2float_))
         case _:
             raise TypeError(
                 f"The input date format is unknown, found {type(dates[0]) = }"
```

### Comparing `volcano_base-2.0.0/.gitignore` & `volcano_base-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/LICENSE` & `volcano_base-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `volcano_base-2.0.0/README.md` & `volcano_base-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v2.0.0</sup> <!-- x-release-please-version -->
+<sup>Latest version: v2.0.1</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

### Comparing `volcano_base-2.0.0/pyproject.toml` & `volcano_base-2.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 [project]
 name = "volcano-base"
-version = "2.0.0"
+version = "2.0.1"
 description = "Download, find and manipulate volcano and climate related time series"
 authors = [{ name = "engeir", email = "engeir@pm.me" }]
 license = "MIT"
 readme = "README.md"
 requires-python = ">= 3.12"
 dependencies = [
-    "returns>=0.22.0",
-    "numpy>=1.26.4",
-    "xarray>=2024.1.1",
-    "matplotlib>=3.8.3",
-    "cftime>=1.6.3",
-    "scipy>=1.12.0",
-    "requests>=2.31.0",
-    "rich>=13.7.0",
-    "dask>=2024.2.0",
-    "h5netcdf>=1.3.0",
-    "datetime>=5.4",
-    "pydantic>=2.6.2",
-    "beautifulsoup4>=4.12.3",
+  "returns>=0.22.0",
+  "numpy>=1.26.4",
+  "xarray>=2024.1.1",
+  "matplotlib>=3.8.3",
+  "cftime>=1.6.3",
+  "scipy>=1.12.0",
+  "requests>=2.31.0",
+  "rich>=13.7.0",
+  "dask>=2024.2.0",
+  "h5netcdf>=1.3.0",
+  "datetime>=5.4",
+  "pydantic>=2.6.2",
+  "beautifulsoup4>=4.12.3",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
-    "pytest>=8.0.0",
-    "pydocstringformatter>=0.7.3",
-    "pydoclint>=0.4.0",
-    "xdoctest>=1.1.3",
-    "pyupgrade>=3.15.0",
-    "pre-commit>=3.6.1",
-    "pre-commit-hooks>=4.5.0",
-    "mypy>=1.8.0",
-    "types-requests>=2.31.0.20240125",
-    "ruff>=0.2.1",
-    "nc-time-axis>=1.4.1",
-    "pyqt5>=5.15.10",
+  "pytest>=8.0.0",
+  "pydocstringformatter>=0.7.3",
+  "pydoclint>=0.4.0",
+  "xdoctest>=1.1.3",
+  "pyupgrade>=3.15.0",
+  "pre-commit>=3.6.1",
+  "pre-commit-hooks>=4.5.0",
+  "mypy>=1.8.0",
+  "types-requests>=2.31.0.20240125",
+  "ruff>=0.3.7",
+  "nc-time-axis>=1.4.1",
+  "pyqt5>=5.15.10",
 ]
 
 [tool.mypy]
 files = ["src"]
 ignore_missing_imports = true
 allow_redefinition = false
 check_untyped_defs = true
@@ -91,24 +91,31 @@
 
 # Same as Black.
 line-length = 88
 
 # Assume Python 3.10
 target-version = "py310"
 
+[tool.ruff.format]
+preview = true
+docstring-code-format = true
+docstring-code-line-length = 88
+
 [tool.ruff.lint]
+preview = true
 select = [ # https://docs.astral.sh/ruff/rules/
-  "B",  # flake8-bugbear
-  "D",  # pydocstyle
-  "E",  # pycodestyle
-  "F",  # pyflakes
-  "I",  # isort
-  "PL", # pylint
-  "Q",  # flake8-quotes
-  "UP", # pyupgrade
+  "B",   # flake8-bugbear
+  "D",   # pydocstyle
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  "I",   # isort
+  "NPY", # numpy specific rules
+  "PL",  # pylint
+  "Q",   # flake8-quotes
+  "UP",  # pyupgrade
 ]
 # Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`)  codes by default.
 # Unlike Flake8, Ruff doesn't enable pycodestyle warnings (`W`) or
 # McCabe complexity (`C901`) by default.
 # select = ["E4", "E7", "E9", "F"]  # These are the default
 # https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
 ignore = [
```

### Comparing `volcano_base-2.0.0/PKG-INFO` & `volcano_base-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: volcano-base
-Version: 2.0.0
+Version: 2.0.1
 Summary: Download, find and manipulate volcano and climate related time series
 Author-email: engeir <engeir@pm.me>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.12
 Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: cftime>=1.6.3
@@ -19,15 +19,15 @@
 Requires-Dist: rich>=13.7.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: xarray>=2024.1.1
 Description-Content-Type: text/markdown
 
 # Core module for volcanic eruption simulation projects
 
-<sup>Latest version: v2.0.0</sup> <!-- x-release-please-version -->
+<sup>Latest version: v2.0.1</sup> <!-- x-release-please-version -->
 
 > [!WARNING]
 >
 > This README reflects the changes made to the main branch. For the most up to date
 > documentation about the version you are using, see the README at the relevant tag.
 
 This repository contains the core elements used across several independent volcanic
```

