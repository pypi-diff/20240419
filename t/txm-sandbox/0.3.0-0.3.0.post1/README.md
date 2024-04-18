# Comparing `tmp/txm_sandbox-0.3.0.tar.gz` & `tmp/txm_sandbox-0.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.0.tar", last modified: Thu Apr 18 11:33:27 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.0.post1.tar", last modified: Thu Apr 18 22:42:48 2024, max compression
```

## Comparing `txm_sandbox-0.3.0.tar` & `txm_sandbox-0.3.0.post1.tar`

### file list

```diff
@@ -1,94 +1,87 @@
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.283419 txm_sandbox-0.3.0/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1070 2024-04-18 03:35:27.000000 txm_sandbox-0.3.0/LICENSE
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      147 2024-04-18 03:34:56.000000 txm_sandbox-0.3.0/MANIFEST.in
--rw-r--r--   0 xiao      (1000) xiao      (1000)      706 2024-04-18 11:33:27.279419 txm_sandbox-0.3.0/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1639 2024-04-18 03:35:09.000000 txm_sandbox-0.3.0/README.md
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     2565 2024-04-18 11:27:34.000000 txm_sandbox-0.3.0/TXM_GUI2.ipynb
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.263419 txm_sandbox-0.3.0/TXM_Sandbox/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.267419 txm_sandbox-0.3.0/TXM_Sandbox/config/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     5092 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/config/XANES2D_GUI_config.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/config/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       45 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/config/analysis_tool_gui_cfg.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      497 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/config/io_tomo_h5_data_structure.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/config/io_xanes2D_h5_data_structure.json
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      616 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/config/io_xanes3D_h5_data_structure.json
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.267419 txm_sandbox-0.3.0/TXM_Sandbox/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/dicts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3848 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/dicts/config_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61110 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      755 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      583 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/dicts/xanes_analysis_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.267419 txm_sandbox-0.3.0/TXM_Sandbox/external/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/external/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      253 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/external/user_io.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.271419 txm_sandbox-0.3.0/TXM_Sandbox/gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    32500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    74137 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    79463 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/gui_components.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    36752 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15709 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/main_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      795 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/misc_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   169879 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   204783 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   202060 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    91679 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   203257 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes_fitting_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.271419 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.275419 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/configs/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/configs/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.275419 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     5528 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/dicts/data_struct_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.275419 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15317 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     9617 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    25660 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    23133 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    47833 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15647 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/xanes_vis_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     1665 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/napari_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.275419 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      605 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      599 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15529 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2428 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16707 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1201 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2029 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    73678 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/txm_napari_gui copy.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    73693 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/txm_napari_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.275419 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1297 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    10609 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/utils/misc.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.279419 txm_sandbox-0.3.0/TXM_Sandbox/tmp/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/tmp/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       69 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/tmp/readme.txt
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.279419 txm_sandbox-0.3.0/TXM_Sandbox/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16672 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/io.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    14410 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     4246 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/misc.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1439 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/plotlib.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61837 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/reg_algs.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    70498 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    36738 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2342 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    23436 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_math.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     6083 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    84774 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3266 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_spectra_filters.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 11:33:27.279419 txm_sandbox-0.3.0/TXM_Sandbox.egg-info/
--rw-r--r--   0 xiao      (1000) xiao      (1000)      706 2024-04-18 11:33:27.000000 txm_sandbox-0.3.0/TXM_Sandbox.egg-info/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2824 2024-04-18 11:33:27.000000 txm_sandbox-0.3.0/TXM_Sandbox.egg-info/SOURCES.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 11:33:27.000000 txm_sandbox-0.3.0/TXM_Sandbox.egg-info/dependency_links.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 11:33:27.000000 txm_sandbox-0.3.0/TXM_Sandbox.egg-info/not-zip-safe
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      170 2024-04-18 11:33:27.000000 txm_sandbox-0.3.0/TXM_Sandbox.egg-info/requires.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       12 2024-04-18 11:33:27.000000 txm_sandbox-0.3.0/TXM_Sandbox.egg-info/top_level.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       38 2024-04-18 11:33:27.283419 txm_sandbox-0.3.0/setup.cfg
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1140 2024-04-18 11:32:18.000000 txm_sandbox-0.3.0/setup.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1070 2024-04-18 03:35:27.000000 txm_sandbox-0.3.0.post1/LICENSE
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      147 2024-04-18 03:34:56.000000 txm_sandbox-0.3.0.post1/MANIFEST.in
+-rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/PKG-INFO
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1639 2024-04-18 03:35:09.000000 txm_sandbox-0.3.0.post1/README.md
+-rwxrwxr-x   0 xiao      (1000) xiao      (1000)     2565 2024-04-18 11:27:34.000000 txm_sandbox-0.3.0.post1/TXM_GUI2.ipynb
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       38 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/setup.cfg
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1155 2024-04-18 22:38:23.000000 txm_sandbox-0.3.0.post1/setup.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.943797 txm_sandbox-0.3.0.post1/txm_sandbox/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.943797 txm_sandbox-0.3.0.post1/txm_sandbox/config/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/config/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.947797 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3848 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    61110 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      755 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      583 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/xanes_analysis_dict.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.947797 txm_sandbox-0.3.0.post1/txm_sandbox/external/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/external/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      253 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/external/user_io.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/gui/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    32500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    74137 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    79463 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/gui_components.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    36752 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15709 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/main_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      795 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   169879 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   204783 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   202060 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    91679 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   203257 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_fitting_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/configs/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/configs/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)     5528 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/data_struct_dict.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      106 2024-04-18 19:44:50.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15327 2024-04-18 19:47:10.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     9587 2024-04-18 19:52:32.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    25806 2024-04-18 19:53:16.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)     1503 2024-04-18 22:36:58.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/txm_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    23082 2024-04-18 19:53:44.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    48430 2024-04-18 19:54:08.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15803 2024-04-18 19:54:19.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)     1533 2024-04-18 20:23:11.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/napari_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.955798 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      605 2024-04-18 20:05:13.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      599 2024-04-18 20:05:03.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15251 2024-04-18 19:59:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2428 2024-04-18 20:01:32.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    16707 2024-04-18 20:01:56.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1197 2024-04-18 20:04:22.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2029 2024-04-18 20:04:35.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.955798 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1264 2024-04-18 20:05:59.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    10590 2024-04-18 20:06:46.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/misc.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.955798 txm_sandbox-0.3.0.post1/txm_sandbox/tmp/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/tmp/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/txm_sandbox/utils/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    16672 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/io.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    14410 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xiao      (1000) xiao      (1000)     4246 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/misc.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1439 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/plotlib.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    61837 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    70498 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    36738 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2342 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    23436 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     6083 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    84774 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3266 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_spectra_filters.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/
+-rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/PKG-INFO
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2504 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/not-zip-safe
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      170 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/requires.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       12 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.0/LICENSE` & `txm_sandbox-0.3.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/PKG-INFO` & `txm_sandbox-0.3.0.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TXM_Sandbox
-Version: 0.3.0
+Name: txm_sandbox
+Version: 0.3.0.post1
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.0/README.md` & `txm_sandbox-0.3.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_GUI2.ipynb` & `txm_sandbox-0.3.0.post1/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/gui_components.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/main_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 import dask.array as da
 import h5py
 import json
 from pathlib import Path
 import matplotlib.pyplot as plt
 from magicgui import widgets
 
