# Comparing `tmp/smrt-1.2.4.tar.gz` & `tmp/smrt-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smrt-1.2.4.tar", last modified: Thu Jan 18 22:15:20 2024, max compression
+gzip compressed data, was "smrt-1.3.tar", last modified: Fri Apr 19 10:42:35 2024, max compression
```

## Comparing `smrt-1.2.4.tar` & `smrt-1.3.tar`

### file list

```diff
@@ -1,215 +1,218 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.026148 smrt-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.986148 smrt-1.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.990148 smrt-1.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-01-18 22:15:06.000000 smrt-1.2.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-01-18 22:15:06.000000 smrt-1.2.4/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-18 22:15:06.000000 smrt-1.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-18 22:15:06.000000 smrt-1.2.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-18 22:15:06.000000 smrt-1.2.4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-01-18 22:15:06.000000 smrt-1.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-01-18 22:15:06.000000 smrt-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-01-18 22:15:20.026148 smrt-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-18 22:15:06.000000 smrt-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.994148 smrt-1.2.4/binder/
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-01-18 22:15:06.000000 smrt-1.2.4/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 22:15:06.000000 smrt-1.2.4/binder/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.994148 smrt-1.2.4/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/rtd_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.994148 smrt-1.2.4/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/developer_guidelines.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.emmodel.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.inputs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.microstructure_model.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.permittivity.rst
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.rtsolver.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.substrate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-18 22:15:06.000000 smrt-1.2.4/doc/source/smrt.utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.998148 smrt-1.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 22:15:06.000000 smrt-1.2.4/examples/dmrt_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-01-18 22:15:06.000000 smrt-1.2.4/examples/iba_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    74189 2024-01-18 22:15:06.000000 smrt-1.2.4/examples/iba_onelayer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-18 22:15:06.000000 smrt-1.2.4/examples/iba_onelayer_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-01-18 22:15:06.000000 smrt-1.2.4/examples/iba_sea_ice.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-18 22:15:06.000000 smrt-1.2.4/examples/smrt_memls_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-01-18 22:15:06.000000 smrt-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-18 22:15:20.026148 smrt-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-18 22:15:06.000000 smrt-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.998148 smrt-1.2.4/smrt/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:19.998148 smrt-1.2.4/smrt/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/atmosphere/simple_isotropic_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/atmosphere/test_atmosphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.002148 smrt-1.2.4/smrt/core/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/filelock.py
--rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/fresnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/globalconstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/optional_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25670 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/run_promise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/sensitivity_study.py
--rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/snowpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/test_globalconstants.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/core/test_snowpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.006148 smrt-1.2.4/smrt/emmodel/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/commontest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/dmrt_qca_shortrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/dmrt_qcacp_shortrange.py
--rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/iba.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/iba_maxwell_garnett.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/iba_original.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/nonscattering.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/prescribed_kskaeps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/sce_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/sce_rechtsman08.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/sce_torquato21.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/sce_torquato21_shortrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/sft_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/symsce_torquato21.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/symsce_torquato21_shortrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/test_iba.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/test_iba_original.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/test_prescribed_kskaeps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/test_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/emmodel/test_sft_rayleigh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.010148 smrt-1.2.4/smrt/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/inputs/altimeter_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    39341 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/inputs/make_medium.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/inputs/make_soil.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/inputs/sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/inputs/test_make_medium.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/inputs/test_sensor_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.010148 smrt-1.2.4/smrt/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/coherent_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17341 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/geometrical_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/geometrical_optics_backscatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/iem_fung92.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/iem_fung92_brogioni10.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/radar_calibration_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/test_geometrical_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/test_iem_fung92.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/test_iem_fung92_brogioni10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/transparent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/interface/vector3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.014148 smrt-1.2.4/smrt/microstructure_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/gaussian_random_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/independent_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/sampled_autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/sticky_hard_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/test_autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/test_exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/test_sticky_hard_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/teubner_strey.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/unified_autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/unified_scaled_exponential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/unified_sticky_hard_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/microstructure_model/unified_teubner_strey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.018148 smrt-1.2.4/smrt/permittivity/
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/brine.py
--rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/generic_mixing_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/saline_ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/saline_snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/saline_water.py
--rw-r--r--   0 runner    (1001) docker     (127)    21863 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/snow_mixing_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/test_generic_mixing_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/test_ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/test_saline_ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/test_snow_mixing_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/water.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/wetice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/permittivity/wetsnow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.018148 smrt-1.2.4/smrt/rtsolver/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/rtsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58666 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/rtsolver/dort.py
--rw-r--r--   0 runner    (1001) docker     (127)    32407 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/rtsolver/dort_nonormalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/rtsolver/nadir_lrm_altimetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/rtsolver/test_dort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/rtsolver/test_nadir_lrm_altimetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/rtsolver/waveform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.018148 smrt-1.2.4/smrt/runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/runner/celery_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/runner/dask_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.022148 smrt-1.2.4/smrt/substrate/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/geometrical_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/geometrical_optics_backscatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/iem_fung92.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/iem_fung92_brogioni10.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/radar_calibration_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/reflector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/reflector_backscatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/rough_choudhury79.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/soil_qnh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/soil_wegmuller.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/test_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/test_reflector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/test_rough_choudhury79.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/test_soil_qnh.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/test_soil_wegmuller.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/substrate/transparent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.026148 smrt-1.2.4/smrt/test/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/README
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_coherent_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_dmrtdort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_iba_sea_ice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_integration_geometrical_optics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_integration_iba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_integration_iba_original.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_mixed_emmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_physics_law.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_reflector_backscattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/test/test_soil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.026148 smrt-1.2.4/smrt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/utils/dmrt_qms_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/utils/hut_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/utils/memls_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/utils/memlsscatt.m
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/utils/mpl_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-18 22:15:06.000000 smrt-1.2.4/smrt/utils/repo_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 22:15:20.026148 smrt-1.2.4/smrt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-01-18 22:15:19.000000 smrt-1.2.4/smrt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-01-18 22:15:19.000000 smrt-1.2.4/smrt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 22:15:19.000000 smrt-1.2.4/smrt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-18 22:15:19.000000 smrt-1.2.4/smrt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-18 22:15:19.000000 smrt-1.2.4/smrt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-01-18 22:15:06.000000 smrt-1.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.684015 smrt-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.644015 smrt-1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.648015 smrt-1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-19 10:42:30.000000 smrt-1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-19 10:42:30.000000 smrt-1.3/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-19 10:42:30.000000 smrt-1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-19 10:42:30.000000 smrt-1.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 10:42:30.000000 smrt-1.3/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-19 10:42:30.000000 smrt-1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-19 10:42:30.000000 smrt-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-19 10:42:35.684015 smrt-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-19 10:42:30.000000 smrt-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.648015 smrt-1.3/binder/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-19 10:42:30.000000 smrt-1.3/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 10:42:30.000000 smrt-1.3/binder/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.648015 smrt-1.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-19 10:42:30.000000 smrt-1.3/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-19 10:42:30.000000 smrt-1.3/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 10:42:30.000000 smrt-1.3/doc/rtd_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.652015 smrt-1.3/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/developer_guidelines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.emmodel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.inputs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.microstructure_model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.permittivity.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.rtsolver.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.substrate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-19 10:42:30.000000 smrt-1.3/doc/source/smrt.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.652015 smrt-1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-19 10:42:30.000000 smrt-1.3/examples/dmrt_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-19 10:42:30.000000 smrt-1.3/examples/iba_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74189 2024-04-19 10:42:30.000000 smrt-1.3/examples/iba_onelayer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-19 10:42:30.000000 smrt-1.3/examples/iba_onelayer_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-19 10:42:30.000000 smrt-1.3/examples/iba_sea_ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-19 10:42:30.000000 smrt-1.3/examples/smrt_memls_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-19 10:42:30.000000 smrt-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-19 10:42:35.684015 smrt-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 10:42:30.000000 smrt-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.652015 smrt-1.3/smrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-19 10:42:30.000000 smrt-1.3/smrt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.656015 smrt-1.3/smrt/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-19 10:42:30.000000 smrt-1.3/smrt/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-19 10:42:30.000000 smrt-1.3/smrt/atmosphere/pyrtlib_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-19 10:42:30.000000 smrt-1.3/smrt/atmosphere/pyrtlib_climatology_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-04-19 10:42:30.000000 smrt-1.3/smrt/atmosphere/pyrtlib_era5_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-19 10:42:30.000000 smrt-1.3/smrt/atmosphere/simple_isotropic_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-19 10:42:30.000000 smrt-1.3/smrt/atmosphere/test_atmosphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.660015 smrt-1.3/smrt/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/fresnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/globalconstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/optional_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26951 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/run_promise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/sensitivity_study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14414 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/snowpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/test_globalconstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-19 10:42:30.000000 smrt-1.3/smrt/core/test_snowpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.664015 smrt-1.3/smrt/emmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/commontest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/dmrt_qca_shortrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/dmrt_qcacp_shortrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15632 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/iba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/iba_maxwell_garnett.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/iba_original.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/nonscattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/prescribed_kskaeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/sce_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/sce_rechtsman08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/sce_torquato21.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/sce_torquato21_shortrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/sft_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/symsce_torquato21.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/symsce_torquato21_shortrange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/test_iba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/test_iba_original.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/test_prescribed_kskaeps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/test_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 10:42:30.000000 smrt-1.3/smrt/emmodel/test_sft_rayleigh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.668015 smrt-1.3/smrt/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-19 10:42:30.000000 smrt-1.3/smrt/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-19 10:42:30.000000 smrt-1.3/smrt/inputs/altimeter_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43816 2024-04-19 10:42:30.000000 smrt-1.3/smrt/inputs/make_medium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-19 10:42:30.000000 smrt-1.3/smrt/inputs/make_soil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11278 2024-04-19 10:42:30.000000 smrt-1.3/smrt/inputs/sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-19 10:42:30.000000 smrt-1.3/smrt/inputs/test_make_medium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-19 10:42:30.000000 smrt-1.3/smrt/inputs/test_sensor_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.668015 smrt-1.3/smrt/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/coherent_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17341 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/geometrical_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/geometrical_optics_backscatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/iem_fung92.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/iem_fung92_brogioni10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/radar_calibration_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/test_geometrical_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/test_iem_fung92.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/test_iem_fung92_brogioni10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/transparent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-19 10:42:30.000000 smrt-1.3/smrt/interface/vector3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.672015 smrt-1.3/smrt/microstructure_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/gaussian_random_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/independent_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/sampled_autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/sticky_hard_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/test_autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/test_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/test_sticky_hard_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/teubner_strey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/unified_autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/unified_scaled_exponential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/unified_sticky_hard_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 10:42:30.000000 smrt-1.3/smrt/microstructure_model/unified_teubner_strey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.672015 smrt-1.3/smrt/permittivity/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/brine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/generic_mixing_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/saline_ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/saline_snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/saline_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21937 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/snow_mixing_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/test_generic_mixing_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/test_ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/test_saline_ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/test_snow_mixing_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/water.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/wetice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-19 10:42:30.000000 smrt-1.3/smrt/permittivity/wetsnow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.676015 smrt-1.3/smrt/rtsolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-19 10:42:30.000000 smrt-1.3/smrt/rtsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59445 2024-04-19 10:42:30.000000 smrt-1.3/smrt/rtsolver/dort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32407 2024-04-19 10:42:30.000000 smrt-1.3/smrt/rtsolver/dort_nonormalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-04-19 10:42:30.000000 smrt-1.3/smrt/rtsolver/nadir_lrm_altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-19 10:42:30.000000 smrt-1.3/smrt/rtsolver/test_dort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-19 10:42:30.000000 smrt-1.3/smrt/rtsolver/test_nadir_lrm_altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-19 10:42:30.000000 smrt-1.3/smrt/rtsolver/waveform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.676015 smrt-1.3/smrt/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:30.000000 smrt-1.3/smrt/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-19 10:42:30.000000 smrt-1.3/smrt/runner/celery_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-19 10:42:30.000000 smrt-1.3/smrt/runner/dask_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.680015 smrt-1.3/smrt/substrate/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/geometrical_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/geometrical_optics_backscatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/iem_fung92.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/iem_fung92_brogioni10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/radar_calibration_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/reflector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/reflector_backscatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/rough_choudhury79.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/soil_qnh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/soil_wegmuller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/test_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/test_reflector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/test_rough_choudhury79.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/test_soil_qnh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/test_soil_wegmuller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 10:42:30.000000 smrt-1.3/smrt/substrate/transparent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.680015 smrt-1.3/smrt/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/README
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_coherent_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_dmrtdort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_iba_sea_ice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_integration_geometrical_optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_integration_iba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_integration_iba_original.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_mixed_emmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_physics_law.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_reflector_backscattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-19 10:42:30.000000 smrt-1.3/smrt/test/test_soil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.684015 smrt-1.3/smrt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-19 10:42:30.000000 smrt-1.3/smrt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-04-19 10:42:30.000000 smrt-1.3/smrt/utils/dmrt_qms_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-19 10:42:30.000000 smrt-1.3/smrt/utils/hut_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-04-19 10:42:30.000000 smrt-1.3/smrt/utils/memls_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-19 10:42:30.000000 smrt-1.3/smrt/utils/memlsscatt.m
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-19 10:42:30.000000 smrt-1.3/smrt/utils/mpl_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-19 10:42:30.000000 smrt-1.3/smrt/utils/repo_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:42:35.684015 smrt-1.3/smrt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13311 2024-04-19 10:42:35.000000 smrt-1.3/smrt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-19 10:42:35.000000 smrt-1.3/smrt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:42:35.000000 smrt-1.3/smrt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 10:42:35.000000 smrt-1.3/smrt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-19 10:42:35.000000 smrt-1.3/smrt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 10:42:30.000000 smrt-1.3/tox.ini
```

### Comparing `smrt-1.2.4/.github/workflows/publish.yml` & `smrt-1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/.github/workflows/pytest.yml` & `smrt-1.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/.gitignore` & `smrt-1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/.readthedocs.yml` & `smrt-1.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/LICENSE` & `smrt-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/PKG-INFO` & `smrt-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smrt
-Version: 1.2.4
+Version: 1.3
 Summary: The Snow Microwave Radiative Transfer (SMRT) model is a highly modular model to compute the thermal emission and backscattering coefficient of snowpacks and other cryospheric bodies in the microwave domain.
 Author-email: Ghislain Picard <ghislain.picard@univ-grenoble-alpes.fr>, Melody Sandells <melody.sandells@gmail.com>, Henning Löwe <loewe@slf.ch>
 License: DISCLAIMER: This version of SMRT is an early release. As such, some components may not be fully implemented or may give rise to unexpected behaviour. Please use this software with caution, ask for assistance if needed, and let us know any feedback you may have.
         
         SMRT is Copyright (c) 2016 Ghislain Picard, Melody Sandells, Henning Löwe. Licensed under GNU LGPL:
         
         
