# Comparing `tmp/txm_sandbox-0.3.0.post1.tar.gz` & `tmp/txm_sandbox-0.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txm_sandbox-0.3.0.post1.tar", last modified: Thu Apr 18 22:42:48 2024, max compression
+gzip compressed data, was "txm_sandbox-0.3.0.post2.tar", last modified: Thu Apr 18 22:57:16 2024, max compression
```

## Comparing `txm_sandbox-0.3.0.post1.tar` & `txm_sandbox-0.3.0.post2.tar`

### file list

```diff
@@ -1,87 +1,97 @@
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1070 2024-04-18 03:35:27.000000 txm_sandbox-0.3.0.post1/LICENSE
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      147 2024-04-18 03:34:56.000000 txm_sandbox-0.3.0.post1/MANIFEST.in
--rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1639 2024-04-18 03:35:09.000000 txm_sandbox-0.3.0.post1/README.md
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     2565 2024-04-18 11:27:34.000000 txm_sandbox-0.3.0.post1/TXM_GUI2.ipynb
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       38 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/setup.cfg
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1155 2024-04-18 22:38:23.000000 txm_sandbox-0.3.0.post1/setup.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.943797 txm_sandbox-0.3.0.post1/txm_sandbox/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.943797 txm_sandbox-0.3.0.post1/txm_sandbox/config/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/config/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.947797 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3848 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/config_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61110 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/customized_struct_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      755 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/sklearn_opt_dict.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      583 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/dicts/xanes_analysis_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.947797 txm_sandbox-0.3.0.post1/txm_sandbox/external/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/external/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      253 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/external/user_io.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    32500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/conv_data_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    74137 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/gen_algn_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    79463 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/gui_components.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    36752 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/io_config_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15709 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/main_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      795 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/misc_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   169879 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/tomo_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   204783 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes2D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   202060 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes3D_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    91679 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_analysis_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)   203257 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_fitting_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/configs/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/configs/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/__init__.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     5528 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/data_struct_dict.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.951797 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      106 2024-04-18 19:44:50.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15327 2024-04-18 19:47:10.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/appl_mask_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     9587 2024-04-18 19:52:32.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/convert_data_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    25806 2024-04-18 19:53:16.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/tomo_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     1503 2024-04-18 22:36:58.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/txm_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    23082 2024-04-18 19:53:44.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    48430 2024-04-18 19:54:08.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15803 2024-04-18 19:54:19.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)     1533 2024-04-18 20:23:11.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/napari_gui.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.955798 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      605 2024-04-18 20:05:13.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      599 2024-04-18 20:05:03.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    15251 2024-04-18 19:59:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2428 2024-04-18 20:01:32.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16707 2024-04-18 20:01:56.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1197 2024-04-18 20:04:22.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2029 2024-04-18 20:04:35.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.955798 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1264 2024-04-18 20:05:59.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/io.py
--rw-r--r--   0 xiao      (1000) xiao      (1000)    10590 2024-04-18 20:06:46.000000 txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/misc.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.955798 txm_sandbox-0.3.0.post1/txm_sandbox/tmp/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/tmp/__init__.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/txm_sandbox/utils/
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/__init__.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    16672 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/io.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    14410 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/lineshapes.py
--rwxrwxr-x   0 xiao      (1000) xiao      (1000)     4246 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/misc.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     1439 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/plotlib.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    61837 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/reg_algs.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    70498 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/tomo_recon_tools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    36738 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2342 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_image_utils.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    23436 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_math.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     6083 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_post_analysis.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)    84774 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_regtools.py
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     3266 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_spectra_filters.py
-drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:42:48.959797 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/
--rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/PKG-INFO
--rw-rw-r--   0 xiao      (1000) xiao      (1000)     2504 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/SOURCES.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/dependency_links.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/not-zip-safe
--rw-rw-r--   0 xiao      (1000) xiao      (1000)      170 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/requires.txt
--rw-rw-r--   0 xiao      (1000) xiao      (1000)       12 2024-04-18 22:42:48.000000 txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/top_level.txt
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.931082 txm_sandbox-0.3.0.post2/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1070 2024-04-18 03:35:27.000000 txm_sandbox-0.3.0.post2/LICENSE
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      147 2024-04-18 03:34:56.000000 txm_sandbox-0.3.0.post2/MANIFEST.in
+-rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-18 22:57:16.931082 txm_sandbox-0.3.0.post2/PKG-INFO
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1639 2024-04-18 03:35:09.000000 txm_sandbox-0.3.0.post2/README.md
+-rwxrwxr-x   0 xiao      (1000) xiao      (1000)     2565 2024-04-18 11:27:34.000000 txm_sandbox-0.3.0.post2/TXM_GUI2.ipynb
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       38 2024-04-18 22:57:16.931082 txm_sandbox-0.3.0.post2/setup.cfg
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1130 2024-04-18 22:55:57.000000 txm_sandbox-0.3.0.post2/setup.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.915082 txm_sandbox-0.3.0.post2/txm_sandbox/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.919082 txm_sandbox-0.3.0.post2/txm_sandbox/config/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     5092 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/config/XANES2D_GUI_config.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/config/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       45 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/config/analysis_tool_gui_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      497 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/config/io_tomo_h5_data_structure.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/config/io_xanes2D_h5_data_structure.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      616 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/config/io_xanes3D_h5_data_structure.json
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.919082 txm_sandbox-0.3.0.post2/txm_sandbox/dicts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/dicts/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3848 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/dicts/config_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    61110 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/dicts/customized_struct_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      755 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/dicts/sklearn_opt_dict.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      583 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/dicts/xanes_analysis_dict.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.919082 txm_sandbox-0.3.0.post2/txm_sandbox/external/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/external/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      253 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/external/user_io.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.923082 txm_sandbox-0.3.0.post2/txm_sandbox/gui/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    32500 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/conv_data_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    74137 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/gen_algn_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    79463 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/gui_components.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    36752 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/io_config_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15709 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/main_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      795 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/misc_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   169879 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/tomo_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   204783 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes2D_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   202060 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes3D_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    91679 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes_analysis_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)   203257 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes_fitting_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.923082 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/__init__.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.923082 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/configs/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/configs/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      915 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      957 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      899 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2389 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1362 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.923082 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/dicts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/dicts/__init__.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)     5528 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/dicts/data_struct_dict.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.927082 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      106 2024-04-18 19:44:50.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15327 2024-04-18 19:47:10.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/appl_mask_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     9587 2024-04-18 19:52:32.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/convert_data_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    25806 2024-04-18 19:53:16.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/tomo_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    23082 2024-04-18 19:53:44.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/xanes_fit_gui.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    48430 2024-04-18 19:54:08.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/xanes_reg_gui.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15803 2024-04-18 19:54:19.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/xanes_vis_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.927082 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      605 2024-04-18 20:05:13.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      599 2024-04-18 20:05:03.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    15251 2024-04-18 19:59:48.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2428 2024-04-18 20:01:32.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    16707 2024-04-18 20:01:56.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1197 2024-04-18 20:04:22.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2029 2024-04-18 20:04:35.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)     1533 2024-04-18 20:23:11.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/txm_gui.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.927082 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/utils/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      181 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/utils/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1264 2024-04-18 20:05:59.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/utils/io.py
+-rw-r--r--   0 xiao      (1000) xiao      (1000)    10590 2024-04-18 20:06:46.000000 txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/utils/misc.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.927082 txm_sandbox-0.3.0.post2/txm_sandbox/tmp/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/tmp/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       69 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/tmp/readme.txt
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.931082 txm_sandbox-0.3.0.post2/txm_sandbox/utils/
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      107 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/__init__.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    16672 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/io.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    14410 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/lineshapes.py
+-rwxrwxr-x   0 xiao      (1000) xiao      (1000)     4246 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/misc.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     1439 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/plotlib.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    61837 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/reg_algs.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    70498 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/tomo_recon_tools.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    36738 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_analysis.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     2342 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_image_utils.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    23436 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_math.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     6083 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_post_analysis.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)    84774 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_regtools.py
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3266 2024-04-18 02:40:37.000000 txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_spectra_filters.py
+drwxrwxr-x   0 xiao      (1000) xiao      (1000)        0 2024-04-18 22:57:16.931082 txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/
+-rw-r--r--   0 xiao      (1000) xiao      (1000)      712 2024-04-18 22:57:16.000000 txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/PKG-INFO
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)     3045 2024-04-18 22:57:16.000000 txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 22:57:16.000000 txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)        1 2024-04-18 22:57:16.000000 txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/not-zip-safe
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)      170 2024-04-18 22:57:16.000000 txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/requires.txt
+-rw-rw-r--   0 xiao      (1000) xiao      (1000)       12 2024-04-18 22:57:16.000000 txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/top_level.txt
```

### Comparing `txm_sandbox-0.3.0.post1/LICENSE` & `txm_sandbox-0.3.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/PKG-INFO` & `txm_sandbox-0.3.0.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.0.post1/README.md` & `txm_sandbox-0.3.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/TXM_GUI2.ipynb` & `txm_sandbox-0.3.0.post2/TXM_GUI2.ipynb`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/setup.py` & `txm_sandbox-0.3.0.post2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: xiao
 """
 
 from setuptools import setup, find_packages
 
 setup(name='txm_sandbox',
-      version='0.3.0.post1',
+      version='0.3.0.post2',
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
-          "":['LICENSE', 'README.md', 'txm_sandbox/tmp/readme.txt', 'txm_sandbox/napari_gui/configs/*.json', 'txm_sandbox/config/*.json']})
+          "txm_sandbox":['LICENSE', 'README.md', 'tmp/readme.txt', 'napari_gui/configs/*.json', 'config/*.json']})
```

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/config_dict.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/dicts/config_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/customized_struct_dict.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/dicts/customized_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/sklearn_opt_dict.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/dicts/sklearn_opt_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/dicts/xanes_analysis_dict.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/dicts/xanes_analysis_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/conv_data_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/conv_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/gen_algn_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/gen_algn_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/gui_components.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/gui_components.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/io_config_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/io_config_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/main_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/misc_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/misc_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/tomo_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes2D_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes2D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes3D_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes3D_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_analysis_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes_analysis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/gui/xanes_fitting_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/gui/xanes_fitting_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/dicts/data_struct_dict.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/dicts/data_struct_dict.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/appl_mask_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/appl_mask_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/convert_data_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/convert_data_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/tomo_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/tomo_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/txm_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/txm_gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 
 import napari
 import skimage.data
 import skimage.filters
 