-from TXM_Sandbox.utils.io import (
+from ..utils.io import (
     tif_writer,
     tif_seq_writer,
     raw_writer,
     raw_seq_writer,
-    asc_writer,
 )
-from TXM_Sandbox.napari_gui.utils.misc import (
+from ..utils.misc import (
     check_avail_items,
     get_slcd_ds_path,
     update_layer_in_viewer,
     show_layers_in_viewer,
     rm_gui_viewers,
 )
 
@@ -240,15 +239,18 @@
             self._appl_mk_mask = None
 
     def __set_layers_order(self):
         if ("appl_mk_data" in self.viewer.layers) and (
             "appl_mk_mask" in self.viewer.layers
         ):
             self.viewer.layers.move_multiple(
-                [self.viewer.layers.index(self.viewer.layers["appl_mk_data"]), self.viewer.layers.index(self.viewer.layers["appl_mk_mask"]), ],
+                [
+                    self.viewer.layers.index(self.viewer.layers["appl_mk_data"]),
+                    self.viewer.layers.index(self.viewer.layers["appl_mk_mask"]),
+                ],
                 0,
             )
             self.viewer.layers["appl_mk_mask"].opacity = 0.2
             self.viewer.layers["appl_mk_mask"].colormap = "yellow"
             self.viewer.layers["appl_mk_data"].visible = True
             self.viewer.layers["appl_mk_mask"].visible = True
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import dask.array as da
 import h5py
 import json
 from pathlib import Path
 import matplotlib.pyplot as plt
 from magicgui import widgets
 
-from TXM_Sandbox.utils.io import (
+from ...utils.io import (
     tif_writer,
     tif_seq_writer,
     raw_writer,
     raw_seq_writer,
     asc_writer,
 )
-from TXM_Sandbox.napari_gui.utils.misc import (
+from ..utils.misc import (
     check_avail_items,
     get_slcd_ds_path,
     update_layer_in_viewer,
     show_layers_in_viewer,
     rm_gui_viewers,
     disp_progress_info,
 )
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/tomo_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import glob
 import h5py
 import datetime
 from pathlib import Path
 import matplotlib.pyplot as plt
 from magicgui import widgets
 
-from TXM_Sandbox.utils.io import data_reader, tomo_h5_reader
-from TXM_Sandbox.utils.tomo_recon_tools import rm_redundant
-from TXM_Sandbox.gui.gui_components import (
+from ...utils.io import data_reader, tomo_h5_reader
+from ...utils.tomo_recon_tools import rm_redundant
+from ...gui.gui_components import (
     check_file_availability,
 )
-from TXM_Sandbox.napari_gui.utils.misc import (
+from ..utils.misc import (
     rm_gui_viewers,
     disp_progress_info,
     info_reader,
     update_layer_in_viewer,
     show_layers_in_viewer,
 )
-from TXM_Sandbox.napari_gui.dicts.data_struct_dict import ZFLY_CFG, FLY_CFG
+from ..dicts.data_struct_dict import ZFLY_CFG, FLY_CFG
 
 
 h5_reader = data_reader(tomo_h5_reader)
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 tomo_rec_script_fn = Path(__file__).parents[1] / "scripts/tomo_recon_cmd.py"
 tomo_batch_rec_script_fn = Path(__file__).parents[1] / "scripts/tomo_batch_recon_cmd.py"
@@ -74,15 +74,17 @@
             name="Step 1",
             value="--------------------     Trial Cen    --------------------",
         )
         self.top_dir = widgets.FileEdit(mode="d", value=Path.home())
         self.file_type = widgets.ComboBox(
             choices=["tomo_zfly", "fly_scan"], value="tomo_zfly", name="scan type"
         )
-        self.find_multi_cen = widgets.CheckBox(value=False, text="find cen for multiple scans", enabled=False)
+        self.find_multi_cen = widgets.CheckBox(
+            value=False, text="find cen for multiple scans", enabled=False
+        )
         self.scan_id = widgets.ComboBox(
             enabled=False, choices=get_self_avail_scn_id_choices, name="scan id"
         )
         self.proj_prev = widgets.CheckBox(value=False, text="proj prev", enabled=False)
         self.cen_sch_s = widgets.SpinBox(
             min=1, max=2500, value=600, step=1, enabled=False, name="cen srch s"
         )
@@ -104,17 +106,15 @@
         )
         self.label2 = widgets.Label(
             name="Step 2",
             value="--------------------     Vol Recon    --------------------",
         )
         self.cen = widgets.LineEdit(name="picked cen", enabled=False)
         self.pick_cen = widgets.PushButton(text="pick center", enabled=False)
-        self.trial_cen_done = widgets.PushButton(
-            text="trial cen done", enabled=False
-        )
+        self.trial_cen_done = widgets.PushButton(text="trial cen done", enabled=False)
         self.trial_cen_done = widgets.RadioButtons(
             name="trial cen done",
             choices=["Yes", "No"],
             orientation="horizontal",
             value="No",
             tooltip="confirm if all trial centering works are finished",
             enabled=False,
@@ -204,15 +204,15 @@
             self.close_file.enabled = False
         else:
             self.find_multi_cen.enabled = True
             self.scan_id.enabled = True
             self.proj_prev.enabled = True
             self.cen_sch_s.enabled = True
             self.ref_sli.enabled = True
-            self.is_wedge.enabled = True 
+            self.is_wedge.enabled = True
             if self.is_wedge.value:
                 self.wedge_thsh.enabled = True
             else:
                 self.wedge_thsh.enabled = False
             self.phase_retrieval.enabled = True
             if self.phase_retrieval.value:
                 self.beta_gamma_ratio.enabled = True
@@ -243,15 +243,14 @@
             else:
                 self.pick_cen.enabled = False
             if self._cen is None:
                 self.vol_rec.enabled = False
             else:
                 self.vol_rec.enabled = True
         self.close_file.enabled = True
-        
 
     def __preset_dflt(self):
         self._data_dim = info_reader(self.scn_fn, dtype="data", cfg=self._tomo_cfg)
         if (self._data_dim[2] / 2 - self.cen_sch_s.value) > (self._data_dim[2] / 6):
             self.cen_sch_s.value = int(self._data_dim[2] / 2 - 40)
         # if self._data_dim[1] < self.cen_sch_s.value:
         self.ref_sli.value = int(self._data_dim[1] / 2)
@@ -302,23 +301,39 @@
     def _proj_prev(self):
         rm_gui_viewers(self.viewer, ["proj_prev"])
         if self.proj_prev.value:
             if self.file_type.value == "tomo_zfly":
                 # self.viewer.add_image(
                 #     h5py.File(self.scn_fn, "r")["/Exchange/data"], name="proj_prev"
                 # )
-                update_layer_in_viewer(self.viewer, h5py.File(self.scn_fn, "r")[ZFLY_CFG["io_data_structure_tomo"]["structured_h5_reader"]["io_data_structure"]["data_path"]], "proj_prev")
+                update_layer_in_viewer(
+                    self.viewer,
+                    h5py.File(self.scn_fn, "r")[
+                        ZFLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
+                            "io_data_structure"
+                        ]["data_path"]
+                    ],
+                    "proj_prev",
+                )
                 show_layers_in_viewer(self.viewer, ["proj_prev"])
             else:
                 # self.viewer.add_image(
                 #     h5py.File(self.scn_fn, "r")["/img_tomo"], name="proj_prev"
                 # )
-                update_layer_in_viewer(self.viewer, h5py.File(self.scn_fn, "r")[FLY_CFG["io_data_structure_tomo"]["structured_h5_reader"]["io_data_structure"]["data_path"]], "proj_prev")
+                update_layer_in_viewer(
+                    self.viewer,
+                    h5py.File(self.scn_fn, "r")[
+                        FLY_CFG["io_data_structure_tomo"]["structured_h5_reader"][
+                            "io_data_structure"
+                        ]["data_path"]
+                    ],
+                    "proj_prev",
+                )
                 show_layers_in_viewer(self.viewer, ["proj_prev"])
-            
+
     @disp_progress_info("missing angle calculate")
     def _is_wedge(self):
         self._cen = None
         self._trial_cen_rec_done = False
         self.__set_vol_rec_widgets()
         if self.is_wedge.value:
             self.wedge_thsh.enabled = True
@@ -439,56 +454,49 @@
         )
         xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["data_center_dir"] = str(
             self.top_dir.value / "data_center"
         )
         xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["recon_top_dir"] = str(
             self.top_dir.value
         )
-        xanes3d_tomo_tplt_cfg["scan id"]["file_params"][
-            "wedge_ang_auto_det_ref_fn"
-        ] = str(
-            self.top_dir.value / f"{self.file_type.value}_id_{self.scan_id.value}.h5"
-        )
-        xanes3d_tomo_tplt_cfg["scan id"]["file_params"][
-            "io_confg"
-        ] = self._tomo_cfg
+        xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["wedge_ang_auto_det_ref_fn"] = (
+            str(
+                self.top_dir.value
+                / f"{self.file_type.value}_id_{self.scan_id.value}.h5"
+            )
+        )
+        xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["io_confg"] = self._tomo_cfg
         xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["hardware_trig_type"] = (
             True if self.file_type.value == "tomo_zfly" else False
         )
 
-        xanes3d_tomo_tplt_cfg["scan id"]["recon_config"][
-            "recon_type"
-        ] = "Trial Cent"
+        xanes3d_tomo_tplt_cfg["scan id"]["recon_config"]["recon_type"] = "Trial Cent"
         xanes3d_tomo_tplt_cfg["scan id"]["recon_config"][
             "is_wedge"
         ] = self.is_wedge.value
 
-        xanes3d_tomo_tplt_cfg["scan id"]["data_params"][
-            "scan_id"
-        ] = self.scan_id.value
+        xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["scan_id"] = self.scan_id.value
         xanes3d_tomo_tplt_cfg["scan id"]["data_params"][
             "rot_cen"
         ] = self.cen_sch_s.value
         xanes3d_tomo_tplt_cfg["scan id"]["data_params"][
             "cen_win_s"
         ] = self.cen_sch_s.value
         xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["sli_s"] = (
             self.ref_sli.value - 10
         )
         xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["sli_e"] = (
             self.ref_sli.value + 10
         )
         xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["col_s"] = 0
-        xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["col_e"] = self._data_dim[
+        xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["col_e"] = self._data_dim[2]
+        xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["wedge_col_s"] = 0
+        xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["wedge_col_e"] = self._data_dim[
             2
         ]
-        xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["wedge_col_s"] = 0
-        xanes3d_tomo_tplt_cfg["scan id"]["data_params"]["wedge_col_e"] = (
-            self._data_dim[2]
-        )
         xanes3d_tomo_tplt_cfg["scan id"]["data_params"][
             "wedge_ang_auto_det_thres"
         ] = self.wedge_thsh.value
 
         if self.file_type.value == "tomo_zfly":
             xanes3d_tomo_tplt_cfg["scan id"]["file_params"]["io_confg"][
                 "structured_h5_reader"
@@ -535,17 +543,15 @@
                     json.dump(tem1, f, indent=4, separators=(",", ": "))
             except:
                 with open(tem["tomo_batch_recon"]["cfg_file"], "w") as f:
                     tem1 = {}
                     tem1[str(self.scan_id.value)] = xanes3d_tomo_tplt_cfg["scan id"]
                     json.dump(tem1, f, indent=4, separators=(",", ": "))
 
-        xanes3d_tomo_cfg = {
-            str(self.scan_id.value): xanes3d_tomo_tplt_cfg["scan id"]
-        }
+        xanes3d_tomo_cfg = {str(self.scan_id.value): xanes3d_tomo_tplt_cfg["scan id"]}
         with open(tem["tomo_recon"]["cfg_file"], "w") as f:
             json.dump(xanes3d_tomo_cfg, f, indent=4, separators=(",", ": "))
 
         sig = os.system(f"ipython {tomo_rec_script_fn}")
         if sig == 0:
             rm_gui_viewers(self.viewer, ["data_center"])
             self.viewer.open(self._trial_cen_dir)
@@ -568,27 +574,27 @@
 
     def _pick_cen(self):
         fns = glob.glob(str(Path(self._trial_cen_dir) / "*.tiff"))
         self._trial_cens = sorted([float(Path(fn).stem) for fn in fns])
         self.cen.value = self._trial_cens[int(self.viewer.dims.point[0])]
         self._cen = float(self.cen.value)
         if self.find_multi_cen.value:
-            with open(cfg_fn, "r") as f:    
-                batch_tplt_fn = json.load(f)["tomo_batch_recon"]["cfg_file"]       
+            with open(cfg_fn, "r") as f:
+                batch_tplt_fn = json.load(f)["tomo_batch_recon"]["cfg_file"]
             with open(batch_tplt_fn, "r") as ft:
                 tem = json.load(ft)
             with open(batch_tplt_fn, "w") as ft:
                 tem[str(self.scan_id.value)]["data_params"]["rot_cen"] = self._cen
                 tem[str(self.scan_id.value)]["data_params"]["sli_s"] = 0
                 tem[str(self.scan_id.value)]["data_params"]["sli_e"] = self._data_dim[1]
                 tem[str(self.scan_id.value)]["recon_config"]["recon_type"] = "Vol Recon"
                 json.dump(tem, ft, indent=4, separators=(",", ": "))
         else:
             with open(cfg_fn, "r") as f:
-                tomo_tplt_fn = json.load(f)["tomo_recon"]["cfg_file"]            
+                tomo_tplt_fn = json.load(f)["tomo_recon"]["cfg_file"]
             with open(tomo_tplt_fn, "r") as ft:
                 tem = json.load(ft)
             tem[list(tem.keys())[0]]["data_params"]["rot_cen"] = self._cen
             tem[list(tem.keys())[0]]["data_params"]["sli_s"] = 0
             tem[list(tem.keys())[0]]["data_params"]["sli_e"] = self._data_dim[1]
             tem[list(tem.keys())[0]]["recon_config"]["recon_type"] = "Vol Recon"
             with open(tomo_tplt_fn, "w") as ft:
@@ -608,15 +614,15 @@
         if self._cen is None:
             self.viewer.status = (
                 "Please pick the best center for volume reconstruction."
             )
             print("Please pick the best center for volume reconstruction.")
         else:
             rm_gui_viewers(self.viewer, ["data_center"])
-            
+
             if self.find_multi_cen.value:
                 sig = os.system(f"ipython {tomo_batch_rec_script_fn}")
             else:
                 sig = os.system(f"ipython {tomo_rec_script_fn}")
                 if sig == 0:
                     with open(cfg_fn, "r") as f:
                         with open(json.load(f)["tomo_recon"]["cfg_file"], "r") as ft:
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import dask.array as da
 import h5py
 import json
 from pathlib import Path
 import matplotlib.pyplot as plt
 from magicgui import widgets
 
-from TXM_Sandbox.gui.gui_components import (
+from ...gui.gui_components import (
     determine_element,
     determine_fitting_energy_range,
     scale_eng_list,
     def_dflt_eng_rgn,
 )
-from TXM_Sandbox.napari_gui.utils.io import create_hdf5_from_json
-from TXM_Sandbox.napari_gui.utils.misc import (
+from ..utils.io import create_hdf5_from_json
+from ..utils.misc import (
     set_data_widget,
     overlap_roi,
     update_layer_in_viewer,
     show_layers_in_viewer,
     rm_gui_viewers,
     disp_progress_info,
 )
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 import h5py
 import json
 import dask.array as da
 import datetime
 from pathlib import Path
 from magicgui import widgets
 
-from TXM_Sandbox.gui.gui_components import (
+from ...gui.gui_components import (
     check_file_availability,
 )
 
-from TXM_Sandbox.napari_gui.utils.misc import (
+from ..utils.misc import (
     set_data_widget,
     overlap_roi,
     update_layer_in_viewer,
     show_layers_in_viewer,
     rm_gui_viewers,
     disp_progress_info,
 )
-from TXM_Sandbox.napari_gui.dicts.data_struct_dict import ZFLY_CFG, FLY_CFG
+from ..dicts.data_struct_dict import ZFLY_CFG, FLY_CFG
 
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 xanes3d_auto_cen_reg_script_fn = (
     Path(__file__).parents[1] / "scripts/xanes3d_tomo_autocent_cmd.py"
 )
 xanes2d_img_auto_cen_script_fn = (
@@ -54,26 +54,36 @@
 
 def get_tomo_xanes3d_rec_id_e_choices(ComboBox):
     global _TOMO_XANES3D_REC_ID_E_CHOICES
     return _TOMO_XANES3D_REC_ID_E_CHOICES
 
 
 def check_cfg_type(json_cfg):
-    with open(json_cfg, 'r') as f:
+    with open(json_cfg, "r") as f:
         tem = json.load(f)
 
     if "run_type" in tem.keys():
         return "xanes3d_autocen&reg"
     elif len(tem.keys()) == 1:
         key = tem[list(tem.keys())[0]]
-        if np.all(item in tem[key].keys for item in ["file_params", "recon_config", "flt_params", "data_params", "alg_params"]):
+        if np.all(
+            item in tem[key].keys
+            for item in [
+                "file_params",
+                "recon_config",
+                "flt_params",
+                "data_params",
+                "alg_params",
+            ]
+        ):
             return "xanes3d_tomo_tplt"
     else:
         return None
 
+
 ################################################################################
 #             auto reconstruction and alignment for XANES3D                    #
 ################################################################################
 class xanes_reg_gui:
     def __init__(self, viewer):
         self.viewer = viewer
         self._tomo_cfg = None
@@ -347,45 +357,57 @@
                 self.ang_corr_range.enabled = False
             self.test_run.enabled = True
             self.close_file.enabled = True
 
     def __3dxanes_tomo_show_sli(self, mode="auto_cen"):
         if mode == "auto_cen":
             try:
-                update_layer_in_viewer(self.viewer, tifffile.imread(
-                    str(self.rec_fntpl).format(
-                        self.ref_scan_id.value,
-                        str(self.ref_sli.value).zfill(5),
-                    )
-                ), "xanes_raw_viewer")
+                update_layer_in_viewer(
+                    self.viewer,
+                    tifffile.imread(
+                        str(self.rec_fntpl).format(
+                            self.ref_scan_id.value,
+                            str(self.ref_sli.value).zfill(5),
+                        )
+                    ),
+                    "xanes_raw_viewer",
+                )
             except Exception as e:
                 self.op_status.value = (
                     "Something is wrong. Please check terminal for more information."
                 )
                 print(f"{str(e)=}")
         elif mode == "recon_roi":
             if self._3dxanes_rec_roiz_old_val[0] != self.rec_roiz.value[0]:
                 try:
-                    update_layer_in_viewer(self.viewer, tifffile.imread(
-                        str(self.rec_fntpl).format(
-                            self.ref_scan_id.value,
-                            str(self.rec_roiz.value[0]).zfill(5),
-                        )
-                    ), "xanes_raw_viewer")
+                    update_layer_in_viewer(
+                        self.viewer,
+                        tifffile.imread(
+                            str(self.rec_fntpl).format(
+                                self.ref_scan_id.value,
+                                str(self.rec_roiz.value[0]).zfill(5),
+                            )
+                        ),
+                        "xanes_raw_viewer",
+                    )
                 except Exception as e:
                     self.op_status.value = "Something is wrong. Please check terminal for more information."
                     print(str(e))
             elif self._3dxanes_rec_roiz_old_val[1] != self.rec_roiz.value[1]:
                 try:
-                    update_layer_in_viewer(self.viewer, tifffile.imread(
-                        str(self.rec_fntpl).format(
-                            self.ref_scan_id.value,
-                            str(self.rec_roiz.value[1]).zfill(5),
-                        )
-                    ), "xanes_raw_viewer")                   
+                    update_layer_in_viewer(
+                        self.viewer,
+                        tifffile.imread(
+                            str(self.rec_fntpl).format(
+                                self.ref_scan_id.value,
+                                str(self.rec_roiz.value[1]).zfill(5),
+                            )
+                        ),
+                        "xanes_raw_viewer",
+                    )
                 except Exception as e:
                     self.op_status.value = "Something is wrong. Please check terminal for more information."
                     print(str(e))
         rng = (
             self.viewer.layers["xanes_raw_viewer"].data.max()
             - self.viewer.layers["xanes_raw_viewer"].data.min()
         )
@@ -929,34 +951,42 @@
             if cfg_type == "xanes3d_tomo_tplt":
                 with open(self._tomo_tplt_fn, "r") as f:
                     tem = json.load(f)
                     self.ref_scan_id.value = list(tem.keys())[0]
                     self._ref_rec_tplt = tem[list(tem.keys())[0]]
                 if (
                     "tomo_zfly"
-                    in self._ref_rec_tplt["file_params"]["io_confg"]["tomo_raw_fn_template"]
+                    in self._ref_rec_tplt["file_params"]["io_confg"][
+                        "tomo_raw_fn_template"
+                    ]
                 ):
                     self._tomo_cfg = ZFLY_CFG["io_data_structure_xanes3D"]
                 elif (
                     "fly_scan"
-                    in self._ref_rec_tplt["file_params"]["io_confg"]["tomo_raw_fn_template"]
+                    in self._ref_rec_tplt["file_params"]["io_confg"][
+                        "tomo_raw_fn_template"
+                    ]
                 ):
                     self._tomo_cfg = FLY_CFG["io_data_structure_xanes3D"]
                 self.__3dxanes_comp_tomo_fntpl()
                 self.__3dxanes_tomo_check_avail_id_s()
                 self.__3dxanes_tomo_check_avail_id_e()
                 self.__3dxanes_set_scan_id_lims()
                 self.__3dxanes_set_widget()
                 self.__3dxanes_set_roi_lims()
                 self.__3dxanes_tomo_show_sli(mode="auto_cen")
                 self.__xanes_reset_run_status()
                 self.__xanes_reset_run_buttons()
             else:
-                self.op_status.value = "wrong type of json cfg file. check error message in terminal"
-                print("The required json file should have file name starting with 'xanes3d_tomo_tplt_cfg'.")
+                self.op_status.value = (
+                    "wrong type of json cfg file. check error message in terminal"
+                )
+                print(
+                    "The required json file should have file name starting with 'xanes3d_tomo_tplt_cfg'."
+                )
         else:
             self.__2dxanes_check_in_file()
             self.__2dxanes_set_widget()
             self.__2dxanes_set_roi_lims()
             self.__2dxanes_show_sli(mode="auto_reg")
             _min = self.viewer.layers["xanes_raw_viewer"].data[self.ref_sli.value].min()
             _max = self.viewer.layers["xanes_raw_viewer"].data[self.ref_sli.value].max()
@@ -1029,15 +1059,17 @@
                 with h5py.File(
                     tem["aut_xns3d_pars"]["xanes3d_sav_trl_reg_fn"], "r"
                 ) as f:
                     for key in f["/auto_centering/"].keys():
                         trial_imgs.append(
                             f[f"/auto_centering/{key}/optimization itr 1/trial_rec"][:]
                         )
-                update_layer_in_viewer(self.viewer, np.array(trial_imgs), "autocent_check")
+                update_layer_in_viewer(
+                    self.viewer, np.array(trial_imgs), "autocent_check"
+                )
                 show_layers_in_viewer(self.viewer, ["autocent_check"])
             if sig == 0:
                 self._test_run_done = True
             else:
                 self._test_run_done = False
                 self.op_status.value = "auto centering fails"
                 print("auto centering fails")
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import dask.array as da
 import h5py
 import json
 from pathlib import Path
 from magicgui import widgets
 
-from TXM_Sandbox.napari_gui.utils.misc import (
+from ..utils.misc import (
     check_avail_items,
     get_slcd_ds_path,
     update_layer_in_viewer,
     show_layers_in_viewer,
     rm_gui_viewers,
     disp_progress_info,
 )
@@ -130,20 +130,21 @@
             self.vis_data_cntrst_highlim.enabled = False
             self.vis_test_mask_thsh.enabled = False
             self.confirm_mask_thsh.enabled = False
             self.vis_mk_mask.enabled = False
             self.close_file.enabled = False
 
     def __set_layers_order(self):
-        if ("vis_data" in self.viewer.layers) and (
-            "mask_viewer" in self.viewer.layers
-        ):
+        if ("vis_data" in self.viewer.layers) and ("mask_viewer" in self.viewer.layers):
             self.viewer.layers.move_multiple(
-                [self.viewer.layers.index(self.viewer.layers["vis_data"]), self.viewer.layers.index(self.viewer.layers["mask_viewer"]),],
-                0
+                [
+                    self.viewer.layers.index(self.viewer.layers["vis_data"]),
+                    self.viewer.layers.index(self.viewer.layers["mask_viewer"]),
+                ],
+                0,
             )
             self.viewer.layers["mask_viewer"].opacity = 0.2
             self.viewer.layers["mask_viewer"].colormap = "yellow"
 
     def __avail_item_slcd(self):
         if self._vis_data_ready:
             (self._in_dat_path_in_h5, _in_dat_desc, _in_dat_dtype) = get_slcd_ds_path(
@@ -335,16 +336,22 @@
                 .compute()
                 .astype(np.int8)
             )
 
         elif self.vis_in_data_type.value == "3D XANES":
             thshed_img = (
                 (
-                    (self._vis_data[*self.viewer.dims.current_step[:-2], ...] > float(self.vis_data_cntrst_lowlim.value))
-                    & (self._vis_data[*self.viewer.dims.current_step[:-2], ...] < float(self.vis_data_cntrst_highlim.value))
+                    (
+                        self._vis_data[*self.viewer.dims.current_step[:-2], ...]
+                        > float(self.vis_data_cntrst_lowlim.value)
+                    )
+                    & (
+                        self._vis_data[*self.viewer.dims.current_step[:-2], ...]
+                        < float(self.vis_data_cntrst_highlim.value)
+                    )
                 )
                 .compute()
                 .astype(np.int8)
             )
 
         rm_gui_viewers(self.viewer, ["mask_viewer"])
         update_layer_in_viewer(self.viewer, thshed_img, "mask_viewer")
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/napari_gui.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/napari_gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 
 import napari
 import skimage.data
 import skimage.filters
 
-from TXM_Sandbox.napari_gui.guis.tomo_gui import tomo_gui
-from TXM_Sandbox.napari_gui.guis.xanes_reg_gui import xanes_reg_gui
-from TXM_Sandbox.napari_gui.guis.xanes_fit_gui import xanes_fit_gui
-from TXM_Sandbox.napari_gui.guis.xanes_vis_gui import xanes_vis_gui
-from TXM_Sandbox.napari_gui.guis.convert_data_gui import convt_dat_gui
-from TXM_Sandbox.napari_gui.guis.appl_mask_gui import appl_mask_gui
+from .guis.tomo_gui import tomo_gui
+from .guis.xanes_reg_gui import xanes_reg_gui
+from .guis.xanes_fit_gui import xanes_fit_gui
+from .guis.xanes_vis_gui import xanes_vis_gui
+from .guis.convert_data_gui import convt_dat_gui
+from .guis.appl_mask_gui import appl_mask_gui
 
 
 def txm_gui():
     viewer = napari.Viewer()
     _tomo_gui = tomo_gui(viewer)
     _xanes_reg_gui = xanes_reg_gui(viewer)
     _xanes_fit_gui = xanes_fit_gui(viewer)
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 
-from TXM_Sandbox.utils.tomo_recon_tools import run_engine
-from TXM_Sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
+from txm_sandbox.utils.tomo_recon_tools import run_engine
+from txm_sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 
 with open(cfg_fn, "r") as f:
     with open(json.load(f)["tomo_batch_recon"]["cfg_file"], "r") as ft:
         tem = json.load(ft)
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 
-from TXM_Sandbox.utils.tomo_recon_tools import run_engine
-from TXM_Sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
+from txm_sandbox.utils.tomo_recon_tools import run_engine
+from txm_sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 
 with open(cfg_fn, "r") as f:
     with open(json.load(f)["tomo_recon"]["cfg_file"], "r") as ft:
         tem = json.load(ft)
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,15 @@
-# import os, h5py
-# import numpy as np
-# import pandas as pd
-# from scipy.ndimage import zoom
-# import TXM_Sandbox.utils.xanes_math as xm
-# import TXM_Sandbox.utils.xanes_analysis as xa
-# from TXM_Sandbox.utils.misc import str2bool
-# from copy import deepcopy
-
-# inf = np.inf
-
-
 import numpy as np
 from scipy.ndimage import zoom
 
 from pathlib import Path
 import json
 import h5py
 
-import TXM_Sandbox.utils.xanes_analysis as xa
+import txm_sandbox.utils.xanes_analysis as xa
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 
 def read_hdf5_group_to_dict(fp, group, is_file=False):
     if is_file:
         with h5py.File(fp, "r") as f:
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import numpy as np
 from multiprocess import freeze_support
 
 import h5py
 import dask.array as da
 
-from TXM_Sandbox.utils import xanes_regtools as xr
+from txm_sandbox.utils import xanes_regtools as xr
 
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 with open(cfg_fn, "r") as f:
     with open(json.load(f)["xanes2d_reg"]["cfg_file"], "r") as ft:
         reg_cfg = json.load(ft)
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from scipy.ndimage import zoom
 
 from pathlib import Path
 import json
 import h5py
 
-import TXM_Sandbox.utils.xanes_analysis as xa
+import txm_sandbox.utils.xanes_analysis as xa
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 
 def read_hdf5_group_to_dict(fp, group, is_file=False):
     if is_file:
         with h5py.File(fp, "r") as f:
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from pathlib import Path
 
-from TXM_Sandbox.utils.tomo_recon_tools import (
+from txm_sandbox.utils.tomo_recon_tools import (
     xanes3d_auto_tomo_rec,
     prep_xns3d_auto_tomo_cfg,
     tomo_auto_center,
 )
-from TXM_Sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
+from txm_sandbox.utils.io import data_reader, tomo_h5_reader, data_info, tomo_h5_info
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 with open(cfg_fn, "r") as f:
     with open(json.load(f)["xanes3d_auto_cen"]["cfg_file"], "r") as ft:
         tem = json.load(ft)
 
@@ -19,15 +19,15 @@
         tem2 = json.load(f)
         params = tem2[list(tem2.keys())[0]]
         params["aut_xns3d_pars"] = tem["aut_xns3d_pars"]
     print(json.dumps(params, indent=4))
 
     params["file_params"]["reader"] = data_reader(tomo_h5_reader)
     params["file_params"]["info_reader"] = data_info(tomo_h5_info)
-    
+
     if tem["run_type"] == "autocen":
         params["aut_xns3d_pars"][
             "xanes3d_h5_ds_path"
         ] = "/registration_results/reg_results/registered_xanes3D"
         prep_xns3d_auto_tomo_cfg(params)
         params["aut_tomo_pars"]["auto_rec"] = False
         success = tomo_auto_center(params)
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 import numpy as np
 from multiprocess import freeze_support
 
 import h5py
 import dask.array as da
 
-from TXM_Sandbox.utils import xanes_regtools as xr
+from txm_sandbox.utils import xanes_regtools as xr
 
 
 cfg_fn = Path(__file__).parents[1] / "configs/txm_simple_gui_script_cfg.json"
 
 with open(cfg_fn, "r") as f:
     with open(json.load(f)["xanes2d_reg"]["cfg_file"], "r") as ft:
         reg_cfg = json.load(ft)
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import numpy as np
 import h5py
-import json
 
 
 def create_hdf5_from_json(structure, file_path):
-    with h5py.File(file_path, 'r+') as f:
+    with h5py.File(file_path, "r+") as f:
         create_group(f, None, structure)
 
 
 def create_group(parent_group, group_name, structure):
     if group_name is None:
         group = parent_group
     else:
@@ -27,23 +25,21 @@
 
 def create_dataset(group, key, value):
     group.create_dataset(key, data=value)
 
 
 def read_hdf5_group_to_dict(fp, group, is_file=False):
     if is_file:
-        with h5py.File(fp, 'r') as f:
+        with h5py.File(fp, "r") as f:
             return recursively_load_dict(f[group])
     else:
         return recursively_load_dict(fp[group])
 
+
 def recursively_load_dict(group):
     output = {}
     for key, val in group.items():
         if isinstance(val, h5py.Dataset):
             output[key] = val[...]
         elif isinstance(val, h5py.Group):
             output[key] = recursively_load_dict(val)
     return output
-
-
-
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import h5py
-import json
 from pathlib import Path
 from qtpy.QtWidgets import QApplication
 
-from TXM_Sandbox.dicts import customized_struct_dict as dat_dict
+from ...dicts import customized_struct_dict as dat_dict
 
 
 def check_avail_items(fn, file_type):
     choices = []
     if Path(fn).exists() & Path(fn).is_file():
         with h5py.File(fn, "r") as f:
             keys = list(f.keys())
@@ -64,23 +63,25 @@
                     except:
                         pass
     return choices
 
 
 def disp_progress_info(info):
     def decorated_func(func):
-        def inner_func(self): 
+        def inner_func(self):
             self.op_status.value = "doing " + info + " ..."
             QApplication.processEvents()
-            print("doing " + info + " ...")           
-            func(self)        
+            print("doing " + info + " ...")
+            func(self)
             self.op_status.value = info + " finished"
             print(info + " finished")
             return
+
         return inner_func
+
     return decorated_func
 
 
 def get_slcd_ds_path(fn, file_type, _slcd_item):
     if not isinstance(fn, str):
         fn = str(fn)
     if (file_type == "TOMO Raw") and _slcd_item:
@@ -148,15 +149,17 @@
             _in_dat_desc = dat_dict.XANES3D_ANA_ITEM_DICT[_slcd_item]["description"]
             _in_dat_dtype = dat_dict.XANES3D_ANA_ITEM_DICT[_slcd_item]["dtype"]
     return _in_dat_path_in_h5, _in_dat_desc, _in_dat_dtype
 
 
 def info_reader(scn_fn, dtype="data", cfg=None):
     with h5py.File(scn_fn, "r") as f:
-        return f[cfg["structured_h5_reader"]["io_data_structure"][f"{dtype}_path"]].shape
+        return f[
+            cfg["structured_h5_reader"]["io_data_structure"][f"{dtype}_path"]
+        ].shape
 
 
 def overlap_roi(viewer, gui, mode="auto_cen"):
     if mode == "auto_cen":
         rm_gui_viewers(viewer, ["auto_cen_roi"])
         if "recon_roi" in viewer.layers:
             viewer.layers["recon_roi"].visible = False
@@ -255,9 +258,7 @@
     viewer.reset_view()
 
 
 def update_layer_in_viewer(viewer, data, layer: str):
     rm_gui_viewers(viewer, [layer])
     viewer.add_image(data, name=layer)
     viewer.reset_view()
-
-
```

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/io.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/misc.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/plotlib.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_regtools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0/TXM_Sandbox.egg-info/PKG-INFO` & `txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TXM_Sandbox
-Version: 0.3.0
+Name: txm_sandbox
+Version: 0.3.0.post1
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.0/setup.py` & `txm_sandbox-0.3.0.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 Created on Thu Jul 16 22:20:14 2020
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
-setup(name='TXM_Sandbox',
-      version='0.3.0',
+setup(name='txm_sandbox',
+      version='0.3.0.post1',
       description='Integrated Spectro-Imaging Analysis Toolbox',
       url='https://github.com/xianghuix/TXM_Sandbox',
       author='Xianghui Xiao',
       author_email='xianghuix@gmail.com',
       license='MIT',
       packages=find_packages(),
       install_requires=[
@@ -36,8 +36,8 @@
             'pystackreg',
             'silx',
             'napari'
       ],
       zip_safe=False,
       include_package_data=True,
       package_data={
-          "":['LICENSE', 'README.md', 'TXM_Sandbox/tmp/readme.txt', 'TXM_Sandbox/config/*.json', 'TXM_GUI3.ipynb', 'txm_gui.py']})
+          "":['LICENSE', 'README.md', 'txm_sandbox/tmp/readme.txt', 'txm_sandbox/napari_gui/configs/*.json', 'txm_sandbox/config/*.json']})
```