@@ -186,14 +186,24 @@
 License-File: LICENSE
 Requires-Dist: numpy<2,>=1.13
 Requires-Dist: pandas>=0.20.3
 Requires-Dist: scipy>=1.0.0
 Requires-Dist: xarray>=0.10.3
 Requires-Dist: numba>=0.40
 Requires-Dist: joblib>=1.0.0
+Provides-Extra: progressbar
+Requires-Dist: tqdm; extra == "progressbar"
+Provides-Extra: pyrtlib
+Requires-Dist: scikit-learn; extra == "pyrtlib"
+Requires-Dist: bs4; extra == "pyrtlib"
+Requires-Dist: netCDF4; extra == "pyrtlib"
+Requires-Dist: requests; extra == "pyrtlib"
+Requires-Dist: cdsapi; extra == "pyrtlib"
+Requires-Dist: cfgrib; extra == "pyrtlib"
+Requires-Dist: pyrtlib; extra == "pyrtlib"
 
 
 Snow Microwave Radiative Transfer model
 =============================================
 
 [SMRT](https://www.smrt-model.science/) is a radiative transfer model to compute emission and backscatter from snowpack.
```

### Comparing `smrt-1.2.4/README.md` & `smrt-1.3/README.md`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/Makefile` & `smrt-1.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/make.bat` & `smrt-1.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/conf.py` & `smrt-1.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/developer_guidelines.rst` & `smrt-1.3/doc/source/developer_guidelines.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/index.rst` & `smrt-1.3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.atmosphere.rst` & `smrt-1.3/doc/source/smrt.atmosphere.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.core.rst` & `smrt-1.3/doc/source/smrt.core.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.emmodel.rst` & `smrt-1.3/doc/source/smrt.emmodel.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.inputs.rst` & `smrt-1.3/doc/source/smrt.inputs.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.interface.rst` & `smrt-1.3/doc/source/smrt.interface.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.microstructure_model.rst` & `smrt-1.3/doc/source/smrt.microstructure_model.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.permittivity.rst` & `smrt-1.3/doc/source/smrt.permittivity.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.rtsolver.rst` & `smrt-1.3/doc/source/smrt.rtsolver.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.substrate.rst` & `smrt-1.3/doc/source/smrt.substrate.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/doc/source/smrt.utils.rst` & `smrt-1.3/doc/source/smrt.utils.rst`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/examples/dmrt_multilayer.py` & `smrt-1.3/examples/dmrt_multilayer.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/examples/iba_multilayer.py` & `smrt-1.3/examples/iba_multilayer.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/examples/iba_onelayer.ipynb` & `smrt-1.3/examples/iba_onelayer.ipynb`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/examples/iba_onelayer_example.py` & `smrt-1.3/examples/iba_onelayer_example.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/examples/iba_sea_ice.py` & `smrt-1.3/examples/iba_sea_ice.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/examples/smrt_memls_legacy.py` & `smrt-1.3/examples/smrt_memls_legacy.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/pyproject.toml` & `smrt-1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     "pandas>=0.20.3",
     "scipy>=1.0.0",
     "xarray>=0.10.3",
     "numba>=0.40",
     "joblib>=1.0.0",
 ]
 
+[project.optional-dependencies]
+    progressbar = ["tqdm"]
+    pyrtlib = ["scikit-learn", "bs4", "netCDF4", "requests", "cdsapi", "cfgrib", "pyrtlib"]
+
 
 [project.urls]
 Homepage = "https://http://smrt-model.science/l"
 Issues = "https://github.com/smrt/smrt-model/issues"
 Documentation = "http://smrt.readthedocs.io/"
 Repository = "https://github.com/smrt-model/smrt.git"
```

### Comparing `smrt-1.2.4/smrt/__init__.py` & `smrt-1.3/smrt/__init__.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/atmosphere/test_atmosphere.py` & `smrt-1.3/smrt/atmosphere/test_atmosphere.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 import numpy as np
 
 from smrt import make_snowpack, make_model, sensor_list
-from smrt.atmosphere.simple_isotropic_atmosphere import SimpleIsotropicAtmosphere, make_atmosphere
+from smrt.atmosphere.simple_isotropic_atmosphere import SimpleIsotropicAtmosphere
 
 
 def test_simple_isotropic_atmosphere():
 
     # prepare inputs
     density = [300, 300]
     temperature = [265, 265]
@@ -36,12 +36,12 @@
     assert abs(res1.TbV() - 227.61318467710458) < 1e-2
     assert abs(res2.TbV() - 214.66092232541834) < 1e-2
 
 
 def test_frequency_dependent_atmosphere():
 
     mu = np.cos(np.arange(0, 90))
-    atmos = make_atmosphere(tbdown={10e9: 15, 21e9: 23}, tbup={10e9: 5, 21e9: 6}, trans={10e9: 1, 21e9: 0.95})
+    atmos = SimpleIsotropicAtmosphere(tb_down={10e9: 15, 21e9: 23}, tb_up={10e9: 5, 21e9: 6}, transmittance={10e9: 1, 21e9: 0.95})
 
-    assert np.all(atmos.tbup(frequency=10e9, costheta=mu, npol=2) == 5)
-    assert np.all(atmos.tbdown(frequency=21e9, costheta=mu, npol=2) == 23)
-    assert np.all(atmos.trans(frequency=21e9, costheta=mu, npol=2) == 0.95)
+    assert np.all(atmos.run(frequency=10e9, costheta=mu, npol=2).tb_up == 5)
+    assert np.all(atmos.run(frequency=21e9, costheta=mu, npol=2).tb_down == 23)
+    assert np.all(atmos.run(frequency=21e9, costheta=mu, npol=2).transmittance == 0.95)
```

### Comparing `smrt-1.2.4/smrt/core/__init__.py` & `smrt-1.3/smrt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/error.py` & `smrt-1.3/smrt/core/error.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/filelock.py` & `smrt-1.3/smrt/core/filelock.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/fresnel.py` & `smrt-1.3/smrt/core/fresnel.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import numpy as np
 from smrt.core.lib import smrt_matrix, abs2
 
 
 def fresnel_coefficients_old(eps_1, eps_2, mu1):
     """compute the reflection in two polarizations (H and V). The equations are only valid for lossless media.
     Applying these equations for (strongly) lossy media result in (large) errors. Don't use it. It is here for reference only.
+    The returned reflection coefficients apply to the electric field. Use abs2(rv), abs2(rh) to obtain the power
+    reflection coefficient.
 
     :param eps_1: permittivity of medium 1.
     :param eps_2: permittivity of medium 2.
     :param mu1: cosine zenith angle in medium 1.
 
     :returns: rv, rh, mu2 the cosine of the angle in medium 2
 """
@@ -31,14 +33,16 @@
 def fresnel_coefficients_maezawa09_classical(eps_1, eps_2, mu1, full_output=False):
     """compute the reflection in two polarizations (H and V) for lossly media with the "classical Fresnel" based
     on Maezawa, H., & Miyauchi, H. (2009). Rigorous expressions for the Fresnel equations at interfaces between absorbing media. 
     Journal of the Optical Society of America A, 26(2), 330. https://doi.org/10.1364/josaa.26.000330
 
     The classical derivation does not respect energy conservation, especially the transmittivity.
     Don't use it. It is here for reference only.
+    The returned reflection coefficients apply to the electric field. Use abs2(rv), abs2(rh) to obtain the power
+    reflection coefficient.
 
     :param eps_1: permittivity of medium 1.
     :param eps_2: permittivity of medium 2.
     :param mu1: cosine zenith angle in medium 1.
 
     :returns: rv, rh, mu2 the cosine of the angle in medium 2
 """
@@ -84,14 +88,16 @@
 
 def fresnel_coefficients_maezawa09_rigorous(eps_1, eps_2, mu1, full_output=False):
     """compute the reflection in two polarizations (H and V) for lossly media with the "rigorous Fresnel" based
     on Maezawa, H., & Miyauchi, H. (2009). Rigorous expressions for the Fresnel equations at interfaces between absorbing media. 
     Journal of the Optical Society of America A, 26(2), 330. https://doi.org/10.1364/josaa.26.000330
 
     The 'rigorous' derivation respect the energy conservation even for strongly loosly media.
+    The returned reflection coefficients apply to the electric field. Use abs2(rv), abs2(rh) to obtain the power
+    reflection coefficient.
 
     :param eps_1: permittivity of medium 1.
     :param eps_2: permittivity of medium 2.
     :param mu1: cosine zenith angle in medium 1.
 
     :returns: rv, rh, mu2 the cosine of the angle in medium 2
 """
@@ -165,15 +171,15 @@
 
     :returns: angle in radians
 """
     return np.arctan(np.sqrt(eps_2 / eps_1).real)
 
 
 def fresnel_reflection_matrix(eps_1, eps_2, mu1, npol):
-    """compute the fresnel reflection matrix for/in medium 1 laying above medium 2.
+    """compute the fresnel power reflection matrix for/in medium 1 laying above medium 2.
 
     :param npol: number of polarizations to return.
     :param eps_1: permittivity of medium 1.
     :param eps_2: permittivity of medium 2.
     :param mu1: cosine zenith angle in medium 1.
 
     :returns: a matrix or the diagional depending on `return_as_diagonal`
@@ -193,15 +199,15 @@
         reflection_coefficients[2] = (rv * np.conj(rh)).real   # TsangI  Eq 7.2.93  
         # It is not sure this equation is valid for strongly loosly materails
 
     return reflection_coefficients
 
 
 def fresnel_transmission_matrix(eps_1, eps_2, mu1, npol):
-    """compute the fresnel reflection matrix for/in medium 1 laying above medium 2.
+    """compute the fresnel power reflection matrix for/in medium 1 laying above medium 2.
 
     :param npol: number of polarizations to return.
     :param eps_1: permittivity of medium 1.
     :param eps_2: permittivity of medium 2.
     :param mu1: cosine zenith angle in medium 1.
 
     :returns: a matrix or the diagional depending on `return_as_diagonal`
```

### Comparing `smrt-1.2.4/smrt/core/globalconstants.py` & `smrt-1.3/smrt/core/globalconstants.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/interface.py` & `smrt-1.3/smrt/core/interface.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/layer.py` & `smrt-1.3/smrt/core/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,14 @@
         given as a complex (or real) value or a function that return a value (see :py:mod:`smrt.permittivity` modules)
         :param inclusion_shape: assumption for shape of air/brine inclusions (so far, "spheres" and "random_needles" (i.e. elongated ellipsoidal inclusions) and "mix_spheres_needles" are implemented)
 
 """
         super().__init__()
 
         self.thickness = thickness
-        # TODO Ghi: send a warning for non valid_args
-        if thickness == 0:
-            raise SMRTError("Layer with thickness = 0 (or even <~wavelength) is not recommended, part of the code does not support it.")
 
         self.temperature = temperature
         if temperature < 0:
             raise SMRTError("Layer temperature is negative. Temperature must be in Kelvin")
 
         self.permittivity_model = permittivity_model
         self.inclusion_shape = inclusion_shape
```

### Comparing `smrt-1.2.4/smrt/core/lib.py` & `smrt-1.3/smrt/core/lib.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/model.py` & `smrt-1.3/smrt/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 import pandas as pd
 
 from .error import SMRTError
 from .result import concat_results
 from .plugin import import_class
 from .sensor import SensorBase
 from .sensitivity_study import SensitivityStudy
-from .progressbar import Progress
 from smrt.core import lib
 
 
 def make_model(emmodel, rtsolver=None, emmodel_options=None, rtsolver_options=None, emmodel_kwargs=None, rtsolver_kwargs=None):
     """create a new model with a given EM model and RT solver. The model is then ready to be run using the :py:meth:`Model.run` method.
     This function is the privileged way to create models compared to class instantiation.
     It supports automatic import of the emmodel and rtsolver modules.
@@ -223,39 +222,38 @@
                 list/generator of simulations, executes the function on each simulation and returns a list of results.
                 'parallel_computation' allows to select between two default (basic) runners (sequential and joblib).
                 Use 'runner' for more advanced parallel distributed computations.
             :returns: result of the calculation(s) as a :py:class:`Results` instance
         """
 
         if atmosphere is not None:
-            raise DeprecationWarning("The atmosphere argument of the run method is going to be depreciated."
-                                     " Setting the 'atmosphere' with make_snowpack (and similar functions) is now the recommended way.")
+            raise DeprecationWarning("""The atmosphere argument of the run method is depreciated.
+Setting the 'atmosphere' through make_snowpack (and similar functions) or using medium = atmosphere + snowpack are now the recommended ways.""")
 
         if not (isinstance(sensor, SensorBase)
                 or (lib.is_sequence(sensor) and all(isinstance(s, SensorBase) for s in sensor))):
             raise SMRTError("the first argument of 'run' must be a sensor or a sequence of sensor")
 
         # determine the simulations to run
         simulations, dimensions = self.prepare_simulations(sensor, snowpack, snowpack_dimension, snowpack_column)
 
         # determine the runner
         if runner is None:
             if parallel_computation:
-                if progressbar:
-                    raise SMRTError("Parallel computation is incompatible with progressbar")
-                runner = JoblibParallelRunner()
+                runner = JoblibParallelRunner(progressbar=progressbar)
             else:
                 runner = SequentialRunner(progressbar=progressbar)
 
         #  run all the simulations (with atmosphere as long as it is not depreciated), the results is a flat list of results
         results = runner(self.run_single_simulation, ((simul, atmosphere) for simul in simulations))
 
         # reshape the results with successive concatenations
         for dimension in reversed(dimensions):
             n = len(dimension[1]) if isinstance(dimension, tuple) else len(dimension)
+            assert n > 0, f"dimension={dimensions}"
             results = [concat_results(results[i: i + n], dimension) for i in range(0, len(results), n)]
 
         assert len(results) == 1
         results = results[0]
 
         if isinstance(snowpack, pd.DataFrame):
             # remove the snowpack_column
@@ -408,41 +406,66 @@
         return RunPromise(self, sensor, snowpack, kwargs)
 
 
 class SequentialRunner(object):
     """Run the simulations sequentially on a single (local) core. This is the most simple way to run smrt simulations, but the 
 efficiency is poor."""
 
-    def __init__(self, progressbar=False):
-        pass
+    def __init__(self, progressbar):
+        """
+        :param progressbar: show a progress bar if True
+        """
+        self.progressbar = progressbar
 
     def __call__(self, function, argument_list):
 
-        return [function(*args) for args in argument_list]
+        if self.progressbar:
+            from tqdm.auto import tqdm
+            argument_list = list(argument_list)
+            return [function(*args) for args in tqdm(argument_list,
+                                                     total=len(argument_list),
+                                                     desc="Running SMRT",
+                                                     )]
+        else:
+            return [function(*args) for args in argument_list]
 
 
 class JoblibParallelRunner(object):
     """Run the simulations on the local machine on all the cores, using the joblib library for parallelism."""
 
-    def __init__(self, backend='loky', n_jobs=-1, max_numerical_threads=1):
+    def __init__(self, progressbar, backend='loky', n_jobs=-1, max_numerical_threads=1):
         """Joblib is a lightweight library for embarasingly parallel task.
 
+    :param progressbar: show a progress bar if True
     :param backend: see joblib documentation. The default 'loky' is the recommended backend.
     :param n_jobs: see joblib documentation. The default is to use all the cores.
     :param max_numerical_threads: :py:func:`~smrt.core.lib.set_max_numerical_threads`. The default avoid miximing different 
     parallelism techniques.
 
 """
         self.n_jobs = n_jobs
         self.backend = backend
+        self.progressbar = progressbar
 
         if max_numerical_threads > 0:
             # it is recommended to set max_numerical_threads to 1, to disable numerical libraries parallelism.
             lib.set_max_numerical_threads(max_numerical_threads)
 
     def __call__(self, function, argument_list):
 
         from joblib import Parallel, delayed
 
-        runner = Parallel(n_jobs=self.n_jobs, backend=self.backend)  # Parallel Runner
-
-        return runner(delayed(function)(*args) for args in argument_list)
+        if self.progressbar:
+            from tqdm.auto import tqdm
+            runner = Parallel(return_as="generator", n_jobs=self.n_jobs, backend=self.backend)  # Parallel Runner
+
+            argument_list = list(argument_list)
+            return list(
+                tqdm(
+                    runner(delayed(function)(*args) for args in argument_list),
+                    total=len(argument_list),
+                    desc="Running SMRT in parallel",
+                )
+            )
+        else:
+            runner = Parallel(n_jobs=self.n_jobs, backend=self.backend)  # Parallel Runner
+            return runner(delayed(function)(*args) for args in argument_list)
```

### Comparing `smrt-1.2.4/smrt/core/plugin.py` & `smrt-1.3/smrt/core/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     try:
         module = importlib.import_module(modulename)
     except ModuleNotFoundError:
         return None
 
     if classname is None:  # search for the first class defined in the module
         for name, obj in inspect.getmembers(module, inspect.isclass):
-            if obj.__module__ == modulename:  # the second condition check if the class was defined in this module
+            if obj.__module__ == modulename and not name.startswith("_"):  # the second condition check if the class was defined in this module
                 classname = name
                 break
 
     if classname is None:
         raise SMRTError("Unable to find a class in the module '%s'" % modulename)
 
     # get the class
```

### Comparing `smrt-1.2.4/smrt/core/progressbar.py` & `smrt-1.3/smrt/core/progressbar.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/result.py` & `smrt-1.3/smrt/core/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,14 +194,39 @@
     def to_series(self, **kwargs):
         """return the result as a series with the channels defined in the sensor as index.
         This requires that the sensor has declared a channel list.
 
         """
         return self.return_as_dataframe('out', channel_axis='column', **kwargs).iloc[0]
 
+    def optical_depth(self):
+        """return the optical depth of each layer tau = ke * thickness, where ke = ka + ks calculated for each layer.
+        This is useful to assess the e-folding depth (aka penetration depth), neglecting the layer transmittance.
+
+        For instance the direct incoming radiation (in active mode) or the radiation emanating directly (in passive
+        mode) can be estimated as::
+
+            intensity = np.exp(-result.optical_depth().cumsum('layer'))
+
+        """
+        if 'ka' not in self.other_data or 'ks' not in self.other_data:
+            raise SMRTError("optical_depth requires that the RT solver provides ka, ks and thickness.")
+
+        ke = self.other_data['ka'] + self.other_data['ks']
+        return ke * self.other_data['thickness']
+
+    def single_scattering_albedo(self):
+        """return the single scattering albedo of each layer: ssalb = ks / (ks + ka). This is useful to assess if
+        multiple scattering is significant (e.g. if ssalb > 0.2).
+        """
+        if 'ka' not in self.other_data or 'ks' not in self.other_data:
+            raise SMRTError("single_scattering_albedo requires that the RT solver provides ka and ks.")
+
+        return self.other_data['ks'] / (self.other_data['ka'] + self.other_data['ks'])
+
 
 class PassiveResult(Result):
 
     mode = 'P'
 
     def sel_data(self, channel=None, **kwargs):
         # this function allows selection as xarray.DataArray.sel and in addition by channel if a channel_map is defined.
```

### Comparing `smrt-1.2.4/smrt/core/run_promise.py` & `smrt-1.3/smrt/core/run_promise.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/sensitivity_study.py` & `smrt-1.3/smrt/core/sensitivity_study.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/sensor.py` & `smrt-1.3/smrt/core/sensor.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/snowpack.py` & `smrt-1.3/smrt/core/snowpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,17 @@
 
         :Example:
 
         # duplicate the top layer:    
         newsp = sp.layers[0] + wetsp
 
 """
+        if other == 0:
+            return self
+
         self.check_addition_validity(other)
 
         if isinstance(other, SubstrateBase):
             return Snowpack(layers=self.layers,
                             interfaces=self.interfaces,
                             atmosphere=self.atmosphere,
                             substrate=other)
@@ -261,15 +264,17 @@
 
     def __iadd__(self, other):  # just for optimization
         """Inplace addition of object to snowpack. See :func:`~snowpack.Snowpack.__add__` description.
 
 """
         self.check_addition_validity(other)
 
-        if isinstance(other, SubstrateBase):
+        if other == 0:
+            pass
+        elif isinstance(other, SubstrateBase):
             self.substrate = other
         elif isinstance(other, Layer):
             self.layers.append(copy.deepcopy(other))
             self.interfaces.append(copy.deepcopy(self.interfaces[-1]))  # duplicate the bottomost layer
             self.update_layer_number()
         else:
             self.layers += other.layers
```

### Comparing `smrt-1.2.4/smrt/core/test_interface.py` & `smrt-1.3/smrt/core/test_interface.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/test_lib.py` & `smrt-1.3/smrt/core/test_lib.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/test_result.py` & `smrt-1.3/smrt/core/test_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,39 @@
 
 import pytest
 
 from smrt.core import result
 
 
 # Tests written in response to -ve intensity bug in result.py
+layer_coord = ('layer', [0, 1, 2])
+
 res_example = result.ActiveResult([[[[4.01445680e-03, 3.77746658e-03, 0.00000000e+00]],
                                     [[3.83889082e-03, 3.85904771e-03, 0.00000000e+00]],
                                     [[2.76453599e-20, -2.73266027e-20, 0.00000000e+00]]]],
                                   coords=[('theta', [35]), ('polarization', ['V', 'H', 'U']),
                                           ('theta_inc', [35]), ('polarization_inc', ['V', 'H', 'U'])],
                                   channel_map={'VV': dict(polarization='V', polarization_inc='V'),
-                                               'VH': dict(polarization='H', polarization_inc='V')})
+                                               'VH': dict(polarization='H', polarization_inc='V')},
+                                  other_data={'ks': xr.DataArray([1., 2., 3.], coords=[layer_coord]),
+                                              'ka': xr.DataArray([3., 2., 1.], coords=[layer_coord]),
+                                              'thickness': xr.DataArray([0.1, 0.1, 0.1], coords=[layer_coord])}
+                                  )
 
 res_example2 = result.ActiveResult([[[[4e-03, 3e-03, 0]],
                                      [[3e-03, 3.85904771e-03, 0]],
                                      [[0, 0, 0.00000000e+00]]]],
                                    coords=[('theta', [45]), ('polarization', ['V', 'H', 'U']),
                                            ('theta_inc', [45]), ('polarization_inc', ['V', 'H', 'U'])],
                                    channel_map={'VV': dict(polarization='V', polarization_inc='V'),
-                                                'VH': dict(polarization='H', polarization_inc='V')})
+                                                'VH': dict(polarization='H', polarization_inc='V')},
+                                  other_data={'ks': xr.DataArray([2., 4., 6.], coords=[layer_coord]),
+                                              'ka': xr.DataArray([3., 2., 1.], coords=[layer_coord]),
+                                              'thickness': xr.DataArray([0.1, 0.1, 0.1], coords=[layer_coord])}
+                                   )
 
 
 def test_methods():
     assert hasattr(res_example, "sigma")
     assert not hasattr(res_example, "Tb")
 
 
@@ -73,15 +83,15 @@
     assert 'VV' in df.columns
     assert 'VH' in df.columns
 
     np.testing.assert_allclose(df['VV'], -13.8379882755357)
     np.testing.assert_allclose(df['VH'], -14.0321985560285)
 
 
-@pytest.mark.skipif(sys.version_info < (3,8),
+@pytest.mark.skipif(sys.version_info < (3, 8),
                     reason="requires python3.8 and higher")
 def test_to_dataframe_without_channel_axis():
     df = res_example.to_dataframe(channel_axis=None)
     print(df)  # this test fail for old version of xarray
     np.testing.assert_allclose(df.loc[(35, 'V', 'V'), :], (35, -13.8379882755357))
     np.testing.assert_allclose(df.loc[(35, 'H', 'V'), :], (35, -14.0321985560285))
 
@@ -106,14 +116,24 @@
 
 
 def test_concat_results_other_data():
 
     res = copy.deepcopy(res_example)
     res2 = copy.deepcopy(res_example2)
 
-    res.other_data['other_value'] = xr.DataArray([0.1, 0.2], coords=[('layer', [0, 1])])
+    allresult = result.concat_results((res, res2), coord=('dim0', [0, 1]))
+
+    assert allresult.other_data['ks'].dims == ('dim0', 'layer')
 
-    res2.other_data['other_value'] = xr.DataArray([0.2, 0.3], coords=[('layer', [0, 1])])
 
-    allresult = result.concat_results((res, res2), coord=('dim0', [0, 1]))
+def test_single_scattering_albedo():
+
+    ssalb = res_example.single_scattering_albedo()
+
+    print(ssalb)
+    assert np.allclose(ssalb, np.array([1 / 4, 2 / 4, 3 / 4]))
+
+
+def test_optical_depth():
+    tau = res_example.optical_depth()
 
-    assert allresult.other_data['other_value'].dims == ('dim0', 'layer')
+    assert np.allclose(tau, [0.4, 0.4, 0.4])
```

### Comparing `smrt-1.2.4/smrt/core/test_sensor.py` & `smrt-1.3/smrt/core/test_sensor.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/core/test_snowpack.py` & `smrt-1.3/smrt/core/test_snowpack.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/__init__.py` & `smrt-1.3/smrt/emmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/common.py` & `smrt-1.3/smrt/emmodel/common.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/commontest.py` & `smrt-1.3/smrt/emmodel/commontest.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/dmrt_qca_shortrange.py` & `smrt-1.3/smrt/emmodel/dmrt_qca_shortrange.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/dmrt_qcacp_shortrange.py` & `smrt-1.3/smrt/emmodel/dmrt_qcacp_shortrange.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/iba.py` & `smrt-1.3/smrt/emmodel/iba.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/iba_maxwell_garnett.py` & `smrt-1.3/smrt/emmodel/iba_maxwell_garnett.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import numpy as np
 
 from smrt.permittivity.generic_mixing_formula import maxwell_garnett
 from .iba import IBA
 
 
-class IBA_MaxewellGarnett(IBA):
+class IBA_MaxwellGarnett(IBA):
 
     """
     Modified Improved Born Approximation electromagnetic model class.
 
     As with all electromagnetic modules, this class is used to create an electromagnetic
     object that holds information about the effective permittivity, extinction coefficient and
     phase function for a particular snow layer. Due to the frequency dependence, information
@@ -36,19 +36,19 @@
     :param sensor: object containing sensor characteristics
     :param layer: object containing snow layer characteristics (single layer)
 
     """
     effective_permittivity_model = staticmethod(maxwell_garnett)
 
 
-    def mean_sq_field_ratio(self, e0, eps):
+    def mean_sq_field_ratio(self):
         """ Mean squared field ratio calculation
 
         Uses layer effective permittivity
 
         :param e0: background relative permittivity
         :param eps: scattering constituent relative permittivity
 
         """
-        apparent_permittivity = e0
-        y2 = (1. / 3.) * np.sum(np.absolute(apparent_permittivity / (apparent_permittivity + (eps - e0) * self.depol_xyz))**2.)
+        apparent_permittivity = self.e0
+        y2 = (1. / 3.) * np.sum(np.absolute(apparent_permittivity / (apparent_permittivity + (self.eps - self.e0) * self.depol_xyz))**2.)
         return y2
```

### Comparing `smrt-1.2.4/smrt/emmodel/iba_original.py` & `smrt-1.3/smrt/emmodel/iba_original.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/nonscattering.py` & `smrt-1.3/smrt/emmodel/nonscattering.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/prescribed_kskaeps.py` & `smrt-1.3/smrt/emmodel/prescribed_kskaeps.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/rayleigh.py` & `smrt-1.3/smrt/emmodel/rayleigh.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/sce_common.py` & `smrt-1.3/smrt/emmodel/sce_common.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/sce_rechtsman08.py` & `smrt-1.3/smrt/emmodel/sce_rechtsman08.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/sce_torquato21.py` & `smrt-1.3/smrt/emmodel/sce_torquato21.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/sce_torquato21_shortrange.py` & `smrt-1.3/smrt/emmodel/sce_torquato21_shortrange.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/sft_rayleigh.py` & `smrt-1.3/smrt/emmodel/sft_rayleigh.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/symsce_torquato21.py` & `smrt-1.3/smrt/emmodel/symsce_torquato21.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/symsce_torquato21_shortrange.py` & `smrt-1.3/smrt/emmodel/symsce_torquato21_shortrange.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/test_iba.py` & `smrt-1.3/smrt/emmodel/test_iba.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/test_iba_original.py` & `smrt-1.3/smrt/emmodel/test_iba_original.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/test_prescribed_kskaeps.py` & `smrt-1.3/smrt/emmodel/test_prescribed_kskaeps.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/test_rayleigh.py` & `smrt-1.3/smrt/emmodel/test_rayleigh.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/emmodel/test_sft_rayleigh.py` & `smrt-1.3/smrt/emmodel/test_sft_rayleigh.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/inputs/__init__.py` & `smrt-1.3/smrt/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/inputs/altimeter_list.py` & `smrt-1.3/smrt/inputs/altimeter_list.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/inputs/make_medium.py` & `smrt-1.3/smrt/inputs/make_medium.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,31 @@
     from smrt import make_snowpack
 
     sp = make_snowpack([1000], density=[300], microstructure_model='sticky_hard_spheres', radius=[0.3e-3], stickiness=0.2)
 
 creates a semi-infinite snowpack made of sticky hard spheres with radius 0.3mm and stickiness 0.2.
 The :py:obj:`~smrt.core.Snowpack` object is in the `sp` variable.
 
+Note that any layer with zero thickness is completely removed in most of these functions (as well as its top interface), 
+and a transparent layer is added if the resulting medium does not have any layer. This allows simulation of bare soil and bare ice 
+more easily. It is important to understand that any layer with non-zero thickness, even much smaller than the wavelength, even
+10^-20 m, has an impact in the radiative transfer framework due to the reflection, transmission and refraction. In reality,
+and according to the wave theory such sub-wavelength layers and their interface should have reduced or close to zero impact.
+It is the responsability of the user to ensure that such thin layers (less than a quarter of wavelength) are removed from
+the snowpack. Alternatively setting the `process_coherent_layers` option when using the
+`smrt.rtsolver.dort` solver allows to deal with sub-wavelength layers provided they are isolated between two thick layers.
+
 Note that `make_snowpack` is directly imported from `smrt` instead of `smrt.inputs.make_medium`. This feature is for convenience.
 
 """
 
 import itertools
 import collections
+import inspect
+from warnings import warn
 
 import numpy as np
 import pandas as pd
 
 from smrt.core.snowpack import Snowpack
 from smrt.core.interface import make_interface
 from smrt.core.plugin import import_class
@@ -117,15 +128,15 @@
                   substrate=None,
                   atmosphere=None,
                   **kwargs):
     """
     Build a multi-layered snowpack. Each parameter can be an array, list or a constant value.
 
     :param thickness: thicknesses of the layers in meter (from top to bottom). The last layer thickness can be "numpy.inf"
-        for a semi-infinite layer.
+        for a semi-infinite layer. Any layer with zero thickness is removed.
     :param microstructure_model: microstructure_model to use (e.g. sticky_hard_spheres or independent_sphere or exponential).
     :param surface: type of surface interface, flat/fresnel is the default.  If surface and interface are both set,
         the interface must be a constant refering to all the "internal" interfaces.
     :param interface: type of interface, flat/fresnel is the default. It is usually a string for the interfaces
         without parameters (e.g. Flat or Transparent) or is created with :py:func:`~smrt.core.interface.make_interface` in more complex cases.
         Interface can be a constant or a list. In the latter case, its length must be the same as the number of layers,
         and interface[0] refers to the surface interface.
@@ -152,22 +163,30 @@
     lib.check_argument_size(density, len(thickness), "density")
     lib.check_argument_size(kwargs, len(thickness))
 
     if surface is not None and lib.is_sequence(interface):
         raise SMRTError("Setting both 'surface' and 'interface' arguments is ambiguous when inteface is a list or any sequence.")
 
     for i, dz in enumerate(thickness):
+        if dz <= 0:
+            continue
         layer = make_snow_layer(dz, lib.get(microstructure_model, i, "microstructure_model"),
                                 density=lib.get(density, i, "density"),
                                 **lib.get(kwargs, i))
 
-        # add the interface
-        linterface = lib.get(interface, i, "interface") if (i > 0) or (surface is None) else surface
+        # add the interface or surface for the first non-zero layer
+        linterface = lib.get(interface, i, "interface") if surface is None else surface
+        surface = None
         sp.append(layer, interface=make_interface(linterface))
 
+    # snowpack without layer is accepted as input of this function, but SMRT prefers to have one internally.
+    # we make a transparent volume
+    if sp.nlayer == 0:
+        sp = add_transparent_layer(sp)
+
     return sp
 
 
 def make_snow_layer(layer_thickness,
                     microstructure_model,
                     density,
                     temperature=FREEZING_POINT,
@@ -206,14 +225,17 @@
         # default ice permittivity model, use ice_permittivity_maetzler06 for dry snow and add support for wet snow
         from ..permittivity.wetice import wetice_permittivity_bohren83
         ice_permittivity_model = wetice_permittivity_bohren83
 
     eps_1 = background_permittivity_model
     eps_2 = ice_permittivity_model
 
+    warn_mixing_formula(background_permittivity_model, "background_permittivity_model")
+    warn_mixing_formula(ice_permittivity_model, "ice_permittivity_model")
+
     if isinstance(microstructure_model, str):
         microstructure_model = get_microstructure_model(microstructure_model)
 
     # if liquid_water is not None:
     #    raise smrt_warn("The argument 'liquid_water' is going to be depreciated because its definition is uncommon"
     #                    " in the snow community. Use instead volumetric_liquid_water. Check the definition")
 
@@ -332,15 +354,15 @@
 
     First-year and multi-year ice is equivalent only if scattering and porosity are nulls. It is important to understand that
     in multi-year ice scattering by brine pockets is neglected because scattering is due to air bubbles and the emmodel
     implemented up to now are not able to deal with three-phase media.
 
     :param ice_type: Ice type. Options are "firstyear", "multiyear", "fresh"
     :param thickness: thicknesses of the layers in meter (from top to bottom). The last layer thickness can be "numpy.inf"
-        for a semi-infinite layer.
+        for a semi-infinite layer. Any layer with zero thickness is removed.
     :param temperature: temperature of ice/water in K
     :param brine_inclusion_shape: assumption for shape of brine inclusions. So far, "spheres" or "random_needles"
         (i.e. elongated ellipsoidal inclusions), and "mix" (a mix of the two) are implemented.
     :param salinity: salinity of ice/water in kg/kg (see PSU constant in smrt module). Default is 0. If neither salinity
         nor brine_volume_fraction are given, the ice column is considered to consist of fresh water ice.
     :param brine_volume_fraction: brine / liquid water fraction in sea ice, optional parameter, if not given brine volume fraction is
         calculated from temperature and salinity in ~.smrt.permittivity.brine_volume_fraction
@@ -381,31 +403,39 @@
                  "interface", "kwargs"]:
         lib.check_argument_size(locals()[name], n)
 
     if surface is not None and lib.is_sequence(interface):
         raise SMRTError("Setting both 'surface' and 'interface' arguments is ambiguous when inteface is a list or any sequence.")
 
     for i, dz in enumerate(thickness):
+        if dz <= 0:
+            continue
         layer = make_ice_layer(ice_type,
                                dz, temperature=lib.get(temperature, i),
                                salinity=lib.get(salinity, i),
                                microstructure_model=lib.get(microstructure_model, i),
                                brine_inclusion_shape=lib.get(brine_inclusion_shape, i),
                                brine_volume_fraction=lib.get(brine_volume_fraction, i),
                                porosity=lib.get(porosity, i),
                                density=lib.get(density, i),
                                brine_permittivity_model=lib.get(brine_permittivity_model, i),
                                ice_permittivity_model=lib.get(ice_permittivity_model, i),
                                saline_ice_permittivity_model=lib.get(saline_ice_permittivity_model, i),
                                **lib.get(kwargs, i))
 
-        # add the interface
-        linterface = lib.get(interface, i, "interface") if (i > 0) or (surface is None) else surface
+        # add the interface or surface for the first non-zero layer
+        linterface = lib.get(interface, i, "interface") if surface is None else surface
+        surface = None
         sp.append(layer, interface=make_interface(linterface))
 
+    # snowpack without layer is accepted as input of this function, but SMRT prefers to have one internally.
+    # we make a transparent volume
+    if sp.nlayer == 0:
+        sp = add_transparent_layer(sp)
+
     return sp
 
 
 def make_ice_layer(ice_type,
                    layer_thickness,
                    temperature,
                    salinity,
@@ -421,15 +451,15 @@
                    **kwargs):
     """Make an ice layer for a given microstructure_model (see also :py:func:`~smrt.inputs.make_medium.make_ice_column`
     to create many layers). The microstructural parameters depend on the microstructural model and should be given as
     additional arguments to this function. To know which parameters are required or optional, refer to the documentation
     of the specific microstructure model used.
 
     :param ice_type: Assumed ice type