-from .tomo_gui import tomo_gui
-from .xanes_reg_gui import xanes_reg_gui
-from .xanes_fit_gui import xanes_fit_gui
-from .xanes_vis_gui import xanes_vis_gui
-from .convert_data_gui import convt_dat_gui
-from .appl_mask_gui import appl_mask_gui
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

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_fit_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/xanes_fit_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_reg_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/xanes_reg_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/guis/xanes_vis_gui.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/guis/xanes_vis_gui.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/io.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/napari_gui/utils/misc.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/napari_gui/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/io.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/io.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/lineshapes.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/lineshapes.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/misc.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/misc.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/plotlib.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/plotlib.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/reg_algs.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/reg_algs.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/tomo_recon_tools.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/tomo_recon_tools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_analysis.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_image_utils.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_image_utils.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_math.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_math.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_post_analysis.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_post_analysis.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_regtools.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_regtools.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox/utils/xanes_spectra_filters.py` & `txm_sandbox-0.3.0.post2/txm_sandbox/utils/xanes_spectra_filters.py`

 * *Files identical despite different names*

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/PKG-INFO` & `txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txm_sandbox
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: Integrated Spectro-Imaging Analysis Toolbox
 Home-page: https://github.com/xianghuix/TXM_Sandbox
 Author: Xianghui Xiao
 Author-email: xianghuix@gmail.com
 License: MIT
 License-File: LICENSE
 Requires-Dist: python>=3.11
```