-    :param layer_thickness: thickness of ice layer in m
+    :param layer_thickness: thickness of ice layer in m. 
     :param temperature: temperature of layer in K
     :param salinity: (firstyear and multiyear) salinity in kg/kg (see PSU constant in smrt module)
     :param brine_inclusion_shape: (firstyear and multiyear) assumption for shape of brine inclusions (so far,
         "spheres" and "random_needles" (i.e. elongated ellipsoidal inclusions), and "mix_spheres_needles" are implemented)
     :param brine_volume_fraction: (firstyear and multiyear) brine / liquid water fraction in sea ice, optional parameter,
         if not given brine volume fraction is calculated from temperature and salinity in ~.smrt.permittivity.brine_volume_fraction
     :param density: (multiyear) density of ice layer in kg m :sup:`-3`. If not given, density is calculated from temperature,
@@ -454,21 +484,27 @@
     if ice_type in ['firstyear', 'multiyear']:
         if brine_volume_fraction is None:
             brine_volume_fraction = brine_volume(temperature, salinity)
 
         if brine_permittivity_model is None:
             brine_permittivity_model = brine_permittivity_stogryn85  # default brine permittivity model
 
+        warn_mixing_formula(brine_permittivity_model, "brine_permittivity_model")
+        warn_mixing_formula(saline_ice_permittivity_model, "saline_ice_permittivity_model")
+
+    warn_mixing_formula(ice_permittivity_model, "ice_permittivity_model")
+
     if density is None:
         density = bulk_ice_density(temperature, salinity, porosity)
     elif porosity == 0:
         porosity = np.clip(1. - density / bulk_ice_density(temperature, salinity, porosity=0), 0., 1.)
     else:
         raise SMRTError("Setting density and porosity is invalid")
 
+
     # specific setup
     if ice_type == "firstyear":
         # scatterers permittivity
         eps_2 = brine_permittivity_model
 
         # background permittivity
         if ice_permittivity_model is None:
@@ -551,27 +587,31 @@
 
     lay.read_only_attributes = {'ice_type', 'density', 'porosity'}
 
     return lay
 
 
 def make_water_body(layer_thickness=1000,
-                    temperature=273,
+                    temperature=FREEZING_POINT,
                     salinity=0,
                     water_permittivity_model=None,
                     surface=None,
                     atmosphere=None,
                     substrate=None):
     """Make a water body with a single layer of water at given temperature and salinity.
 
     Note that water is a very strong absorber even fresh water, it is unlikely that the layers under a water body 
     could be seen by microwaves. If really needed anyway, a multi-layer water body or
-     a water layer on another medium (e.g. ice) can be build using the addition operator.
+        a water layer on another medium (e.g. ice) can be build using the addition operator. 
 
-    :param layer_thickness: thickness of ice layer in m
+    Note that water has a strong real permittivity and when used in
+        combinaison with the DORT solver, it is recommended to increase the `n_max_stream` option of the solver to get
+        enough streams in the air (see about stream Picard et al. 2018).
+
+    :param layer_thickness: thickness of ice layer in m. If the thickness is zero, a transparent layer is added.
     :param temperature: temperature of layer in K
     :param salinity: salinity in kg/kg (see PSU constant in smrt module)
     :param water_permittivity_model: water permittivity formulation (default is seawater_permittivity_klein76)
     :param surface: type of surface interface. Flat surface (Fresnel coefficient) is the default.
     :param substrate: the substrate under the water layer.
 
 """