### Comparing `txm_sandbox-0.3.0.post1/txm_sandbox.egg-info/SOURCES.txt` & `txm_sandbox-0.3.0.post2/txm_sandbox.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 txm_sandbox/__init__.py
 txm_sandbox.egg-info/PKG-INFO
 txm_sandbox.egg-info/SOURCES.txt
 txm_sandbox.egg-info/dependency_links.txt
 txm_sandbox.egg-info/not-zip-safe
 txm_sandbox.egg-info/requires.txt
 txm_sandbox.egg-info/top_level.txt
+txm_sandbox/config/XANES2D_GUI_config.json
 txm_sandbox/config/__init__.py
+txm_sandbox/config/analysis_tool_gui_cfg.json
+txm_sandbox/config/io_tomo_h5_data_structure.json
+txm_sandbox/config/io_xanes2D_h5_data_structure.json
+txm_sandbox/config/io_xanes3D_h5_data_structure.json
 txm_sandbox/dicts/__init__.py
 txm_sandbox/dicts/config_dict.py
 txm_sandbox/dicts/customized_struct_dict.py
 txm_sandbox/dicts/sklearn_opt_dict.py
 txm_sandbox/dicts/xanes_analysis_dict.py
 txm_sandbox/external/__init__.py
 txm_sandbox/external/user_io.py