@@ -581,19 +621,24 @@
     layer = make_water_layer(layer_thickness,
                              temperature=temperature,
                              salinity=salinity,
                              water_permittivity_model=water_permittivity_model)
     # add the layer and the interface interface
     sp.append(layer, interface=make_interface(surface))
 
+    if layer_thickness <= 0:
+        # snowpack without layer is accepted as input of this function, but SMRT prefers to have one internally.
+        # we make a transparent volume
+        sp = add_transparent_layer(sp)
+
     return sp
 
 
 def make_water_layer(layer_thickness,
-                     temperature=273,
+                     temperature=FREEZING_POINT,
                      salinity=0,
                      water_permittivity_model=None, **kwargs):
     """Make a water layer at given temperature and salinity.
 
     :param layer_thickness: thickness of ice layer in m
     :param temperature: temperature of layer in K
     :param salinity: salinity in kg/kg (see PSU constant in smrt module)
@@ -680,24 +725,24 @@
 
     if rho < 0:
         raise SMRTError("Ice density may not be negative.")
 
     return rho
 
 
-def make_generic_stack(thickness, temperature=273, ks=0, ka=0, effective_permittivity=1,
+def make_generic_stack(thickness, temperature=FREEZING_POINT, ks=0, ka=0, effective_permittivity=1,
                        interface=None,
                        substrate=None,
                        atmosphere=None):
     """
     build a multi-layered medium with prescribed scattering and absorption coefficients and effective permittivity.
     Must be used with presribed_kskaeps emmodel.
 
     :param thickness: thicknesses of the layers in meter (from top to bottom). The last layer thickness can be "numpy.inf" for
-        a semi-infinite layer.
+        a semi-infinite layer. Any layer with zero thickness is removed.
     :param temperature: temperature of layers in K
     :param ks: scattering coefficient of layers in m^-1
     :param ka: absorption coefficient of layers in m^-1
     :param interface: type of interface, flat/fresnel is the default
 
 """
 # TODO: Add an example
@@ -709,27 +754,34 @@
 
     sp = Snowpack(substrate=substrate, atmosphere=atmosphere)
 
     if not isinstance(thickness, collections.abc.Iterable):
         raise SMRTError("The thickness argument must be iterable, that is, a list of numbers, numpy array or pandas Series or DataFrame.")
 
     for i, dz in enumerate(thickness):
+        if dz <= 0:
+            continue
         layer = make_generic_layer(dz,
                                    ks=lib.get(ks, i, "ks"),
                                    ka=lib.get(ka, i, "ka"),
                                    effective_permittivity=lib.get(effective_permittivity, i, "effective_permittivity"),
                                    temperature=lib.get(temperature, i, "temperature")
                                    )
 
         sp.append(layer, lib.get(interface, i))
 
+    # snowpack without layer is accepted as input of this function, but SMRT prefers to have one internally.
+    # we make a transparent volume
+    if sp.nlayer == 0:
+        sp = add_transparent_layer(sp)
+
     return sp
 
 
-def make_generic_layer(layer_thickness, ks=0, ka=0, effective_permittivity=1, temperature=273):
+def make_generic_layer(layer_thickness, ks=0, ka=0, effective_permittivity=1, temperature=FREEZING_POINT):
     """Make a generic layer with prescribed scattering and absorption coefficients and effective permittivity.
     Must be used with presribed_kskaeps emmodel.
 
     :param layer_thickness: thickness of ice layer in m
     :param temperature: temperature of layer in K
     :param ks: scattering coefficient of layers in m^-1
     :param ka: absorption coefficient of layers in m^-1
@@ -743,14 +795,53 @@
     lay.effective_permittivity = effective_permittivity
     lay.ks = float(ks)
     lay.ka = float(ka)
 
     return lay
 
 
+def add_transparent_layer(snowpack):
+    """
+    add a transparent layer to the snowpack
+
+    :param snowpack: the substrate under the transparent layer.
+
+   e.g.::
+
+       sp = add_transparent_layer(sp)
+
+"""
+
+    layer = Layer(thickness=0,
+                  microstructure_model=get_microstructure_model("homogeneous"),
+                  frac_volume=0,
+                  temperature=0,
+                  permittivity_model=(1, 1))
+
+    snowpack.append(layer, interface=make_interface("transparent"))
+
+    return snowpack
+
+
+def make_transparent_volume(substrate=None,
+                            atmosphere=None):
+    """
+    build a transparent single-layer snowpack. This is useful to run SMRT without any 'real' layer.
+
+    :param substrate: the substrate under the transparent layer.
+
+   e.g.::
+
+       sp = make_transparent_volume()
+
+"""
+
+    return add_transparent_layer(Snowpack(substrate=substrate, atmosphere=atmosphere))
+
+
 def make_atmosphere(atmosphere_model, **kwargs):
     """
     make a atmospheric single-layer using the prescribed atmosphere model.
     Warning: this function is subject to change in the future when refactoring how SMRT deals with atmosphere.
 
     :param atmosphere_model: the name of the model to use. The available models are in smrt.atmosphere.
     :param **kwargs: all the parameters used by the atmosphere_model.
@@ -803,7 +894,20 @@
             # this is unusual
             raise SMRTError("z is ascending and has negative values, which an ambiguous situation")
 
     else:
         raise SMRTError("The z argument is not sorted")
 
     return np.diff(z)
+
+
+def warn_mixing_formula(permittivity_model, name):
+
+    if not callable(permittivity_model):
+        return
+
+    signature = inspect.signature(permittivity_model).parameters
+    if ('density' in signature) or ('frac_volume' in signature):
+        warn(f"""The permittivity model set for the {name} argument seems to be a mixing formula. Such formula should
+        not be used in this function but rather using derived_IBA or derive_SymSCE or equivalent functions. Check the
+        module documentation of the permittivity model.""",
+             stacklevel=2)
```

### Comparing `smrt-1.2.4/smrt/inputs/make_soil.py` & `smrt-1.3/smrt/inputs/make_soil.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,25 +129,25 @@
 def soil_dielectric_constant_hut(frequency, tempK, SM, sand, clay, dm_rho):
 
     # Parameters for soil dielectric constant calculation with water
     ew_inf = 4.9
 
     tempC = tempK - 273.15
 
-    if tempC > 0:  # liquid water
+    if tempC >= 0:  # liquid water
         # calculates real and imag. part of water dielectricity (code HUT 20.12.95 [epsw.m]; K.Tigerstedt)
         ew0 = 87.74 - 0.40008 * tempC + 9.398e-4 * tempC**2 + 1.410e-6 * tempC**3
         d = 25 - tempC
         alfa = 2.033e-2 + 1.266e-4 * d + 2.464e-6 * d**2
         tw = 1 / (2 * np.pi) * (1.1109e-10 - 3.824e-12 * tempC + 6.938e-14 * tempC**2 - 5.096e-16 * tempC**3)
 
         ew_r = ew_inf + (ew0 - ew_inf) / (1 + (2 * np.pi * frequency * tw)**2)
         ew_i = (ew0 - ew_inf) * 2 * np.pi * frequency * tw / (1 + (2 * np.pi * frequency * tw)**2)
     else:
-        raise NotImplementedError("not implemented")
+        raise SMRTError("soil_dielectric_constant_hut requires above freezing point temperatures")
 #      !option for salt consideration (Mätzler 1987)
 #      !iei_S =A/M+B*M**C                 !impure ice
 #      !iei_P=Ap/M+Bp*M**Cp                 !pure ice
 #      !delta_iei = iei_S - iei_P
 #      !ew_i=ew_i+delta_iei*SS/13
 
     beta = 1.09 - 0.11 * sand + 0.18 * clay
```

### Comparing `smrt-1.2.4/smrt/inputs/sensor_list.py` & `smrt-1.3/smrt/inputs/sensor_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
     """Configuration for the passive (mode=P) and active (mode=A) sensor on smap
 
         This function returns either a passive sensor at 1.4 GHz (L-band) sensor or an active sensor at 1.26 GHz. The incidence angle is 40°.
 
     """
 
     if mode == 'P':
-        return passive(1.4e9, theta=theta, channel_map={pola: dict(polarization=pola) for pola in 'HV'}, name='smap')
+        return passive(1.4e9, theta=theta, channel_map={'01' + pola: dict(polarization=pola) for pola in 'HV'}, name='smap')
     elif mode == 'A':
         return active(1.26e9, theta=theta, theta_inc=theta,
                       channel_map={channel: dict(polarization=channel[1], polarization_inc=channel[0]) for channel in ['HH', 'VV', 'HV']},
                       name='smap')
     else:
         raise SMRTError('mode must by A (active) or P (passive')
 
@@ -291,12 +291,15 @@
 def extract_configuration(channel_map):
 
     keys = ['frequency', 'polarization', 'theta', 'polarization_inc', 'theta_inc']
 
     configuration = dict()
     for k in keys:
         try:
-            configuration[k] = list({channel_map[ch][k] for ch in channel_map})
+            x = np.unique([channel_map[ch][k] for ch in channel_map])
+            if len(x) == 1:
+                x = x[0]
+            configuration[k] = x
         except KeyError:
             continue
 
     return configuration
```

### Comparing `smrt-1.2.4/smrt/inputs/test_sensor_list.py` & `smrt-1.3/smrt/inputs/test_sensor_list.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/coherent_flat.py` & `smrt-1.3/smrt/interface/coherent_flat.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/flat.py` & `smrt-1.3/smrt/interface/flat.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/geometrical_optics.py` & `smrt-1.3/smrt/interface/geometrical_optics.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/geometrical_optics_backscatter.py` & `smrt-1.3/smrt/interface/geometrical_optics_backscatter.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/iem_fung92.py` & `smrt-1.3/smrt/interface/iem_fung92.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/iem_fung92_brogioni10.py` & `smrt-1.3/smrt/interface/iem_fung92_brogioni10.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/radar_calibration_sphere.py` & `smrt-1.3/smrt/interface/radar_calibration_sphere.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/test_geometrical_optics.py` & `smrt-1.3/smrt/interface/test_geometrical_optics.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/test_iem_fung92.py` & `smrt-1.3/smrt/interface/test_iem_fung92.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/test_iem_fung92_brogioni10.py` & `smrt-1.3/smrt/interface/test_iem_fung92_brogioni10.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/transparent.py` & `smrt-1.3/smrt/interface/transparent.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/interface/vector3.py` & `smrt-1.3/smrt/interface/vector3.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/__init__.py` & `smrt-1.3/smrt/microstructure_model/__init__.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/autocorrelation.py` & `smrt-1.3/smrt/microstructure_model/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/exponential.py` & `smrt-1.3/smrt/microstructure_model/exponential.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/gaussian_random_field.py` & `smrt-1.3/smrt/microstructure_model/gaussian_random_field.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/homogeneous.py` & `smrt-1.3/smrt/microstructure_model/homogeneous.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/independent_sphere.py` & `smrt-1.3/smrt/microstructure_model/independent_sphere.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/sampled_autocorrelation.py` & `smrt-1.3/smrt/microstructure_model/sampled_autocorrelation.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/sticky_hard_spheres.py` & `smrt-1.3/smrt/microstructure_model/sticky_hard_spheres.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/teubner_strey.py` & `smrt-1.3/smrt/microstructure_model/teubner_strey.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/unified_scaled_exponential.py` & `smrt-1.3/smrt/microstructure_model/unified_scaled_exponential.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/unified_sticky_hard_spheres.py` & `smrt-1.3/smrt/microstructure_model/unified_sticky_hard_spheres.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/microstructure_model/unified_teubner_strey.py` & `smrt-1.3/smrt/microstructure_model/unified_teubner_strey.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/__init__.py` & `smrt-1.3/smrt/permittivity/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,7 +31,9 @@
     This complication is necessary because there is no way in Python to inspect the name of the arguments of
     a function, so the need for explicit declaration.
 
     3. to use the new function, import the module (e.g. from smrt.permittivity.ice import permittivity_something) and
     pass this function to :py:func:`smrt.core.snowpack.make_snowpack` or :py:func:`smrt.core.layer:make_snow_layer`.
 
 """
+
+
```

### Comparing `smrt-1.2.4/smrt/permittivity/brine.py` & `smrt-1.3/smrt/permittivity/brine.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/generic_mixing_formula.py` & `smrt-1.3/smrt/permittivity/generic_mixing_formula.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/ice.py` & `smrt-1.3/smrt/permittivity/ice.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from __future__ import print_function
 
 # Stdlib import
 import math
 
 # other import
-# import numpy as np
+import numpy as np
 
 # local import
 # from ..core.error import SMRTError
 from ..core.globalconstants import FREEZING_POINT, DENSITY_OF_ICE
 from ..core.layer import layer_properties
+from ..core.error import SMRTError
 
 #
 # for developers: see note in __init__.py
 #
 
 
 @layer_properties("temperature")
@@ -41,23 +42,28 @@
         to ice_permittivity_maetzler06 may be specified as an argument to the make_snow_layer 
         function. The usage example is provided for external reference or testing purposes.
 
 """
 
     freqGHz = frequency / 1e9
 
-    Ereal = 3.1884 + 9.1e-4 * (temperature - FREEZING_POINT)
+    tempC = temperature - FREEZING_POINT
+
+    if np.any(tempC > 0):
+        raise SMRTError(f"The ice temperature must be lower or equal to {FREEZING_POINT}K")
+
+    Ereal = 3.1884 + 9.1e-4 * tempC
 
     theta = 300.0 / temperature - 1.0
     alpha = (0.00504 + 0.0062 * theta) * math.exp(-22.1 * theta)
 
     B1 = 0.0207
     B2 = 1.16e-11
     b = 335.
-    deltabeta = math.exp(- 9.963 + 0.0372 * (temperature - FREEZING_POINT))
+    deltabeta = math.exp(- 9.963 + 0.0372 * tempC)
     betam = (B1 / temperature) * (math.exp(b / temperature) / ((math.exp(b / temperature) - 1)**2)) + B2 * freqGHz**2
     beta = betam + deltabeta
 
     Eimag = alpha / freqGHz + beta * freqGHz
 
     return Ereal + 1j * Eimag
 
@@ -65,16 +71,21 @@
 @layer_properties("temperature")
 def ice_permittivity_maetzler98(frequency, temperature):
     """computes permittivity of ice (accounting for ionic impurities in ice?), equations from Hufford (1991) as given in Maetzler (1998): 'Microwave properties of ice and snow', in B. Schmitt et al. (eds.): 'Solar system ices', p. 241-257, Kluwer.
 
     :param temperature: ice temperature in K
     :param frequency: Frequency in Hz"""
 
+    tempC = temperature - FREEZING_POINT
+
+    if np.any(tempC > 0):
+        raise SMRTError(f"The ice temperature must be lower or equal to {FREEZING_POINT}K")
+
     f = frequency * 1e-9
-    epi = 3.1884 + 9.1e-4 * (temperature - 273.15)
+    epi = 3.1884 + 9.1e-4 * tempC
 
     # The Hufford model for the imaginary part:
     theta = 300. / temperature - 1.
     alpha = (0.00504 + 0.0062 * theta) * math.exp(-22.1 * theta)
     beta = (0.502 - 0.131 * theta / (1 + theta)) * 1e-4 + \
         (0.542e-6 * ((1 + theta) / (theta + 0.0073))**2)
 
@@ -104,16 +115,22 @@
         a warning will be displayed.
 
 """
 
     import warnings
 
     freqGHz = frequency / 1e9
+
+    tempC = temperature - FREEZING_POINT
+
+    if np.any(tempC > 0):
+        raise SMRTError(f"The ice temperature must be lower or equal to {FREEZING_POINT}K")
+
     # Equation 10
-    Ereal = 3.1884 + 9.1e-4 * (temperature - FREEZING_POINT)
+    Ereal = 3.1884 + 9.1e-4 * tempC
 
     if (temperature - FREEZING_POINT) < -10:
         A = 3.5e-4
         B = 3.6e-5
         C = 1.2
     else:
         A = 6e-4
@@ -142,25 +159,29 @@
     **Usage example**::
 
         from smrt.permittivity.ice import ice_permittivity_tiuri84
         eps_ice = ice_permittivity_tiuri84(frequency=1.9e9, temperature=250)
 
 """
 
+    tempC = temperature - FREEZING_POINT
+
+    if np.any(tempC > 0):
+        raise SMRTError(f"The ice temperature must be lower or equal to {FREEZING_POINT}K")
+
     # Units conversion
     density_gm3 = DENSITY_OF_ICE * 1e-3
-    temp_degC = temperature - 273.15
 
     # Eq (1) - Real part
     Ereal = 1 + 1.7 * density_gm3 + 0.7 * density_gm3**2
 
     # Eq (6) - Imaginary part
     Eimag = 1.59e6 * \
         (0.52 * density_gm3 + 0.62*density_gm3**2) * \
-        (frequency**-1 + 1.23e-14 * frequency**.5) * math.exp(0.036 * temp_degC)
+        (frequency**-1 + 1.23e-14 * frequency**.5) * math.exp(0.036 * tempC)
 
     return Ereal + 1j * Eimag
 
 
 @layer_properties("temperature")
 def _ice_permittivity_HUT(frequency, temperature):
     # This gives exact agreement with the HUT model version
@@ -172,14 +193,20 @@
     #    raise SMRTError('Temperature used in calculation of ice permittivity is zero')
 
     # Issue warning if temperature is below 240K (real part is for T > 240K)
     # if (temperature < 240).any:
     #    warnings.warn('Warning: temperature is below 240K. Ice permittivity is out of range of applicability')
 
     # Real part: from Mätzler and Wegmuller (1987)
+
+    
+
+    if np.any(temperature > 273):
+        raise SMRTError(f"The ice temperature must be lower or equal to 273.0 K")
+
     real_permittivity_ice = 3.1884 + 9.1e-4 * (temperature - 273.0)
 
     # Imaginary part: from Mätzler (2006)
     # NB frequencies in original equations are in GHz, here in Hz.
     freqGHz = frequency * 1e-9
     theta = (300.0 / temperature) - 1.0  # Floats needed for correct calculation in py2.7 but not needed in 3.x
     alpha = (0.00504 + 0.0062 * theta) * math.exp(-22.1 * theta)
@@ -201,14 +228,15 @@
     #     raise SMRTError('Temperature used in calculation of ice permittivity is zero')
 
     # Issue warning if temperature is below 240K (real part is for T > 240K)
     # if np.any(temperature < 240):
     #    warnings.warn('Warning: temperature is below 240K. Ice permittivity is out of range of applicability')
 
     # Real part: from Mätzler and Wegmuller (1987)
+
     real_permittivity_ice = 3.1884 + 9.1e-4 * (temperature - 273.0)
     # Imaginary part: from Mätzler (2006)
     # NB frequencies in original equations are in GHz, here in Hz.
     freqGHz = frequency * 1e-9
     theta = (300.0 / temperature) - 1.0  # Floats needed for correct calculation in py2.7 but not needed in 3.x
     alpha = (0.00504 + 0.0062 * theta) * math.exp(-22.1 * theta)
     beta = (0.0207 / temperature) * (math.exp(335.0 / temperature) / (math.exp(335.0 / temperature) - 1.0)**2) + (
```

### Comparing `smrt-1.2.4/smrt/permittivity/saline_ice.py` & `smrt-1.3/smrt/permittivity/saline_ice.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/saline_snow.py` & `smrt-1.3/smrt/permittivity/saline_snow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+"""Mixing formulae relevant to saline snow. This module contains equations to compute the effective permittivity of saline snow. 
+
+These functions are to be used with py:meth:`~smrt.emmodel.iba.derived_IBA` or
+py:meth:`~smrt.emmodel.symsce_torquato21.derived_SymSCETK21` to change the default of most emmodels (IBA, DMRT, SFT
+Rayleigh, SCE) using the generic mixing formula Polder van Staten that automatically mixes the permittivities of the
+background (e.g.) and the scatterer materials (e.g. saline ice) to compute the effective permittivity of snow in a proportion
+determined by frac_volume.
+
+They should not be used to set the material permittivities as input of py:meth:`~smrt.smrt_inputs.make_snowpack` and
+similar functions (because the emmodel would re-mix the already mixed materials with the background material).
+"""
+
 import warnings
 
 import numpy as np
 
 from smrt.core.globalconstants import DENSITY_OF_ICE, FREEZING_POINT, GHz, PERMITTIVITY_OF_FREE_SPACE, PSU
 from .brine import brine_conductivity, brine_relaxation_time, calculate_brine_salinity, \
     permittivity_high_frequency_limit, static_brine_permittivity
@@ -76,15 +88,15 @@
     """Computes permittivity of saline snow. See `saline_snow_permittivity_scharien` documentation"""
 
     return saline_snow_permittivity_scharien(density, temperature, salinity,
                                              seawater_permittivity_stogryn95(frequency, temperature, salinity))
 
 
 def saline_snow_permittivity_scharien(density, temperature, salinity, brine_permittivity):
-    """Computes permittivity of saline snow using the Denoth / Matzler Mixture Model - Dielectric Contsant of Saline Snow.
+    """Computes permittivity of saline snow using the Denoth / Matzler Mixture Model - Dielectric Constant of Saline Snow.
 
      Assumptions:
      (1) Brine inclusion geometry as oblate spheroids
          Depolarization factor, A0 = 0.053 (Denoth, 1980)
      (2) Brine inclusions are isotropically oriented
          Coupling factor, X = 2/3 (Drinkwater and Crocker, 1988)
```

### Comparing `smrt-1.2.4/smrt/permittivity/saline_water.py` & `smrt-1.3/smrt/permittivity/saline_water.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # coding: utf-8
 
 import numpy as np
+from smrt.core.error import SMRTError
 
 from smrt.core.globalconstants import FREEZING_POINT, GHz, PERMITTIVITY_OF_FREE_SPACE, PSU
 from .brine import brine_conductivity, brine_relaxation_time, permittivity_high_frequency_limit, \
     static_brine_permittivity
 from ..core.layer import layer_properties
 
 
@@ -15,15 +16,21 @@
 
        :param frequency: frequency in Hz
        :param temperature: water temperature in K
        :param salinity: water salinity in kg/kg (see PSU constant in smrt module)
        Returns complex water permittivity for a frequency f."""
 
     tempC = temperature - FREEZING_POINT
+
     Sppt = salinity / PSU
+    
+    # Millero and Leung 1976
+    tempF = - (0.0575 * Sppt - 1.710523e-3 * Sppt**1.5 + 2.154996e-4 * Sppt**2)
+    if np.any(tempC < tempF - 0.1):  # take into account a small tolerance
+        raise SMRTError(f"The water temperature must be higher than the freezing point at the given salinity (here {tempF + FREEZING_POINT:.2f} K).")
 
     omega = 2 * np.pi * frequency
     eps_inf = 4.9  # limiting high frequency value
 
     # calculate static dielectric constant of saline water:
     eps_s_T = 87.134 - 1.949e-1 * tempC - 1.276e-2 * tempC ** 2 + 2.491e-4 * tempC ** 3
     a_ST = 1. + 1.613e-5 * Sppt * tempC - 3.656e-3 * Sppt + 3.210e-5 * Sppt ** 2 - 4.232e-7 * Sppt ** 3
```

### Comparing `smrt-1.2.4/smrt/permittivity/snow_mixing_formula.py` & `smrt-1.3/smrt/permittivity/snow_mixing_formula.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 
 # coding: utf-8
 
 """Mixing formulae relevant to snow. This module contains equations to compute the effective permittivity of snow.
+Many semi-empirical mixing formulae have been developed for specific mixture of two, three or more materials (e.g. snow).
 
-Note that by default most emmodels (IBA, DMRT, SFT Rayleigh) uses the generic mixing formula Polder van Staten that mixes the permittivities
-of the background (e.g.) and the scatterer materials (e.g. ice) to compute the effective permittivity of snow in a proportion
-determined by frac_volume. See py:meth:`~smrt.emmolde.derived_IBA`.
+These functions are to be used with py:meth:`~smrt.emmodel.iba.derived_IBA` or
+py:meth:`~smrt.emmodel.symsce_torquato21.derived_SymSCETK21` to change the default of most emmodels (IBA, DMRT, SFT
+Rayleigh, SCE) using the generic mixing formula Polder van Staten that automatically mixes the permittivities of the
+background (e.g.) and the scatterer materials (e.g. ice) to compute the effective permittivity of snow in a proportion
+determined by frac_volume.
 
-Many semi-empirical mixing formulae have been developed for specific mixture of materials (e.g. snow). They can be used to replace
-the Polder van Staten in the EM models. They should not be used to set the material permittivities
-as input of py:meth:`~smrt.smrt_inputs.make_snowpack` and similar functions (because the emmodel would re-mix
-the already mixed materials with the background material).
+They should not be used to set the material permittivities as input of py:meth:`~smrt.smrt_inputs.make_snowpack` and
+similar functions (because the emmodel would re-mix the already mixed materials with the background material).
 """
 
 import numpy as np
 from ..core.layer import layer_properties
 from ..core.globalconstants import FREEZING_POINT, DENSITY_OF_ICE, DENSITY_OF_WATER
 from ..core.error import SMRTError, smrt_warn
 from .generic_mixing_formula import polder_van_santen, polder_van_santen_three_components, polder_van_santen_three_spherical_components
```

### Comparing `smrt-1.2.4/smrt/permittivity/test_generic_mixing_formula.py` & `smrt-1.3/smrt/permittivity/test_generic_mixing_formula.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/test_ice.py` & `smrt-1.3/smrt/permittivity/test_ice.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/test_saline_ice.py` & `smrt-1.3/smrt/permittivity/test_saline_ice.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/test_snow_mixing_formula.py` & `smrt-1.3/smrt/permittivity/test_snow_mixing_formula.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/water.py` & `smrt-1.3/smrt/permittivity/water.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # coding: utf-8
 
+import numpy as np
+
 from ..core.layer import layer_properties
 from ..core.globalconstants import FREEZING_POINT, GHz
+from ..core.error import SMRTError
 
 
 @layer_properties("temperature")
 def water_permittivity_maetzler87(frequency, temperature):
     """ Calculates the complex water dielectric constant depending on the frequency and temperature
      Based on Mätzler, C., & Wegmuller, U. (1987). Dielectric properties of freshwater
      ice at microwave frequencies. *Journal of Physics D: Applied Physics*, 20(12), 1623-1630.
 
      :param frequency: frequency in Hz
      :param temperature: temperature in K
      :raises Exception: if liquid water > 0 or salinity > 0 (model unsuitable)
      :returns: Complex permittivity of pure ice
 """
+    if temperature < FREEZING_POINT:
+        raise SMRTError(f"The water temperature must be higher or equal to {FREEZING_POINT}K")
 
     freqGHz = frequency / 1e9
 
     theta = 1 - 300.0 / temperature
 
     e0 = 77.66 - 103.3 * theta
     e1 = 0.0671 * e0