@@ -27,23 +32,27 @@
 txm_sandbox/gui/misc_gui.py
 txm_sandbox/gui/tomo_gui.py
 txm_sandbox/gui/xanes2D_gui.py
 txm_sandbox/gui/xanes3D_gui.py
 txm_sandbox/gui/xanes_analysis_gui.py
 txm_sandbox/gui/xanes_fitting_gui.py
 txm_sandbox/napari_gui/__init__.py
-txm_sandbox/napari_gui/napari_gui.py
+txm_sandbox/napari_gui/txm_gui.py
 txm_sandbox/napari_gui/configs/__init__.py
+txm_sandbox/napari_gui/configs/txm_simple_gui_script_cfg.json
+txm_sandbox/napari_gui/configs/xanes2d_image_autoreg_cfg.json
+txm_sandbox/napari_gui/configs/xanes3d_tomo_autocent_cfg.json
+txm_sandbox/napari_gui/configs/xanes3d_tomo_template_cfg.json
+txm_sandbox/napari_gui/configs/xanes_proc_data_struct_cfg.json
 txm_sandbox/napari_gui/dicts/__init__.py
 txm_sandbox/napari_gui/dicts/data_struct_dict.py
 txm_sandbox/napari_gui/guis/__init__.py
 txm_sandbox/napari_gui/guis/appl_mask_gui.py
 txm_sandbox/napari_gui/guis/convert_data_gui.py
 txm_sandbox/napari_gui/guis/tomo_gui.py
-txm_sandbox/napari_gui/guis/txm_gui.py
 txm_sandbox/napari_gui/guis/xanes_fit_gui.py
 txm_sandbox/napari_gui/guis/xanes_reg_gui.py
 txm_sandbox/napari_gui/guis/xanes_vis_gui.py
 txm_sandbox/napari_gui/scripts/__init__.py
 txm_sandbox/napari_gui/scripts/tomo_batch_recon_cmd.py
 txm_sandbox/napari_gui/scripts/tomo_recon_cmd.py
 txm_sandbox/napari_gui/scripts/xanes2D_fit_cmd.py
@@ -51,14 +60,15 @@
 txm_sandbox/napari_gui/scripts/xanes3D_fit_cmd.py
 txm_sandbox/napari_gui/scripts/xanes3d_tomo_autocent_cmd.py
 txm_sandbox/napari_gui/scripts/xnaes2d_image_autoreg_cmd.py
 txm_sandbox/napari_gui/utils/__init__.py
 txm_sandbox/napari_gui/utils/io.py
 txm_sandbox/napari_gui/utils/misc.py
 txm_sandbox/tmp/__init__.py
+txm_sandbox/tmp/readme.txt
 txm_sandbox/utils/__init__.py
 txm_sandbox/utils/io.py
 txm_sandbox/utils/lineshapes.py
 txm_sandbox/utils/misc.py
 txm_sandbox/utils/plotlib.py
 txm_sandbox/utils/reg_algs.py
 txm_sandbox/utils/tomo_recon_tools.py
```