@@ -48,14 +53,17 @@
     https://ntrs.nasa.gov/api/citations/19810010984/downloads/19810010984.pdf
 
 """
     freqGHz = frequency / GHz
 
     tempC = temperature - FREEZING_POINT
 
+    if np.any(tempC < 0):
+        raise SMRTError(f"The water temperature must be higher or equal to {FREEZING_POINT}K")
+
     e2 = 4.903e-2
 
     e1 = 87.74 - 0.4008 * tempC + 9.398e-4 * tempC**2 + 1.410e-6 * tempC**3
 
     # version of Liebe 1991 because Tiuri 1980 does not give the relaxation frequency
     theta = 1 - 300.0 / temperature
     f1 = 20.2 + 146.4 * theta + 316 * theta**2
```

### Comparing `smrt-1.2.4/smrt/permittivity/wetice.py` & `smrt-1.3/smrt/permittivity/wetice.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/permittivity/wetsnow.py` & `smrt-1.3/smrt/permittivity/wetsnow.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/rtsolver/__init__.py` & `smrt-1.3/smrt/rtsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/rtsolver/dort.py` & `smrt-1.3/smrt/rtsolver/dort.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,24 @@
 
 # Stdlib import
 import math
 from functools import partial
 
 # other import
 import numpy as np
+from pandas._libs import properties
 import xarray as xr
 import scipy.special.orthogonal
 import scipy.linalg
 import scipy.interpolate
 
 # local import
 from ..core.error import SMRTError, smrt_warn
 from ..core.result import make_result
-from smrt.core.lib import smrt_matrix, smrt_diag, is_equal_zero
+from smrt.core.lib import smrt_matrix, smrt_diag, is_equal_zero, is_zero_scalar
 from smrt.core.optional_numba import numba
 # Lazy import: from smrt.interface.coherent_flat import process_coherent_layers
 
 
 class DORT(object):
     """Discrete Ordinate and Eigenvalue Solver
 
@@ -204,41 +205,47 @@
         result = make_result(sensor, intensity, coords)
 
         # store other diagnostic information
         layer_index = 'layer', range(snowpack.nlayer)
         other_data = {
             'effective_permittivity': xr.DataArray(self.effective_permittivity, coords=[layer_index]),
             'ks': xr.DataArray([getattr(em, "ks", np.nan) for em in emmodels], coords=[layer_index]),
-            'ka': xr.DataArray([getattr(em, "ka", np.nan) for em in emmodels], coords=[layer_index])
+            'ka': xr.DataArray([getattr(em, "ka", np.nan) for em in emmodels], coords=[layer_index]),
+            'thickness': xr.DataArray(self.snowpack.layer_thicknesses, coords=[layer_index]),
         }
 
         return make_result(sensor, intensity, coords, other_data=other_data)
 
     def dort(self, m_max=0, special_return=False):
         # not to be called by the user
         #     """
         #     :param incident_intensity: give either the intensity (array of size 2) at incident_angle (radar) or isotropic or a function
         #             returning the intensity as a function of the cosine of the angle.
         #     :param incident_angle: if None, the spectrum is considered isotropic, otherise the angle (in radian) given the direction of
         #             the incident beam
         #     :param viewing_phi: viewing azimuth angle, the incident beam is at 0, so pi is the backscatter
         # """
 
+        npol = 3 if self.sensor.mode == 'A' else 2
+
         #
         #   compute the cosine of the angles in all layers
         # first compute the permittivity of the ground
 
         streams = compute_stream(self.n_max_stream, self.effective_permittivity, self.substrate_permittivity, mode=self.stream_mode)
 
+        # prepare the atmosphere
+
+        self.atmosphere_result = self.atmosphere.run(self.sensor.frequency, streams.outmu, npol) if self.atmosphere is not None else None
+
         #
         # compute the incident intensity array depending on the sensor
 
         intensity_0, intensity_higher, incident_streams = self.prepare_intensity_array(streams)  # TODO Ghi: make an iterator
 
-        npol = 3 if self.sensor.mode == 'A' else 2
 
         #
         # compute interface reflection and transmittance properties
 
         interfaces = InterfaceProperties(self.sensor.frequency, self.snowpack.interfaces, self.snowpack.substrate,
                                          self.effective_permittivity, streams, m_max, npol)
         #
@@ -277,17 +284,17 @@
                 intensity_up[0::npol] += intensity_up_m[0::npol] * np.cos(m * self.sensor.phi)  # TODO Ghi: deals with an array of phi
                 intensity_up[1::npol] += intensity_up_m[1::npol] * np.cos(m * self.sensor.phi)  # TODO Ghi: deals with an array of phi
                 intensity_up[2::npol] += intensity_up_m[2::npol] * np.sin(m * self.sensor.phi)  # TODO Ghi: deals with an array of phi
 
                 # TODO: implement a convergence test if we want to avoid long computation
                 # when self.m_max is too high for the phase function.
 
-        if self.sensor.mode == 'P' and self.atmosphere is not None:
-            intensity_up = self.atmosphere.tbup(self.sensor.frequency, streams.outmu, npol) + \
-                self.atmosphere.trans(self.sensor.frequency, streams.outmu, npol) * intensity_up
+        if self.sensor.mode == 'P' and self.atmosphere_result is not None:
+            intensity_up = self.atmosphere_result.tb_up + \
+                self.atmosphere_result.transmittance * intensity_up
 
         if self.sensor.mode == 'A':
             # compress to get only the backscatter
             backscatter_intensity_up = np.empty((npol * len(incident_streams), npol))
             for j, i in enumerate(incident_streams):
                 # the j-th column vector contains the stram i, with angle mu[i]
                 backscatter_intensity_up[3 * j: 3 * j + 3, :] = intensity_up[3 * i: 3 * i + 3, 3 * j: 3 * j + 3]
@@ -340,27 +347,26 @@
                     j_higher += 1
 
         elif self.sensor.mode == 'P':
 
             npol = 2
             incident_streams = []
 
-            if self.atmosphere is not None:
+            if self.atmosphere_result is not None:
 
                 # incident radiation is a function of frequency and incidence angle
                 # assume azimuthally symmetric
-                intensity_0 = self.atmosphere.tbdown(self.sensor.frequency, streams.outmu, npol)[:, np.newaxis]
+                intensity_0 = self.atmosphere_result.tb_down[:, np.newaxis]
                 intensity_higher = np.zeros_like(intensity_0)
 
             else:
                 intensity_0 = np.zeros((len(streams.outmu) * npol, 1))
                 intensity_higher = intensity_0
                 intensity_0.flags.writeable = False  # make immutable
                 intensity_higher.flags.writeable = False  # make immutable
-
         else:
             raise SMRTError("Unknow sensor mode")
 
         return intensity_0, intensity_higher, incident_streams
 
     def dort_modem_banded(self, m, streams, eigenvalue_solver,
                           interfaces, intensity_down_m,
@@ -560,15 +566,15 @@
 
 
 def muleye(x):
     #  """multiply x * 1v """
 
     if isinstance(x, smrt_diag):
         return x.diagonal()
-    elif (x.is_zero_scalar()) or (len(x.shape) == 0):
+    elif (is_zero_scalar(x)) or (len(x.shape) == 0):
         return np.atleast_1d(x)
     else:
         assert len(x.shape) == 2
         return np.sum(x, axis=1)
 
 
 def matmul(a, b, *args):
@@ -635,14 +641,16 @@
         # :param Ke: extinction coefficient of the layer for mode m
         # :param ft_even_phase: ft_even_phase function of the layer for mode m
         # :param mu: cosines
         # :param weight: weights
 
         self.ke = ke
         self.ks = ks
+        self.ft_even_phase_function = ft_even_phase_function
+        self.m_max = m_max
         self.mu = mu
         self.weight = weight
         self.normalization = normalization
 
         if method == "eig":
             self.diagonalize_function = self.diagonalize_eig
         elif method == "shur":
@@ -651,19 +659,24 @@
             self.diagonalize_function = partial(self.diagonalize_shur, force_triu=True)
         else:
             raise SMRTError(f"Unknown method '{method}' to diagonalize the matrix")
 
         self.norm_0 = None
         self.norm_m = None
 
-        if ft_even_phase_function is not None:
-            mu = np.concatenate((self.mu, -self.mu))
-            self.ft_even_phase = ft_even_phase_function(mu, mu, m_max)
-        else:
-            self.ft_even_phase = smrt_matrix(0)
+    @property
+    def ft_even_phase(self):
+        # cached version of the ft_even_phase
+        if not hasattr(self, "_ft_even_phase"):
+            if self.ft_even_phase_function is None:
+                self._ft_even_phase = smrt_matrix(0)
+            else:
+                mu = np.concatenate((self.mu, -self.mu))
+                self._ft_even_phase = self.ft_even_phase_function(mu, mu, self.m_max)
+        return self._ft_even_phase
 
     def solve(self, m, compute_coherent_only, debug_A=False):
         # solve the homogeneous equation for a single layer and return eignen values and eigen vectors
         # :param m: mode
         # :param compute_coherent_only
         # :returns: beta, E, Q
         #
@@ -1069,14 +1082,26 @@
     #     :param permittivity: permittivity of each layer
     #     :type permittivity: ndarray
     #     :returns: mu, weight, outmu
     # """
 
     streams = Streams()
 
+    nlayer = len(permittivity)
+
+    if nlayer == 0:
+        streams.outmu, streams.outwweight = gaussquad(n_max_stream)
+        streams.n_air = n_max_stream
+        streams.weight = []
+        streams.mu = []
+        streams.n = []
+        return streams
+
+    # there are some layers
+
     #  ### search and proceed with the most refringent layer
     k_most_refringent = np.argmax(permittivity)
     real_index_air = np.real(np.sqrt(permittivity[k_most_refringent] / 1.0))
 
     if mode is None or mode == "most_refringent":
         # calculate the gaussian weights and nodes for the most refringent layer
         mu_most_refringent, weight_most_refringent = gaussquad(n_max_stream)
@@ -1092,15 +1117,14 @@
 
         streams.n = scipy.optimize.brentq(n_max_stream, 2 * n_max_stream)
         mu_most_refringent, weight_most_refringent = gaussquad(streams.n)
 
     else:
         raise RuntimeError("Unknow mode to compute the number of stream")
 
-    nlayer = len(permittivity)
 
     #  calculate the nodes and weights of all the other layers
 
     # calculate real part of the index. It is an approximation.
     # See for instance "Semiconductor Physics, Quantum Electronics & Optoelectronics. 2001. V. 4, N 3. P. 214-218."
     real_index = np.real(np.sqrt(permittivity[k_most_refringent] / permittivity[:]))
```

### Comparing `smrt-1.2.4/smrt/rtsolver/dort_nonormalization.py` & `smrt-1.3/smrt/rtsolver/dort_nonormalization.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/rtsolver/nadir_lrm_altimetry.py` & `smrt-1.3/smrt/rtsolver/nadir_lrm_altimetry.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/rtsolver/test_dort.py` & `smrt-1.3/smrt/rtsolver/test_dort.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     m = Model(IBA, DORT, rtsolver_options=dict(
         m_max=m_max,
         n_max_stream=nstreams,
         diagonalization_method="shur"))
 
 
-def test_shur_based_diagonalisation():
+def test_shur_forcedtriu_based_diagonalisation():
 
     sp = make_snowpack(thickness=[1000],
                        microstructure_model='exponential',
                        density=280,
                        temperature=265,
                        corr_length=0.05e-3)
```

### Comparing `smrt-1.2.4/smrt/rtsolver/test_nadir_lrm_altimetry.py` & `smrt-1.3/smrt/rtsolver/test_nadir_lrm_altimetry.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/rtsolver/waveform_model.py` & `smrt-1.3/smrt/rtsolver/waveform_model.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/runner/celery_runner.py` & `smrt-1.3/smrt/runner/celery_runner.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/runner/dask_runner.py` & `smrt-1.3/smrt/runner/dask_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 from dask.distributed import Client
 
 
 class DaskParallelRunner(object):
     """Run the simulations using dask.distributed on a cluster.
     """
 
-    def __init__(self, client="localhost:7454", chunk=10):
+    def __init__(self, progressbar=False, client="localhost:7454", chunk=10):
         """prepare a dask runner.
 
+        :param progressbar: show a progress bar if True (not available for DaskparalleRunner)
         :param client: the url or a dask client objbect
         :param chunk: size of the chunk to transmit to the runner
 
         """
 
         super().__init__()
```

### Comparing `smrt-1.2.4/smrt/substrate/__init__.py` & `smrt-1.3/smrt/substrate/__init__.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/iem_fung92_brogioni10.py` & `smrt-1.3/smrt/substrate/iem_fung92_brogioni10.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/reflector.py` & `smrt-1.3/smrt/substrate/reflector.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/reflector_backscatter.py` & `smrt-1.3/smrt/substrate/reflector_backscatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # coding: utf-8
 
-""" Implement a reflective boundary conditions with prescribed reflection coefficient in the specular direction.
-The reflection is set to a value or a function of theta. Azimuthal symmetry is assumed (no dependence on phi).
+""" Implement a reflective boundary conditions with prescribed reflection coefficient in the specular direction, and backscatter coefficient.
+The reflection is set to a value or a function of theta. Azimuthal symmetry is assumed (no dependence on phi). 
 
 The `specular_reflection` parameter can be a scalar, a function or a dictionary.
 
     - scalar: same reflection is use for all angles
     - function: the function must take a unique argument theta array (in radians) and return the reflection as an array of the same size as theta
     - dictionary: in this case, the keys must be 'H' and 'V' and the values are a scalar or a function and are interpreted as for the non-polarized case.
 
+The `backscattering_coefficient` is a dictionary with VV nad HH keys. It is not possible to set HV and VH.
+Note also that modeling substrate with prescribed backscatter value with the DORT solver is an approximate trick, and
+the result is only approximatly the prescribed value even for a transparent snowpack.
+
 To make a reflector, it is recommended to use the helper function :py:func:`~smrt.substrate.reflector.make_reflector`.
 
 
 Examples::
 
     # the full path import is required
     from smrt.substrate.reflector import make_reflector
@@ -40,28 +44,28 @@
 def make_reflector(temperature=None, specular_reflection=None, backscattering_coefficient=None):
 
     """ Construct a reflector or absorber instance.
 
     """
 
     # create the instance
-    return Reflector(temperature=temperature, specular_reflection=specular_reflection,
+    return ReflectorBackscatter(temperature=temperature, specular_reflection=specular_reflection,
                      backscattering_coefficient=backscattering_coefficient)
 
 
-class Reflector(Substrate):
+class ReflectorBackscatter(Substrate):
 
     args = []
     optional_args = {'specular_reflection': None, 'backscattering_coefficient': None}
 
     def specular_reflection_matrix(self, frequency, eps_1, mu1, npol):
 
-        if npol > 2 and not hasattr(Reflector, "stop_pol2_warning"):
+        if npol > 2 and not hasattr(ReflectorBackscatter, "stop_pol2_warning"):
             print("active model is not yet fully implemented, need modification for the third component")  # !!!
-            Reflector.stop_pol2_warning = True
+            ReflectorBackscatter.stop_pol2_warning = True
 
         if self.specular_reflection is None and self.backscattering_coefficient is None:
             self.specular_reflection = 1
 
         spec_refl_coeff = smrt_matrix.zeros((npol, len(mu1)))
         if isinstance(self.specular_reflection, dict):  # we have a dictionary with polarization
             spec_refl_coeff[0] = self._get_refl(self.specular_reflection['V'], mu1)
@@ -91,15 +95,15 @@
 
                 diffuse_refl_coeff[0, m, :] += coef * self._get_refl(self.backscattering_coefficient['VV'], mu_i)
                 diffuse_refl_coeff[1, m, :] += coef * self._get_refl(self.backscattering_coefficient['HH'], mu_i)
 
         elif self.backscattering_coefficient is not None:
             raise SMRTError("backscattering_coefficient must be a dictionary with keys VV and HH")
         else:
-            return smrt_matrix(0)
+            diffuse_refl_coeff = smrt_matrix(0)
 
         return diffuse_refl_coeff
 
     def emissivity_matrix(self, frequency, eps_1, mu1, npol):
 
         if self.specular_reflection is None and self.backscattering_coefficient is None:
             self.specular_reflection = 1
```

### Comparing `smrt-1.2.4/smrt/substrate/rough_choudhury79.py` & `smrt-1.3/smrt/substrate/rough_choudhury79.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/soil_qnh.py` & `smrt-1.3/smrt/substrate/soil_qnh.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/soil_wegmuller.py` & `smrt-1.3/smrt/substrate/soil_wegmuller.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/test_reflector.py` & `smrt-1.3/smrt/substrate/test_reflector.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/test_rough_choudhury79.py` & `smrt-1.3/smrt/substrate/test_rough_choudhury79.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import numpy as np
 import pytest
 
+from smrt.core.globalconstants import FREEZING_POINT
 from smrt.inputs.make_soil import make_soil
 from smrt.permittivity.water import water_permittivity
 
 
 def test_make_rough_choudhury():
 
     make_soil('rough_choudhury79', 'dobson85', 275, moisture=0.9, sand=0.2, clay=0.3, drymatter=1100, roughness_rms=1e-2)
@@ -29,16 +30,16 @@
         frequency = 1e9
         mu1 = np.cos(np.radians(np.arange(10, 80)))
         npol = 2
         s.specular_reflection_matrix(frequency, 1, mu1, npol)
 
 
 def test_make_rough_water():
-    make_soil('rough_choudhury79', water_permittivity(6e9, 273), temperature=270, roughness_rms=0.5e-3)
+    make_soil('rough_choudhury79', water_permittivity(6e9, FREEZING_POINT), temperature=270, roughness_rms=0.5e-3)
 
 
 def test_equivalence_fresnel():
 
-    h2o = water_permittivity(6e9, 273)
-    rough = make_soil('rough_choudhury79', h2o, temperature=273, roughness_rms=0.)
-    smooth = make_soil('flat', h2o, temperature=273)
+    h2o = water_permittivity(6e9, FREEZING_POINT)
+    rough = make_soil('rough_choudhury79', h2o, temperature=FREEZING_POINT, roughness_rms=0.)
+    smooth = make_soil('flat', h2o, temperature=FREEZING_POINT)
     np.testing.assert_equal(rough.specular_reflection_matrix(10e9, 1, np.cos(50), 2)[0], smooth.specular_reflection_matrix(10e9, 1, np.cos(50), 2)[0])
```

### Comparing `smrt-1.2.4/smrt/substrate/test_soil_qnh.py` & `smrt-1.3/smrt/substrate/test_soil_qnh.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/substrate/test_soil_wegmuller.py` & `smrt-1.3/smrt/substrate/test_soil_wegmuller.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_coherent_layer.py` & `smrt-1.3/smrt/test/test_coherent_layer.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_dmrtdort.py` & `smrt-1.3/smrt/test/test_dmrtdort.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # coding: utf-8
 
+from re import sub
 import numpy as np
 
 # local import
 from smrt import make_snowpack, make_model, make_snow_layer, make_soil
-from smrt.inputs.sensor_list import amsre, active
+from smrt.inputs.make_medium import make_transparent_volume
+from smrt.inputs.sensor_list import amsre, active, passive
+from smrt.substrate.reflector import make_reflector
 
 #
 # Ghi: rapid hack, should be splitted in different functions
 #
 
 
 def setup_snowpack():
@@ -75,35 +78,54 @@
 
 
 def test_less_refringent_bottom_layer():
     # Regression test 19-03-2018: value may change if other bugs found
     snowpack = make_snowpack([0.2, 0.3], "sticky_hard_spheres", density=[290.0, 250.0], radius=50e-6, stickiness=0.2,
                              substrate=make_soil("transparent", 1, 270))
     # this test fails with some version of scipy if not using the shur method
-    m = make_model("dmrt_qcacp_shortrange", "dort", rtsolver_options=dict(diagonalization_method='shur'))
+    m = make_model("dmrt_qcacp_shortrange", "dort", rtsolver_options=dict(diagonalization_method='shur_forcedtriu'))
     scat = active(10e9, 45)
     res = m.run(scat, snowpack)
     print(res.sigmaVV_dB(), res.sigmaHH_dB())
     assert abs(res.sigmaVV_dB() - -50.25547167709486) < 1e-1
     assert abs(res.sigmaHH_dB() - -50.52755576862734) < 1e-1
 
 
 
 #The following test fails
 def test_less_refringent_bottom_layer_VV():
     # Regression test 19-03-2018: value may change if other bugs found
     snowpack = make_snowpack([0.2, 0.3], "sticky_hard_spheres", density = [290.0, 250.0], radius = 1e-4, stickiness=0.2)
-    m = make_model("dmrt_qcacp_shortrange", "dort", rtsolver_options=dict(diagonalization_method='shur'))
+    m = make_model("dmrt_qcacp_shortrange", "dort", rtsolver_options=dict(diagonalization_method='shur_forcedtriu'))
     scat = active(10e9, 45)
     res = m.run(scat, snowpack)
     print(res.sigmaVV())
     assert abs(res.sigmaVV() - 7.54253344e-05) < 1e-7
 
 
 def test_less_refringent_bottom_layer_HH():
     # Regression test 19-03-2018: value may change if other bugs found
     snowpack = make_snowpack([0.2, 0.3], "sticky_hard_spheres", density = [290.0, 250.0], radius = 1e-4, stickiness=0.2)
-    m = make_model("dmrt_qcacp_shortrange", "dort", rtsolver_options=dict(diagonalization_method='shur'))
+    m = make_model("dmrt_qcacp_shortrange", "dort", rtsolver_options=dict(diagonalization_method='shur_forcedtriu'))
     scat = active(10e9, 45)
     res = m.run(scat, snowpack)
     print(res.sigmaHH())
-    assert abs(res.sigmaHH() - 7.09606407e-05) < 1e-7
+    assert abs(res.sigmaHH() - 7.09606407e-05) < 1e-7
+
+
+def test_transparent_volume():
+
+    r = 0.5
+    temperature = 200
+    substrate=make_reflector(temperature=temperature, specular_reflection=r)
+    snowpack = make_transparent_volume(substrate=substrate)
+
+    m = make_model("iba", "dort")
+    radiometer = passive(37e9, 45)
+    res = m.run(radiometer, snowpack)
+    print(res.TbV(), res.TbH())
+
+    # the emissivity is e = 1-r 
+    assert abs(res.TbV() - (1 - r) * temperature) < 1e-7
+    assert abs(res.TbH() - (1 - r) * temperature) < 1e-7
+
+
```

### Comparing `smrt-1.2.4/smrt/test/test_iba_sea_ice.py` & `smrt-1.3/smrt/test/test_iba_sea_ice.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_integration_geometrical_optics.py` & `smrt-1.3/smrt/test/test_integration_geometrical_optics.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_integration_iba.py` & `smrt-1.3/smrt/test/test_integration_iba.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_integration_iba_original.py` & `smrt-1.3/smrt/test/test_integration_iba_original.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_mixed_emmodel.py` & `smrt-1.3/smrt/test/test_mixed_emmodel.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_model.py` & `smrt-1.3/smrt/test/test_model.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_physics_law.py` & `smrt-1.3/smrt/test/test_physics_law.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def _do_test_isothermal_universe(pc, thickness_1):
 
     T = 265
 
     substrate = make_soil('soil_wegmuller', permittivity_model=complex(10, 1), roughness_rms=0.001, temperature=T)
 
-    atmosphere = SimpleIsotropicAtmosphere(tbdown=T, tbup=0, trans=1)
+    atmosphere = SimpleIsotropicAtmosphere(tb_down=T, tb_up=0, transmittance=1)
 
     snowpack = make_snowpack([0.3, thickness_1], "exponential",
                              density=[200, 300], temperature=T, corr_length=pc,
                              ice_permittivity_model=complex(1.7, 0.00001),
                              substrate=substrate, atmosphere=atmosphere)
 
     # create the sensor
@@ -60,15 +60,15 @@
 
 def _do_test_kirchoff_law(pc, thickness_1):
 
     T = 265.
 
     substrate = make_soil('soil_wegmuller', permittivity_model=complex(10, 1), roughness_rms=0.001, temperature=T)
 
-    atmosphere1K = SimpleIsotropicAtmosphere(tbdown=1, tbup=0, trans=1)
+    atmosphere1K = SimpleIsotropicAtmosphere(tb_down=1, tb_up=0, transmittance=1)
 
     snowpack = make_snowpack([0.3, thickness_1], "exponential",
                              density=[200, 300], temperature=T, corr_length=pc,
                              ice_permittivity_model=complex(1.7, 0.00001),
                              substrate=substrate)
 
     # create the sensor
```

### Comparing `smrt-1.2.4/smrt/test/test_reflector_backscattering.py` & `smrt-1.3/smrt/test/test_reflector_backscattering.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/test/test_soil.py` & `smrt-1.3/smrt/test/test_soil.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/utils/dmrt_qms_legacy.py` & `smrt-1.3/smrt/utils/dmrt_qms_legacy.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/utils/hut_legacy.py` & `smrt-1.3/smrt/utils/hut_legacy.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/utils/memls_legacy.py` & `smrt-1.3/smrt/utils/memls_legacy.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/utils/memlsscatt.m` & `smrt-1.3/smrt/utils/memlsscatt.m`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/utils/mpl_plots.py` & `smrt-1.3/smrt/utils/mpl_plots.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt/utils/repo_tools.py` & `smrt-1.3/smrt/utils/repo_tools.py`

 * *Files identical despite different names*

### Comparing `smrt-1.2.4/smrt.egg-info/PKG-INFO` & `smrt-1.3/smrt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smrt
-Version: 1.2.4
+Version: 1.3
 Summary: The Snow Microwave Radiative Transfer (SMRT) model is a highly modular model to compute the thermal emission and backscattering coefficient of snowpacks and other cryospheric bodies in the microwave domain.
 Author-email: Ghislain Picard <ghislain.picard@univ-grenoble-alpes.fr>, Melody Sandells <melody.sandells@gmail.com>, Henning Löwe <loewe@slf.ch>
 License: DISCLAIMER: This version of SMRT is an early release. As such, some components may not be fully implemented or may give rise to unexpected behaviour. Please use this software with caution, ask for assistance if needed, and let us know any feedback you may have.
         
         SMRT is Copyright (c) 2016 Ghislain Picard, Melody Sandells, Henning Löwe. Licensed under GNU LGPL:
         
         
@@ -186,14 +186,24 @@
 License-File: LICENSE
 Requires-Dist: numpy<2,>=1.13
 Requires-Dist: pandas>=0.20.3
 Requires-Dist: scipy>=1.0.0
 Requires-Dist: xarray>=0.10.3
 Requires-Dist: numba>=0.40
 Requires-Dist: joblib>=1.0.0
+Provides-Extra: progressbar
+Requires-Dist: tqdm; extra == "progressbar"
+Provides-Extra: pyrtlib
+Requires-Dist: scikit-learn; extra == "pyrtlib"
+Requires-Dist: bs4; extra == "pyrtlib"
+Requires-Dist: netCDF4; extra == "pyrtlib"
+Requires-Dist: requests; extra == "pyrtlib"
+Requires-Dist: cdsapi; extra == "pyrtlib"
+Requires-Dist: cfgrib; extra == "pyrtlib"
+Requires-Dist: pyrtlib; extra == "pyrtlib"
 
 
 Snow Microwave Radiative Transfer model
 =============================================
 
 [SMRT](https://www.smrt-model.science/) is a radiative transfer model to compute emission and backscatter from snowpack.
```

### Comparing `smrt-1.2.4/smrt.egg-info/SOURCES.txt` & `smrt-1.3/smrt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 smrt/__init__.py
 smrt.egg-info/PKG-INFO
 smrt.egg-info/SOURCES.txt
 smrt.egg-info/dependency_links.txt
 smrt.egg-info/requires.txt
 smrt.egg-info/top_level.txt
 smrt/atmosphere/__init__.py
+smrt/atmosphere/pyrtlib_atmosphere.py
+smrt/atmosphere/pyrtlib_climatology_atmosphere.py
+smrt/atmosphere/pyrtlib_era5_atmosphere.py
 smrt/atmosphere/simple_isotropic_atmosphere.py
 smrt/atmosphere/test_atmosphere.py
 smrt/core/__init__.py
 smrt/core/atmosphere.py
 smrt/core/error.py
 smrt/core/filelock.py
 smrt/core/fresnel.py
```

