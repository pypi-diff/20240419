# Comparing `tmp/dash-connectivity-viewer-2.1.0.tar.gz` & `tmp/dash_connectivity_viewer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-connectivity-viewer-2.1.0.tar", last modified: Fri Aug 11 21:43:23 2023, max compression
+gzip compressed data, was "dash_connectivity_viewer-2.2.0.tar", last modified: Fri Apr 19 01:36:21 2024, max compression
```

## Comparing `dash-connectivity-viewer-2.1.0.tar` & `dash_connectivity_viewer-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.741717 dash-connectivity-viewer-2.1.0/
--rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash-connectivity-viewer-2.1.0/LICENSE.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-08-11 21:43:23.741527 dash-connectivity-viewer-2.1.0/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.731431 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/
--rw-r--r--   0 caseysm    (501) staff       (20)       22 2023-08-11 21:19:28.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/__init__.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.734666 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/
--rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    25450 2023-08-11 21:19:18.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6156 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    20408 2023-05-14 19:13:50.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/layout.py
--rw-r--r--   0 caseysm    (501) staff       (20)     4469 2023-05-24 07:29:35.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.735916 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14472 2023-05-14 19:13:28.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/ct_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14841 2023-05-14 19:13:16.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.739332 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/
--rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)     5233 2023-05-23 23:46:19.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/dash_url_helper.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.740165 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/data/
--rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/data/height_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
--rw-r--r--   0 caseysm    (501) staff       (20)    10305 2023-05-24 23:49:21.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/dataframe_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/external_stylesheets.py
--rw-r--r--   0 caseysm    (501) staff       (20)    13477 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/link_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3889 2023-05-24 20:55:11.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/lookup_utilities.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11744 2023-08-11 21:19:18.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/neuron_data_base.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3871 2023-05-24 20:54:59.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/schema_utils.py
--rw-r--r--   0 caseysm    (501) staff       (20)     3950 2023-05-24 16:16:13.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/table_lookup.py
--rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/transform_utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.741204 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/
--rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    14166 2023-08-11 21:19:18.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/callbacks.py
--rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/config.py
--rw-r--r--   0 caseysm    (501) staff       (20)     9093 2023-04-13 06:41:46.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/layout.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-08-11 21:43:23.732101 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)      525 2023-08-11 21:43:23.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)     1990 2023-08-11 21:43:23.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-08-11 21:43:23.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      180 2023-08-11 21:43:23.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       25 2023-08-11 21:43:23.000000 dash-connectivity-viewer-2.1.0/dash_connectivity_viewer.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)      179 2023-08-11 21:42:59.000000 dash-connectivity-viewer-2.1.0/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-08-11 21:43:23.741767 dash-connectivity-viewer-2.1.0/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash-connectivity-viewer-2.1.0/setup.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.221196 dash_connectivity_viewer-2.2.0/
+-rw-r--r--   0 caseysm    (501) staff       (20)     1842 2023-05-09 18:49:42.000000 dash_connectivity_viewer-2.2.0/LICENSE.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       71 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/MANIFEST.in
+-rw-r--r--   0 caseysm    (501) staff       (20)      928 2024-04-19 01:36:21.220889 dash_connectivity_viewer-2.2.0/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)      216 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/README.md
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.208639 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/
+-rw-r--r--   0 caseysm    (501) staff       (20)       22 2024-04-19 01:36:06.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/__init__.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.212270 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/
+-rw-r--r--   0 caseysm    (501) staff       (20)      568 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    28668 2024-04-18 20:23:56.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5453 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     3461 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6514 2024-04-16 04:45:20.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py
+-rw-r--r--   0 caseysm    (501) staff       (20)       82 2023-03-18 18:57:32.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    22319 2024-04-17 19:43:24.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/layout.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4469 2023-05-24 07:29:35.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.213693 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      711 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    16791 2024-04-18 20:56:02.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     1347 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      210 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/ct_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15463 2024-04-18 19:37:35.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.218172 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/
+-rw-r--r--   0 caseysm    (501) staff       (20)       17 2023-04-13 06:43:13.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     5357 2024-04-19 01:36:01.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     2914 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dash_url_helper.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.218747 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/data/
+-rw-r--r--   0 caseysm    (501) staff       (20)      144 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/data/height_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)      168 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/data/layer_bounds_v1.npy
+-rw-r--r--   0 caseysm    (501) staff       (20)    10434 2024-04-17 23:53:01.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dataframe_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      294 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/external_stylesheets.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    14029 2024-04-16 20:08:15.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/link_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     6041 2024-04-18 01:08:17.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/lookup_utilities.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    12472 2024-04-17 22:34:42.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/neuron_data_base.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4163 2024-04-18 22:28:25.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/schema_utils.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     4020 2024-04-18 20:36:47.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/table_lookup.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      762 2023-04-13 06:41:46.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/transform_utils.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.220101 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/
+-rw-r--r--   0 caseysm    (501) staff       (20)      591 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/__init__.py
+-rw-r--r--   0 caseysm    (501) staff       (20)    15965 2024-04-18 20:15:50.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/callbacks.py
+-rw-r--r--   0 caseysm    (501) staff       (20)      523 2023-02-08 23:15:09.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/config.py
+-rw-r--r--   0 caseysm    (501) staff       (20)     9905 2024-04-18 02:02:07.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/layout.py
+drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2024-04-19 01:36:21.220527 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/
+-rw-r--r--   0 caseysm    (501) staff       (20)      928 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 caseysm    (501) staff       (20)     1990 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)        1 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      178 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/requires.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       25 2024-04-19 01:36:21.000000 dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/top_level.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)      178 2024-04-16 00:28:06.000000 dash_connectivity_viewer-2.2.0/requirements.txt
+-rw-r--r--   0 caseysm    (501) staff       (20)       38 2024-04-19 01:36:21.221248 dash_connectivity_viewer-2.2.0/setup.cfg
+-rw-r--r--   0 caseysm    (501) staff       (20)     1153 2022-11-16 18:21:07.000000 dash_connectivity_viewer-2.2.0/setup.py
```

### Comparing `dash-connectivity-viewer-2.1.0/LICENSE.txt` & `dash_connectivity_viewer-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/callbacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import pytz
 import numpy as np
 from functools import partial
 
 from dash import dcc, html, callback_context
 from dash.dependencies import Input, Output, State
 
 from .config import TypedConnectivityConfig
@@ -12,23 +13,28 @@
     generate_statebuilder_post,
     generate_statebuider_syn_grouped,
     generate_statebuilder_syn_cell_types,
     EMPTY_INFO_CACHE,
     MAX_URL_LENGTH,
     make_url_robust,
     aligned_volume,
+    get_viewer_site_from_target,
 )
 from ..common.dash_url_helper import _COMPONENT_ID_TYPE
 from ..common.lookup_utilities import (
     get_type_tables,
     make_client,
+    get_version_options,
 )
 from ..common.schema_utils import get_table_info
 from ..common.dataframe_utilities import (
-    stringify_root_ids, stringify_list, rehydrate_dataframe, rebuild_synapse_dataframe
+    stringify_root_ids,
+    stringify_list,
+    rehydrate_dataframe,
+    rebuild_synapse_dataframe,
 )
 from .neuron_data_cortex import NeuronDataCortex as NeuronData
 from .neuron_data_cortex import ALLOW_COLUMN_TYPES_DISCRETE
 from .cortex_panels import *
 
 try:
     from loguru import logger
@@ -50,31 +56,42 @@
     "options",
 )
 OutputCellTypeValue = Output(
     {"id_inner": "cell-type-table-dropdown", "type": _COMPONENT_ID_TYPE},
     "value",
 )
 
+InputMaterializationVersion = Input(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
+)
+StateMaterializationVersion = State(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
+)
+OutputMaterializeOptions = Output(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "options"
+)
+OutputMaterializeValue = Output(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
+)
+
 StateAnnoType = State({"id_inner": "id-type", "type": _COMPONENT_ID_TYPE}, "value")
 StateLiveQuery = State(
     {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE}, "value"
 )
-StateLinkGroupValue = State('group-by', 'value')
+StateLinkGroupValue = State("group-by", "value")
 
 OutputLiveQueryToggle = Output(
     {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE},
     "options",
 )
 OutputLiveQueryValue = Output(
     {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE}, "value"
 )
 
 
-
-
 def allowed_action_trigger(ctx, allowed_buttons):
     if not ctx.triggered:
         return False
     trigger_src = ctx.triggered[0]["prop_id"].split(".")[0]
     return trigger_src in allowed_buttons
 
 
@@ -107,138 +124,184 @@
 
 def make_violin_plot(ndat, height=350):
     if ndat is None:
         return html.Div("")
 
     violin = violin_fig(ndat, height=height)
     contents = [
-        html.H5("Input/Output Depth", className='card-title'),
+        html.H5("Input/Output Depth", className="card-title"),
         dcc.Graph(
-            figure=violin, style={"margin-left": "5rem", "margin-right": "5rem", "width": "auto", "height": "25rem"}
+            figure=violin,
+            style={
+                "margin-left": "5rem",
+                "margin-right": "5rem",
+                "width": "auto",
+                "height": "25rem",
+            },
         ),
     ]
     return contents
 
 
-def make_ct_plots(rows, config, aligned_volume, color_column):
+def make_ct_plots(rows, config, aligned_volume, color_column, table_values):
     if rows is None:
         return html.Div(""), html.Div("")
     if len(rows) == 0:
         return html.Div(""), html.Div("")
 
     df = rebuild_synapse_dataframe(
         rows,
         config,
         aligned_volume,
         value_cols=[color_column],
     )
+    if color_column in table_values:
+        df[color_column] = df[color_column].astype(
+            pd.CategoricalDtype(
+                categories=sorted(table_values[color_column])
+                + [config.null_cell_type_label],
+                ordered=True,
+            )
+        )
 
     if color_column == "":
         color_column = None
 
     if config.show_depth_plots:
-        scatter_contents = make_scatter_div(df.copy(), config, color_column, width=450, height=350)
+        scatter_contents = make_scatter_div(
+            df.copy(), config, color_column, width=450, height=350
+        )
     else:
         scatter_contents = html.Div("")
-    bar_contents = make_bar_div(df.copy(), config, color_column, width = 450, height=350)
+    bar_contents = make_bar_div(df.copy(), config, color_column, width=450, height=350)
 
     return scatter_contents, bar_contents
 
 
 def make_scatter_div(
-    df, config, color_column, width=450, height=350,
+    df,
+    config,
+    color_column,
+    width=450,
+    height=350,
 ):
     scatter_fig = scatter_fig_df(df, config, color_column, width, height)
     contents = [
-        html.H5("Synapse/Target Soma Depth", className='card-title'),
+        html.H5("Synapse/Target Soma Depth", className="card-title"),
         dcc.Graph(
-            figure=scatter_fig, style={"height": "100%",  "width": "auto"},
+            figure=scatter_fig,
+            style={"height": "100%", "width": "auto"},
         ),
     ]
     return contents
 
+
 def make_bar_div(df, config, color_column, width=450, height=350):
     if color_column is None:
         contents = [
             html.H4(
                 "Select value column for bar chart",
-                style=
-                    {
-                        'text-align': 'center', 'vertical-align': 'middle'
-                    },
-                ),
+                style={"text-align": "center", "vertical-align": "middle"},
+            ),
         ]
     else:
         bar_fig = bar_fig_df(df, config, color_column)
         contents = [
-            html.H5("Target Distribution", style={'text-align': 'center'}),
-            dcc.Graph(
-                figure=bar_fig, style={"width": "auto", "height": "100%"}
-            )
+            html.H5("Target Distribution", style={"text-align": "center"}),
+            dcc.Graph(figure=bar_fig, style={"width": "auto", "height": "100%"}),
         ]
     return contents
 
-def register_callbacks(app, config):
 
+def register_callbacks(app, config):
     c = TypedConnectivityConfig(config)
 
     @app.callback(
         Output("data-table", "selected_rows"),
         Input("reset-selection", "n_clicks"),
         Input("connectivity-tab", "value"),
     )
     def reset_selection(n_clicks, tab_value):
         return []
 
     @app.callback(
-        Output("header-bar", 'children'),
+        Output("header-bar", "children"),
         InputDatastack,
     )
     def set_header(datastack):
-        return html.H3(f"Typed Connectivity Viewer — {datastack}", className="bg-primary text-white p-2 mb-2 text-center")
+        return html.H3(
+            f"Typed Connectivity Viewer — {datastack}",
+            className="bg-primary text-white p-2 mb-2 text-center",
+        )
 
+    @app.callback(
+        OutputMaterializeOptions,
+        OutputMaterializeValue,
+        InputDatastack,
+    )
+    def get_materialization_versions(
+        datastack_name,
+    ):
+        # Produce ordered list of materialization versions to choose from
+        client = make_client(datastack_name, c.server_address)
+        version_options, default_value = get_version_options(
+            client, c.disallow_live_query
+        )
+        return version_options, default_value
 
     @app.callback(
         Output("data-table", "columns"),
         Output("group-by", "options"),
+        Output("unique-table-values", "data"),
         Input("submit-button", "n_clicks"),
         InputDatastack,
         StateCellTypeTable,
     )
     def define_table_columns(_, datastack, cell_type_table):
         client = make_client(datastack, c.server_address)
 
         if cell_type_table == "" or cell_type_table is None:
-            return [{"name": i, "id": i} for i in c.table_columns], []
+            return [{"name": i, "id": i} for i in c.table_columns], [], {}
 
         if c.debug:
-            print('cell_type_table', cell_type_table, 'client', client.datastack_name)
-        _, val_cols = get_table_info(cell_type_table, client, allow_types=ALLOW_COLUMN_TYPES_DISCRETE)
+            print("cell_type_table", cell_type_table, "client", client.datastack_name)
+        _, val_cols = get_table_info(
+            cell_type_table, client, allow_types=ALLOW_COLUMN_TYPES_DISCRETE
+        )
 
         table_cons = c.table_columns + val_cols
+        table_values = client.materialize.get_unique_string_values(cell_type_table)
         return (
             [{"name": i, "id": i} for i in table_cons],
             [{"label": k, "value": k} for k in val_cols],
+            table_values,
         )
 
     @app.callback(
-        Output('plot-color-value', 'options'),
-        Output('plot-color-value', 'value'),
-        Input('group-by', 'options'),
-        Input('plot-color-value', 'value'),
+        OutputCellTypeValue,
+        InputMaterializationVersion,
+    )
+    def clear_cell_type_dropdown(mat_version):
+        return ""
+
+    @app.callback(
+        Output("plot-color-value", "options"),
+        Output("plot-color-value", "value"),
+        Input("group-by", "options"),
+        Input("plot-color-value", "value"),
     )
     def update_plot_options(new_options, old_value):
-        DEFAULT_VALUE = 'cell_type'
-        option_labels = [v['label'] for v in new_options]
+        DEFAULT_VALUE = "cell_type"
+        option_labels = [v["label"] for v in new_options]
         if old_value in option_labels:
             new_value = old_value
         elif DEFAULT_VALUE in new_options:
             new_value = DEFAULT_VALUE
         else:
-            new_value = ''
+            new_value = ""
         return new_options, new_value
 
     @app.callback(
         OutputDatastack,
         InputDatastack,
     )
     def define_datastack(datastack):
@@ -247,44 +310,23 @@
 
         if len(datastack) == 0:
             return c.default_datastack
         else:
             return datastack
 
     @app.callback(
-        OutputLiveQueryToggle,
-        OutputLiveQueryValue,
-        InputDatastack,
-        StateLiveQuery,
-    )
-    def disable_live_query(_, lq):
-        options_active = [{"label": "Live Query", "value": 1}]
-        options_disabled = [{"label": "Live Query", "value": 1, "disabled": True}]
-        if c.disallow_live_query:
-            return options_disabled, ""
-        else:
-            return options_active, lq
-
-    @app.callback(
         OutputCellTypeMenuOptions,
         InputDatastack,
+        InputMaterializationVersion,
     )
-    def set_cell_type_dropdown(datastack):
-        return get_type_tables(datastack, c)
-
-    @app.callback(
-        OutputCellTypeValue,
-        InputDatastack,
-        StateCellTypeTable,
-    )
-    def default_cell_type_option(_, curr_value):
-        if curr_value != "":
-            return curr_value
-        else:
-            return c.default_cell_type_option
+    def set_cell_type_dropdown(datastack, mat_version):
+        if c.debug:
+            print("Triggered cell type dropdown options")
+        type_tables = get_type_tables(datastack, c, mat_version)
+        return type_tables
 
     @app.callback(
         Output("message-text", "children"),
         Output("message-text", "color"),
         Output("main-loading-placeholder", "children"),
         Output("target-table-json", "data"),
         Output("source-table-json", "data"),
@@ -295,24 +337,36 @@
         Output("violin-plot", "children"),
         Output("synapse-table-resolution-json", "data"),
         Input("submit-button", "n_clicks"),
         InputDatastack,
         StateRootID,
         StateAnnoType,
         StateCellTypeTable,
-        StateLiveQuery,
+        StateMaterializationVersion,
     )
-    def update_data(_1, datastack_name, anno_id, id_type, ct_table_value, query_toggle):
+    def update_data(_1, datastack_name, anno_id, id_type, ct_table_value, mat_version):
         if logger is not None:
             t0 = time.time()
+        if c.debug:
+            print("Mat version:", mat_version)
+
+        if mat_version == "live" or "":
+            version = None
+        else:
+            version = mat_version
 
         try:
-            client = make_client(datastack_name, c.server_address)
+            client = make_client(
+                datastack_name, c.server_address, materialize_version=version
+            )
+            if version is None:
+                version = client.materialize.version
             info_cache = client.info.info_cache[datastack_name]
             info_cache["global_server"] = client.server_address
+
         except Exception as e:
             return (
                 html.Div(str(e)),
                 "danger",
                 "",
                 [],
                 [],
@@ -324,91 +378,92 @@
                 None,
             )
 
         if not ct_table_value:
             ct_table_value = None
         info_cache["cell_type_column"] = ct_table_value
 
-        if len(query_toggle) == 1 and not c.disallow_live_query:
+        if mat_version == "live":
             live_query = True
         else:
             live_query = False
 
         if live_query:
-            timestamp = datetime.datetime.utcnow()
+            timestamp = datetime.datetime.now(tz=pytz.UTC)
             timestamp_ngl = None
-            info_cache['ngl_timestamp'] = None
+            info_cache["ngl_timestamp"] = None
         else:
-            timestamp = client.materialize.get_timestamp()
+            timestamp = client.materialize.get_timestamp(version=version)
             timestamp_ngl = timestamp
             info_cache["ngl_timestamp"] = timestamp.timestamp()
 
         if anno_id is None or len(anno_id) == 0:
             return (
                 html.Div("Please select a cell id and press Submit"),
                 "info",
                 "",
                 [],
                 [],
                 "Output",
                 "Input",
                 1,
-                EMPTY_INFO_CACHE,
+                info_cache,
                 make_violin_plot(None),
                 None,
             )
         else:
             if id_type == "root_id":
                 object_id = int(anno_id)
                 object_id_type = "root"
             elif id_type == "nucleus_id":
                 object_id = int(anno_id)
                 object_id_type = "nucleus"
             else:
                 raise ValueError('id_type must be either "root_id" or "nucleus_id"')
-        
+
         try:
             nrn_data = NeuronData(
                 object_id=object_id,
                 client=client,
                 config=c,
                 value_table=ct_table_value,
                 timestamp=timestamp,
                 id_type=object_id_type,
                 is_live=live_query,
                 n_threads=2,
             )
             if c.debug:
-                print(f'\nMade NeuronData object with nuc table: {nrn_data._soma_table}\n')
+                print(
+                    f"\nMade NeuronData object with nuc table: {nrn_data._soma_table}\n"
+                )
 
             root_id = nrn_data.root_id
             info_cache["root_id"] = str(root_id)
 
             if c.debug:
-                print(f'\n Starting partners out')
+                print(f"\n Starting partners out")
             pre_targ_df = nrn_data.partners_out_plus()
             pre_targ_df = stringify_root_ids(
                 pre_targ_df, stringify_cols=[c.root_id_col]
             )
 
             if c.debug:
-                print(f'\n Starting partners in')
+                print(f"\n Starting partners in")
             post_targ_df = nrn_data.partners_in_plus()
             post_targ_df = stringify_root_ids(
                 post_targ_df, stringify_cols=[c.root_id_col]
             )
 
             n_syn_pre = pre_targ_df[c.num_syn_col].sum()
             n_syn_post = post_targ_df[c.num_syn_col].sum()
 
             for col in nrn_data.config.syn_pt_position_split:
                 stringify_list(col, pre_targ_df)
                 stringify_list(col, post_targ_df)
 
-
             if logger is not None:
                 logger.info(
                     f"Data update for {root_id} | time:{time.time() - t0:.2f} s, syn_in: {len(pre_targ_df)} , syn_out: {len(post_targ_df)}"
                 )
             if nrn_data.nucleus_id is not None and nrn_data.soma_table is not None:
                 if np.issubdtype(type(nrn_data.nucleus_id), np.integer):
                     nuc_id_text = f"  (nucleus id: {nrn_data.nucleus_id})"
@@ -419,18 +474,18 @@
             if ct_table_value:
                 ct_text = f"table {ct_table_value}"
             else:
                 ct_text = "no cell type table"
 
             if nrn_data.old_root_id is not None:
                 change_root_id_text = f" Warning: {nrn_data.old_root_id} is not valid at timestamp queried! Showing data for the most overlapping valid root id. — "
-                output_status='warning'
+                output_status = "warning"
             else:
                 change_root_id_text = ""
-                output_status='success'
+                output_status = "success"
 
             if live_query:
                 message_text = f"{change_root_id_text}Current connectivity for root id {root_id}{nuc_id_text} and {ct_text}."
             else:
                 message_text = f"{change_root_id_text}Connectivity for root id {root_id}{nuc_id_text} and {ct_text} materialized on {timestamp_ngl:%m/%d/%Y} (v{client.materialize.version})"
 
             if c.show_depth_plots:
@@ -454,17 +509,17 @@
                 vplot,
                 syn_res,
             )
         except Exception as e:
             if c.debug:
                 print(f"Failed on datastack {datastack_name}!")
                 print(
-                    '\n',
+                    "\n",
                     info_cache,
-                    '\n',
+                    "\n",
                 )
             return (
                 html.Div(str(e)),
                 "danger",
                 "",
                 [],
                 [],
@@ -473,26 +528,24 @@
                 1,
                 EMPTY_INFO_CACHE,
                 make_violin_plot(None),
                 None,
             )
 
     @app.callback(
-        Output('scatter-plot', 'children'),
-        Output('bar-plot', 'children'),
+        Output("scatter-plot", "children"),
+        Output("bar-plot", "children"),
         Input("target-table-json", "data"),
-        Input("plot-color-value", 'value'),
+        Input("plot-color-value", "value"),
         Input("client-info-json", "data"),
+        Input("unique-table-values", "data"),
     )
-    def update_scatter_bar_plots(rows, color_column, info_cache):
+    def update_scatter_bar_plots(rows, color_column, info_cache, table_values):
         return make_ct_plots(
-            rows,
-            c,
-            aligned_volume(info_cache),
-            color_column,
+            rows, c, aligned_volume(info_cache), color_column, table_values
         )
 
     @app.callback(
         Output("data-table", "data"),
         Input("connectivity-tab", "value"),
         Input("target-table-json", "data"),
         Input("source-table-json", "data"),
@@ -515,32 +568,46 @@
         Output("ngl-link", "disabled"),
         Output("link-loading", "children"),
         Input("connectivity-tab", "value"),
         Input("data-table", "derived_virtual_data"),
         Input("data-table", "derived_virtual_selected_rows"),
         Input("client-info-json", "data"),
         Input("synapse-table-resolution-json", "data"),
+        Input("ngl-target-site", "value"),
+        InputDatastack,
     )
     def update_link(
         tab_value,
         rows,
         selected_rows,
         info_cache,
         synapse_data_resolution,
+        target_site,
+        datastack_name,
     ):
+        if c.debug:
+            print(f"Target site: {target_site}")
         large_state_text = (
             "Table Too Large - Please Filter or Use Whole Cell Neuroglancer Links"
         )
 
         def small_state_text(n):
             return f"Neuroglancer: ({n} partners)"
 
         if info_cache is None:
-            return "", "No datastack set", True, ""
+            client = make_client(datastack_name, c.server_address)
+            info_cache = client.info.info_cache[datastack_name]
 
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+        if c.debug:
+            print("generating link")
+            print(info_cache)
         if rows is None or len(rows) == 0:
             rows = {}
             sb = generate_statebuilder(info_cache, c)
             return (
                 sb.render_state(None, return_as="url"),
                 small_state_text(0),
                 False,
@@ -598,19 +665,32 @@
         Input("all-input-link-button", "n_clicks"),
         Input("all-input-link-button", "children"),
         Input("submit-button", "n_clicks"),
         Input("source-table-json", "data"),
         Input("client-info-json", "data"),
         InputDatastack,
         Input("synapse-table-resolution-json", "data"),
+        Input("ngl-target-site", "value"),
         prevent_initial_call=True,
     )
     def generate_all_input_link(
-        _1, _2, curr, rows, info_cache, datastack, data_resolution
+        _1,
+        _2,
+        curr,
+        rows,
+        info_cache,
+        datastack,
+        data_resolution,
+        target_site,
     ):
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if not allowed_action_trigger(callback_context, ["all-input-link-button"]):
             return "  ", "Generate Link", False
         return (
             generic_syn_link_generation(
                 partial(
                     generate_statebuilder_post,
                     config=c,
@@ -633,21 +713,35 @@
         Output("cell-typed-input-link-button", "disabled"),
         Input("cell-typed-input-link-button", "n_clicks"),
         Input("submit-button", "n_clicks"),
         Input("source-table-json", "data"),
         Input("client-info-json", "data"),
         InputDatastack,
         Input("synapse-table-resolution-json", "data"),
-        Input('group-by', 'value'),
-        Input('no-type-annotation', 'value'),
+        Input("group-by", "value"),
+        Input("no-type-annotation", "value"),
+        Input("ngl-target-site", "value"),
         prevent_initial_call=True,
     )
     def generate_cell_typed_input_link(
-        _1, _2, rows, info_cache, datastack, data_resolution, value_column, include_no_type,
+        _1,
+        _2,
+        rows,
+        info_cache,
+        datastack,
+        data_resolution,
+        value_column,
+        include_no_type,
+        target_site,
     ):
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if value_column is None or value_column == "":
             return "  ", "No Annotation Column Set", True
         if not allowed_action_trigger(
             callback_context, ["cell-typed-input-link-button"]
         ):
             return "  ", "Generate Link", False
 
@@ -684,17 +778,25 @@
         Output("all-output-link-button", "disabled"),
         Input("all-output-link-button", "n_clicks"),
         Input("submit-button", "n_clicks"),
         Input("target-table-json", "data"),
         Input("client-info-json", "data"),
         InputDatastack,
         Input("synapse-table-resolution-json", "data"),
+        Input("ngl-target-site", "value"),
         prevent_initial_call=True,
     )
-    def generate_all_output_link(_1, _2, rows, info_cache, datastack, data_resolution):
+    def generate_all_output_link(
+        _1, _2, rows, info_cache, datastack, data_resolution, target_site
+    ):
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if not allowed_action_trigger(callback_context, ["all-output-link-button"]):
             return "", "Generate Link", False
         return (
             generic_syn_link_generation(
                 partial(
                     generate_statebuilder_pre, config=c, data_resolution=data_resolution
                 ),
@@ -715,24 +817,38 @@
         Output("cell-typed-output-link-button", "disabled"),
         Input("cell-typed-output-link-button", "n_clicks"),
         Input("submit-button", "n_clicks"),
         Input("target-table-json", "data"),
         Input("client-info-json", "data"),
         InputDatastack,
         Input("synapse-table-resolution-json", "data"),
-        Input('group-by', 'value'),
-        Input('no-type-annotation', 'value'),
+        Input("group-by", "value"),
+        Input("no-type-annotation", "value"),
+        Input("ngl-target-site", "value"),
         prevent_initial_call=True,
     )
     def generate_cell_typed_output_link(
-        _1, _2, rows, info_cache, datastack, data_resolution, value_column, include_no_type,
+        _1,
+        _2,
+        rows,
+        info_cache,
+        datastack,
+        data_resolution,
+        value_column,
+        include_no_type,
+        target_site,
     ):
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if value_column is None or value_column == "":
             return "  ", "No Annotation Column Set", True
-        
+
         if not allowed_action_trigger(
             callback_context, ["cell-typed-output-link-button"]
         ):
             return "  ", "Generate Link", False
 
         include_no_type = 1 in include_no_type
 
@@ -777,8 +893,8 @@
         State("plot-collapse", "is_open"),
     )
     def toggle_plot_collapse(n, is_open):
         if n:
             return not is_open
         return is_open
 
-    pass
+    pass
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/config.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_panels.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/cortex_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from plotly import colors
 import plotly.graph_objects as go
 import numpy as np
 import pandas as pd
 
+
 def _violin_plot(syn_df, x_col, y_col, name, side, color, xaxis, yaxis):
     return go.Violin(
         x=syn_df[x_col],
         y=syn_df[y_col],
         side=side,
         scalegroup="syn",
-        spanmode='hard',
+        spanmode="hard",
         name=name,
         points=False,
         line_color=f"rgb{color}",
         fillcolor=f"rgb{color}",
         xaxis=xaxis,
         yaxis=yaxis,
-        hoverinfo='text',
+        hoverinfo="text",
         hovertext=f"{len(syn_df)} Syn.",
         # bandwidth=0.2,
     )
 
 
 def post_violin_plot(
     ndat,
@@ -51,58 +52,70 @@
         name="Pre",
         side="positive",
         color=ndat.config.vis.axon_color,
         xaxis=xaxis,
         yaxis=yaxis,
     )
 
+
 from itertools import cycle
+
+
 def _colorscheme(n):
     if n <= 10:
         clrs = cycle(colors.qualitative.G10)
     else:
         clrs = cycle(colors.qualitative.Dark24)
     return [next(clrs) for i in range(n)]
 
+
 def synapse_soma_scatterplot(
     targ_df,
     config,
     color_column,
     xaxis=None,
     yaxis=None,
 ):
-
     if color_column is None or color_column == "":
-        fake_cell_type_column = 'DummyColumn_'
+        fake_cell_type_column = "DummyColumn_"
         while fake_cell_type_column in targ_df.columns:
-            fake_cell_type_column += 'a'
+            fake_cell_type_column += "a"
         color_column = fake_cell_type_column
         targ_df[color_column] = config.null_cell_type_label
         ctypes = [config.null_cell_type_label]
     else:
-        if targ_df[color_column].dtype == 'float64':
+        if targ_df[color_column].dtype == "float64":
             targ_df[color_column] = targ_df[color_column].astype(pd.Int64Dtype())
             ctypes = sorted(list(np.unique(targ_df[color_column].dropna()).astype(str)))
-            targ_df[color_column] = targ_df[color_column].astype(str).replace(
-                {'<NA>': config.null_cell_type_label}
+            targ_df[color_column] = (
+                targ_df[color_column]
+                .astype(str)
+                .replace({"<NA>": config.null_cell_type_label})
             )
         else:
-            ctypes = sorted(list(np.unique(targ_df[color_column].dropna()).astype(str)))
-            targ_df[color_column] = targ_df[color_column].fillna(config.null_cell_type_label).astype(str)
-        ctypes = ctypes+[config.null_cell_type_label]
-
-    
-    if len(ctypes)>1:
-        cmap = _colorscheme(len(ctypes)-1) + ['#333333']
+            try:
+                ctypes = targ_df[color_column].dtype.categories
+                print("from category")
+            except:
+                ctypes = sorted(
+                    list(np.unique(targ_df[color_column].dropna()).astype(str))
+                )
+                print("from values")
+            print(ctypes)
+            targ_df[color_column] = (
+                targ_df[color_column].fillna(config.null_cell_type_label).astype(str)
+            )
+    if len(ctypes) > 1:
+        cmap = _colorscheme(len(ctypes) - 1) + ["#333333"]
     else:
-        cmap = ['#333333']
+        cmap = ["#333333"]
 
     alpha_default = {config.null_cell_type_label: 0.2}
     panels = []
-    alpha= config.vis.e_opacity
+    alpha = config.vis.e_opacity
     for ct, clr in zip(ctypes, cmap):
         targ_df_r = targ_df.query(f"{color_column}=='{ct}'")
         panel = go.Scattergl(
             x=targ_df_r[config.soma_depth_column],
             y=targ_df_r[config.synapse_depth_column],
             mode="markers",
             marker=dict(
@@ -116,22 +129,28 @@
             name=ct,
             # hoverinfo='none',
         )
         panels.append(panel)
 
     return panels
 
+
 def bar_plot_df(
     targ_df,
     config,
     color_value,
 ):
+    targ_df = targ_df.replace({config.null_cell_type_label: None}).dropna(
+        subset=color_value
+    )
 
-    targ_df = targ_df.replace({config.null_cell_type_label: None}).dropna(subset=color_value)
-    xtypes = sorted(list(np.unique(targ_df[color_value])))
+    try:
+        xtypes = targ_df[color_value].dtype.categories
+    except:
+        xtypes = sorted(list(np.unique(targ_df[color_value])))
     clrs = _colorscheme(len(xtypes))
     cnts = targ_df.value_counts(color_value).loc[xtypes]
 
     bar = go.Bar(
         name=color_value,
         x=xtypes,
         y=cnts,
@@ -238,8 +257,8 @@
 def uniform_bar_plot(
     ndat,
     cell_type_column,
     cell_types=None,
 ):
     return _prepare_bar_plot(
         ndat, cell_type_column, ndat.config.vis.u_color, cell_types, "u"
-    )
+    )
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/layout.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/layout.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,34 +51,48 @@
                             ),
                         ],
                         width={"size": 1},
                         align="end",
                     ),
                     dbc.Col(
                         [
-                            dbc.Checklist(
+                            "Materialization:",
+                            dcc.Dropdown(
                                 **create_component_kwargs(
                                     state,
-                                    id_inner="live-query-toggle",
-                                    options=[
-                                        {
-                                            "label": "Live Query",
-                                            "value": 1,
-                                        },
-                                    ],
-                                    value=[
-                                        1,
-                                    ],
-                                    switch=True,
+                                    id_inner="mat-version",
+                                    options=[{"label": "Latest", "value": ""}],
+                                    value="",
                                     style={
-                                        "bottom-margin": "10px",
-                                        "font-size": "16px",
+                                        "margin-left": "12px",
+                                        "font-size": "12px",
                                     },
+                                    clearable=False,
                                 )
                             ),
+                            # dbc.Checklist(
+                            #     **create_component_kwargs(
+                            #         state,
+                            #         id_inner="live-query-toggle",
+                            #         options=[
+                            #             {
+                            #                 "label": "Live Query",
+                            #                 "value": 1,
+                            #             },
+                            #         ],
+                            #         value=[
+                            #             1,
+                            #         ],
+                            #         switch=True,
+                            #         style={
+                            #             "bottom-margin": "10px",
+                            #             "font-size": "16px",
+                            #         },
+                            #     )
+                            # ),
                         ],
                         width={"size": 1, "offset": 1},
                         align="center",
                     ),
                     dbc.Col(
                         dbc.Button(
                             children="Submit",
@@ -174,22 +188,40 @@
                     children="Reset Selection",
                     color="warning",
                     size="sm",
                 ),
                 width=1,
             ),
             dbc.Col(
+                html.Div(
+                    [
+                        dcc.Dropdown(
+                            options={
+                                "seunglab": "Seung-lab Neuroglancer (classic)",
+                                "mainline": "Spelunker (experimental)",
+                            },
+                            value="seunglab",
+                            id="ngl-target-site",
+                            clearable=False,
+                        ),
+                    ],
+                    style={"font-size": "13px"},
+                ),
+                align="top",
+                width={"size": 2, "offset": 1},
+            ),
+            dbc.Col(
                 html.A(
                     "Instructions for filtering the table",
                     href="https://dash.plotly.com/datatable/filtering",
                     style={"font-size": "15px"},
                     target="_blank",
                 ),
                 align="center",
-                width={"size": 2, "offset": 3},
+                width={"size": 2, "offset": 2},
             ),
         ],
         justify="start",
     )
 
 
 def make_data_table_content():
@@ -232,36 +264,38 @@
                     width=10,
                 ),
             ],
             justify="center",
         )
     )
 
+
 def make_input_link_tab():
     return [
         dbc.Card(
             [
                 dbc.CardBody(
                     [
                         html.H4("All Inputs", className="card-title"),
                         html.Div(
                             children=[
                                 dbc.Button(
                                     "Generate Link",
                                     id="all-input-link-button",
                                     color="secondary",
                                     className="d-grid gap-2 col-6 mx-auto",
-                                    style={"align-items":"center", "justify-content":"center"}
+                                    style={
+                                        "align-items": "center",
+                                        "justify-content": "center",
+                                    },
                                 ),
                             ]
                         ),
                         dbc.Spinner(
-                            html.Div(
-                                "", id="all-input-link", className="card-text"
-                            ),
+                            html.Div("", id="all-input-link", className="card-text"),
                             size="sm",
                         ),
                     ]
                 )
             ]
         ),
         dbc.Col(
@@ -291,36 +325,38 @@
                         ]
                     )
                 ]
             ),
         ),
     ]
 
+
 def make_output_link_tab():
     return [
         dbc.Card(
             [
                 dbc.CardBody(
                     [
                         html.H4("All Outputs", className="card-title"),
                         html.Div(
                             children=[
                                 dbc.Button(
                                     "Generate Link",
                                     id="all-output-link-button",
                                     color="secondary",
                                     className="d-grid gap-2 col-6 mx-auto",
-                                    style={"align-items":"center", "justify-content":"center"},
+                                    style={
+                                        "align-items": "center",
+                                        "justify-content": "center",
+                                    },
                                 ),
                             ]
                         ),
                         dbc.Spinner(
-                            html.Div(
-                                "", id="all-output-link", className="card-text"
-                            ),
+                            html.Div("", id="all-output-link", className="card-text"),
                             size="sm",
                         ),
                     ]
                 )
             ],
             style={"width": "18rem"},
         ),
@@ -349,21 +385,22 @@
                         ),
                     ]
                 )
             ]
         ),
     ]
 
+
 def page_layout(state: State = None):
     state = state or {}
 
     header_text = dbc.Row(
         [
             dbc.Col(
-                html.Div(id='header-bar'),
+                html.Div(id="header-bar"),
                 width={"size": 12},
             ),
         ],
     )
     input_row = make_input_row(state)
     message_row = make_message_row(state)
     top_link = make_table_link_row(state)
@@ -377,15 +414,14 @@
                     dcc.Tab(id="output-tab", label="Output", value="tab-pre"),
                 ],
             ),
             make_data_table_content(),
         ]
     )
 
-
     input_tab = make_input_link_tab()
     output_tab = make_output_link_tab()
 
     cell_links = [
         dbc.Row(
             [
                 dbc.Col(
@@ -415,27 +451,27 @@
                                                         "label": "Include No Type",
                                                         "value": 1,
                                                     },
                                                 ],
                                                 value=[],
                                                 switch=True,
                                                 style={"font-size": "16px"},
-                                                id='no-type-annotation',
+                                                id="no-type-annotation",
                                             ),
                                         ],
                                         width={"size": 2},
                                     ),
                                     dbc.Col(
                                         dcc.Dropdown(
                                             options={},
                                             value="",
                                             id="group-by",
                                             searchable=True,
                                         ),
-                                        width={'size': 8},
+                                        width={"size": 8},
                                     ),
                                 ],
                             ),
                         ]
                     )
                 ),
                 width={"size": 10, "offset": 1},
@@ -456,24 +492,32 @@
                                         id="violin-plot",
                                         className="text-center v-100 h-100",
                                     ),
                                 )
                             ),
                             dbc.Card(
                                 dbc.CardBody(
-                                    html.Div("", id="scatter-plot", className="text-center h-100 v-100"),
+                                    html.Div(
+                                        "",
+                                        id="scatter-plot",
+                                        className="text-center h-100 v-100",
+                                    ),
                                 )
                             ),
                             dbc.Card(
                                 dbc.CardBody(
-                                    html.Div("", id="bar-plot", className="text-center v-100 h-100"),
+                                    html.Div(
+                                        "",
+                                        id="bar-plot",
+                                        className="text-center v-100 h-100",
+                                    ),
                                 )
                             ),
                         ],
-                    className="h-100",
+                        className="h-100",
                     ),
                 )
             ],
         ),
         dbc.Row(
             dbc.Col(
                 dbc.Card(
@@ -481,28 +525,28 @@
                         [
                             dbc.Row(
                                 [
                                     dbc.Col(
                                         [
                                             html.Div(
                                                 "Color by value:",
-                                                style={'align-content': 'right'},
+                                                style={"align-content": "right"},
                                             ),
                                         ],
-                                        style={'align-content': 'right'},
-                                        width={"size": 1, 'offset':1},
+                                        style={"align-content": "right"},
+                                        width={"size": 1, "offset": 1},
                                     ),
                                     dbc.Col(
                                         dcc.Dropdown(
                                             options={"cell_type": "cell_type"},
                                             value="cell_type",
                                             id="plot-color-value",
-                                        ),  
+                                        ),
                                         style={"align-content": "left"},
-                                        width={'size': 9},
+                                        width={"size": 9},
                                     ),
                                 ],
                             ),
                         ]
                     )
                 ),
                 # width={"size": 12},
@@ -513,18 +557,18 @@
     main_tab = dbc.Row(
         [
             dbc.Col(
                 dbc.Tabs(
                     [
                         dbc.Tab(html.Div(), label="Table Only"),
                         dbc.Tab(plot_data, label="Plots"),
-                        dbc.Tab(cell_links, label="Neuroglancer Links")
+                        dbc.Tab(cell_links, label="Neuroglancer Links"),
                     ],
                 ),
-                width={'size': 10, 'offset': 1},
+                width={"size": 10, "offset": 1},
             )
         ]
     )
 
     layout = html.Div(
         children=[
             header_text,
@@ -540,14 +584,15 @@
             top_link,
             data_table,
             dcc.Store("target-table-json"),
             dcc.Store("source-table-json"),
             dcc.Store("client-info-json"),
             dcc.Store("synapse-table-resolution-json"),
             dcc.Store("value-columns"),
+            dcc.Store("unique-table-values"),
             html.Div(
                 dcc.Input(
                     **create_component_kwargs(
                         state,
                         id_inner="datastack",
                         value="",
                     ),
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_connectivity/neuron_data_cortex.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/__init__.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/callbacks.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/callbacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import flask
 import datetime
 from dash import callback_context
 from dash import dcc
 from dash import html
+import pytz
+import pandas as pd
 from .config import CellTypeConfig, RegisterTable
 
 from dash.dependencies import Input, Output, State
 from ..common.dataframe_utilities import *
 from ..common.link_utilities import (
     DEFAULT_NGL,
     generate_statebuilder,
     generate_url_cell_types,
     EMPTY_INFO_CACHE,
     MAX_URL_LENGTH,
+    get_viewer_site_from_target,
 )
 from ..common.lookup_utilities import (
     get_type_tables,
     make_client,
+    get_version_options,
 )
 from ..common.schema_utils import get_table_info
 from ..common.table_lookup import TableViewer
 
 # Callbacks using data from URL-encoded parameters requires this import
 from ..common.dash_url_helper import _COMPONENT_ID_TYPE
 
@@ -35,31 +39,39 @@
 )
 StateCellTypeMenu = State(
     {"id_inner": "cell-type-table-menu", "type": _COMPONENT_ID_TYPE}, "value"
 )
 StateCellType = State({"id_inner": "cell-type", "type": _COMPONENT_ID_TYPE}, "value")
 StateAnnoID = State({"id_inner": "anno-id", "type": _COMPONENT_ID_TYPE}, "value")
 StateCategoryID = State({"id_inner": "id-type", "type": _COMPONENT_ID_TYPE}, "value")
-StateLiveQuery = State(
-    {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE}, "value"
-)
 StateValueSearch = State(
     {"id_inner": "value-column-search", "type": _COMPONENT_ID_TYPE}, "value"
 )
 
-OutputLiveQueryToggle = Output(
-    {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE},
-    "options",
-)
-OutputLiveQueryValue = Output(
-    {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE}, "value"
-)
 OutputValueSearch = Output(
     {"id_inner": "value-column-search", "type": _COMPONENT_ID_TYPE}, "options"
 )
+OutputCellTypeValue = Output(
+    {"id_inner": "cell-type-table-menu", "type": _COMPONENT_ID_TYPE},
+    "value",
+)
+
+InputMaterializationVersion = Input(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
+)
+StateMaterializationVersion = State(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
+)
+OutputMaterializeOptions = Output(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "options"
+)
+OutputMaterializeValue = Output(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
+)
+
 
 ######################################
 # register_callbacks must be defined #
 ######################################
 
 
 def register_callbacks(app, config):
@@ -88,78 +100,111 @@
 
         if len(datastack) == 0:
             return c.default_datastack
         else:
             return datastack
 
     @app.callback(
-        Output("header-bar", 'children'),
+        Output("header-bar", "children"),
         InputDatastack,
     )
     def set_header(datastack):
-        return html.H3(f"Table Info — {datastack}", className="bg-primary text-white p-2 mb-2 text-center")
+        return html.H3(
+            f"Table Info — {datastack}",
+            className="bg-primary text-white p-2 mb-2 text-center",
+        )
 
     @app.callback(
-        OutputCellTypeMenuOptions,
-        InputDatastack,
+        OutputCellTypeValue,
+        InputMaterializationVersion,
     )
-    def cell_type_dropdown(datastack):
-        return get_type_tables(datastack, c)
+    def clear_cell_type_dropdown(mat_version):
+        return ""
 
     @app.callback(
-        OutputLiveQueryToggle,
-        OutputLiveQueryValue,
+        OutputCellTypeMenuOptions,
         InputDatastack,
-        StateLiveQuery,
+        InputMaterializationVersion,
     )
-    def disable_live_query(_, lq):
-        options_active = [{"label": "Live Query", "value": 1}]
-        options_disabled = [{"label": "Live Query", "value": 1, "disabled": True}]
-        if c.disallow_live_query:
-            return options_disabled, ""
-        else:
-            return options_active, lq
+    def cell_type_dropdown(datastack, mat_version):
+        if c.debug:
+            print("triggered new options")
+        return get_type_tables(datastack, c, mat_version)
 
     @app.callback(
         OutputValueSearch,
         InputDatastack,
         InputCellTypeMenu,
+        StateMaterializationVersion,
     )
-    def update_value_search_list(datastack, table_name):
-        if table_name is None:
+    def update_value_search_list(datastack, table_name, mat_version):
+        if table_name is None or table_name == "":
             return []
-        client = make_client(datastack, c.server_address)
+        if mat_version == "live" or mat_version == "":
+            version = None
+        else:
+            version = mat_version
+        client = make_client(datastack, c.server_address, materialize_version=version)
         _, cols = get_table_info(table_name, client, merge_schema=False)
         return [{"label": i, "value": i} for i in cols]
 
+    @app.callback(
+        OutputMaterializeOptions,
+        OutputMaterializeValue,
+        InputDatastack,
+    )
+    def get_materialization_versions(
+        datastack_name,
+    ):
+        # Produce ordered list of materialization versions to choose from
+        client = make_client(datastack_name, c.server_address)
+        version_options, default_value = get_version_options(
+            client, c.disallow_live_query
+        )
+        return version_options, default_value
 
     @app.callback(
         Output("group-by", "options"),
         Input("submit-button", "n_clicks"),
         StateCellTypeMenu,
         InputDatastack,
+        StateMaterializationVersion,
     )
-    def update_groupby_list(_, cell_type_table, datastack):
+    def update_groupby_list(_, cell_type_table, datastack, mat_version):
         if cell_type_table == "" or cell_type_table is None:
             return {}
         else:
-            client = make_client(datastack, c.server_address)
-            _, cols = get_table_info(cell_type_table, client, allow_types=['boolean', 'integer', 'string'])
+            if mat_version == "live" or mat_version == "":
+                version = None
+            else:
+                version = mat_version
+            client = make_client(
+                datastack, c.server_address, materialize_version=version
+            )
+
+            _, cols = get_table_info(
+                cell_type_table, client, allow_types=["boolean", "integer", "string"]
+            )
             return {k: k for k in cols}
 
     @app.callback(
         Output("data-table", "columns"),
         Output("pt-column", "data"),
         Output("value-columns", "data"),
         Input("submit-button", "n_clicks"),
         InputDatastack,
         StateCellTypeMenu,
+        StateMaterializationVersion,
     )
-    def define_table_columns(_, datastack, cell_type_table):
-        client = make_client(datastack, c.server_address)
+    def define_table_columns(_, datastack, cell_type_table, mat_version):
+        if mat_version == "live" or mat_version == "":
+            version = None
+        else:
+            version = mat_version
+        client = make_client(datastack, c.server_address, materialize_version=version)
         pt, cols = get_table_info(cell_type_table, client)
         reg_con = RegisterTable(pt, cols, c)
         return (
             [{"name": i, "id": i} for i in reg_con.ct_table_columns],
             pt,
             cols,
         )
@@ -173,61 +218,73 @@
         Output("data-resolution-json", "data"),
         Input("submit-button", "n_clicks"),
         InputDatastack,
         StateCellTypeMenu,
         StateAnnoID,
         StateCategoryID,
         StateCellType,
-        StateLiveQuery,
         StateValueSearch,
+        StateMaterializationVersion,
     )
     def update_table(
         clicks,
         datastack,
         cell_type_table,
         anno_id,
         id_type,
         value_search,
-        live_query_toggle,
         value_search_field,
+        mat_version,
     ):
+        if mat_version == "live" or mat_version == "":
+            version = None
+        else:
+            version = mat_version
+
         try:
-            client = make_client(datastack, c.server_address)
+            client = make_client(
+                datastack, c.server_address, materialize_version=version
+            )
+            if version is None:
+                version = client.materialize.version
             info_cache = client.info.get_datastack_info()
             info_cache["global_server"] = client.server_address
+
         except Exception as e:
             return [], str(e), "", EMPTY_INFO_CACHE, "danger", c.data_resolution
 
         if cell_type_table is None:
             return [], "No Table Selected", "", info_cache, "info", c.data_resolution
 
         if len(anno_id) == 0:
             anno_id = None
         else:
             anno_id = [int(x) for x in anno_id.split(",")]
 
-        live_query = len(live_query_toggle) == 1
+        live_query = mat_version == "live"
 
-        if live_query and not c.disallow_live_query:
-            timestamp = datetime.datetime.utcnow()
+        if live_query:
+            timestamp = datetime.datetime.now(tz=pytz.UTC)
+            timestamp_ngl = None
+            info_cache["ngl_timestamp"] = None
         else:
-            timestamp = None
+            timestamp = client.materialize.get_timestamp()
             timestamp_ngl = client.materialize.get_timestamp()
             info_cache["ngl_timestamp"] = timestamp_ngl.timestamp()
 
         anno_type_lookup = {
             "root_id": "root",
             "nucleus_id": "nucleus",
             "anno_id": "annotation",
         }
 
         annotation_filter = {}
         if value_search is not None or value_search_field is not None:
             if len(value_search_field) > 0 and len(value_search) > 0:
-                annotation_filter = {value_search_field: value_search.split(',')}
+                annotation_filter = {value_search_field: value_search.split(",")}
 
         try:
             tv = TableViewer(
                 cell_type_table,
                 client,
                 c,
                 id_query=anno_id,
@@ -273,30 +330,37 @@
         Input("data-table", "derived_virtual_data"),
         Input("data-table", "derived_virtual_selected_rows"),
         Input("client-info-json", "data"),
         Input("data-resolution-json", "data"),
         Input("pt-column", "data"),
         Input("do-group", "value"),
         Input("group-by", "value"),
+        Input("ngl-target-site", "value"),
     )
     def update_link(
         rows,
         selected_rows,
         info_cache,
         data_resolution,
         pt_column,
         do_group,
         group_column,
+        target_site,
     ):
         def state_text(n):
             return f"Neuroglancer: ({n} rows)"
 
         if info_cache is None:
             return "", "No datastack set", True, ""
 
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if pt_column is None:
             return "", "No clear point field in table", True, ""
 
         if 1 in do_group:
             do_group = True
         else:
             do_group = False
@@ -350,17 +414,29 @@
         Input("data-table", "data"),
         Input("client-info-json", "data"),
         InputDatastack,
         Input("data-resolution-json", "data"),
         Input("pt-column", "data"),
         Input("do-group", "value"),
         Input("group-by", "value"),
+        State("ngl-target-site", "value"),
         prevent_initial_call=True,
     )
-    def update_whole_table_link(_1, _2, rows, info_cache, datastack, data_resolution, pt_column, do_group, group_column):
+    def update_whole_table_link(
+        _1,
+        _2,
+        rows,
+        info_cache,
+        datastack,
+        data_resolution,
+        pt_column,
+        do_group,
+        group_column,
+        target_site,
+    ):
         ctx = callback_context
         if not ctx.triggered:
             return ""
         trigger_src = ctx.triggered[0]["prop_id"].split(".")[0]
         if trigger_src in [
             "submit-button",
             "client-info-json",
@@ -384,14 +460,19 @@
 
         if group_column is None:
             do_group = False
         else:
             if len(group_column) == 0:
                 do_group = False
 
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         df = pd.DataFrame(rows)
         if len(df) > c.max_server_dataframe_length:
             df = df.sample(c.max_server_dataframe_length)
             sampled = True
         else:
             sampled = False
 
@@ -421,21 +502,21 @@
                 [],
                 df,
                 info_cache,
                 c,
                 pt_column,
                 group_annotations=do_group,
                 cell_type_column=group_column,
-                data_resolution= data_resolution,
+                data_resolution=data_resolution,
             )
 
         if sampled:
             link_text = f"Neuroglancer Link (State very large — Random {c.max_server_dataframe_length} shown)"
         else:
-            link_text = f"Neuroglancer Link"
+            link_text = "Neuroglancer Link"
 
         return (
             html.A(link_text, href=url, target="_blank", style={"font-size": "20px"}),
             "Link Generated",
             True,
         )
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/config.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/cell_type_table/layout.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/cell_type_table/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     -------
     layout : list
         List of layout components for the dash app.
     """
     header_row = dbc.Row(
         [
             dbc.Col(
-                html.Div(id='header-bar'),
+                html.Div(id="header-bar"),
                 width={"size": 12},
             ),
         ],
     )
 
     cell_type_query = html.Div(
         children=[
@@ -60,29 +60,26 @@
                             ),
                         ],
                         width={"size": 3, "offset": 1},
                         align="end",
                     ),
                     dbc.Col(
                         [
-                            dbc.Checklist(
+                            "Materialization:",
+                            dcc.Dropdown(
                                 **create_component_kwargs(
                                     state,
-                                    id_inner="live-query-toggle",
-                                    options=[
-                                        {"label": "Live Query", "value": 1},
-                                    ],
-                                    value=[
-                                        1,
-                                    ],
-                                    switch=True,
+                                    id_inner="mat-version",
+                                    options=[{"label": "Latest", "value": ""}],
+                                    value="",
                                     style={
-                                        "bottom-margin": "10px",
-                                        "font-size": "16px",
+                                        "margin-left": "12px",
+                                        "font-size": "12px",
                                     },
+                                    clearable=False,
                                 )
                             ),
                         ],
                         width={"size": 1, "offset": 0},
                         align="center",
                     ),
                     dbc.Col(
@@ -164,15 +161,14 @@
                 ],
                 justify="start",
             ),
             dbc.Row(
                 [
                     dbc.Col(
                         [
-                            
                             html.Div("Value Search (optional):"),
                             dbc.Input(
                                 **create_component_kwargs(
                                     state,
                                     value="",
                                     id_inner="cell-type",
                                     type="text",
@@ -196,15 +192,15 @@
                                     },
                                     clearable=False,
                                 )
                             ),
                         ],
                         width={"size": 1},
                         align="end",
-                    )
+                    ),
                 ],
                 justify="state",
             ),
             html.Hr(),
         ]
     )
 
@@ -283,22 +279,40 @@
                     children="Reset Selection",
                     color="warning",
                     size="sm",
                 ),
                 width=1,
             ),
             dbc.Col(
+                html.Div(
+                    [
+                        dcc.Dropdown(
+                            options={
+                                "seunglab": "Seung-lab Neuroglancer (classic)",
+                                "mainline": "Spelunker (experimental)",
+                            },
+                            value="seunglab",
+                            id="ngl-target-site",
+                            clearable=False,
+                        ),
+                    ],
+                    style={"font-size": "13px"},
+                ),
+                align="top",
+                width={"size": 2, "offset": 1},
+            ),
+            dbc.Col(
                 html.A(
                     "Instructions for filtering the table",
                     href="https://dash.plotly.com/datatable/filtering",
                     style={"font-size": "15px"},
                     target="_blank",
                 ),
                 align="center",
-                width={"size": 2, "offset": 3},
+                width={"size": 2, "offset": 1},
             ),
         ],
         justify="start",
     )
 
     whole_column_link = dbc.Row(
         [
@@ -317,49 +331,51 @@
                                             className="d-grid gap-2 col-6 mx-auto",
                                         ),
                                     ]
                                 ),
                                 dbc.Spinner(
                                     dbc.Row(
                                         html.Div(
-                                            "", id="whole-table-link", className="card-text"
+                                            "",
+                                            id="whole-table-link",
+                                            className="card-text",
                                         ),
-                                        justify='center',
-                                        align='center',
+                                        justify="center",
+                                        align="center",
                                     ),
                                     size="sm",
                                 ),
                             ]
                         )
                     ]
                 ),
             ),
             dbc.Col(
                 dbc.Card(
                     dbc.CardBody(
                         [
-                            html.H4('Annotation Grouping', className='card-title'),
+                            html.H4("Annotation Grouping", className="card-title"),
                             dbc.Checklist(
                                 options=[
                                     {"label": "Group annotations", "value": 1},
                                 ],
                                 value=[],
                                 id="do-group",
                                 switch=True,
                             ),
                             dcc.Dropdown(
                                 options={},
-                                value='cell_type',
-                                id='group-by',
+                                value="cell_type",
+                                id="group-by",
                                 searchable=False,
                             ),
                         ]
                     )
                 )
-            )
+            ),
         ],
     )
 
     datastack_comp = (
         dcc.Input(
             **create_component_kwargs(
                 state,
@@ -387,17 +403,17 @@
             dbc.Container(whole_column_link),
             html.Hr(),
             html.Div(ngl_link),
             html.Div(data_table),
             html.Div(datastack_comp, style={"display": "none"}),
             dcc.Store(id="client-info-json"),
             dcc.Store(id="table-resolution-json"),
-            dcc.Store(id='data-resolution-json'),
-            dcc.Store(id='pt-column'),
-            dcc.Store(id='value-columns'),
+            dcc.Store(id="data-resolution-json"),
+            dcc.Store(id="pt-column"),
+            dcc.Store(id="value-columns"),
         ]
     )
     return layout
 
 
 ######################################################
 # Leave this rest alone for making the template work #
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/config.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
+
 ###########################################
 ### Default data and request parameters ###
 ###########################################
 from .schema_utils import bound_pt_position, split_pt_position, bound_pt_root_id
 
-DATA_RESOLUTION = [1,1,1]
+DATA_RESOLUTION = [1, 1, 1]
+
 
 def parse_environ_vector(input, num_type):
     return [num_type(x) for x in input.split(",")]
 
 
 class CommonConfig(object):
     def __init__(self, config):
@@ -16,14 +18,17 @@
         if self.default_datastack is None:
             raise ValueError("Must datastack parameter!")
 
         self.server_address = config.get("server_address")
         if self.server_address is None:
             raise ValueError("Must set server address parameter!")
 
+        self.viewer_site = config.get("viewer_site", None)
+        self.target_site = config.get("target_site", None)
+
         self.disallow_live_query = config.get("disallow_live_query", False)
         self.image_black = config.get("image_black", 0)
         self.image_white = config.get("image_white", 1)
 
         self.target_root_id_per_call = config.get("target_root_id_per_call", 200)
         self.max_chunks = config.get("max_chunks", 20)
         self.pool_maxsize = 2 * self.max_chunks
@@ -39,15 +44,15 @@
         self.max_server_dataframe_length = config.get(
             "max_server_dataframe_length", 20_000
         )
 
         # If None, the info service is used
         self.nucleus_table = config.get("nucleus_table", None)
         self.nucleus_id_column = config.get("nucleus_id_column", "id")
-        self.nucleus_filter = config.get('nucleus_filter', {})
+        self.nucleus_filter = config.get("nucleus_filter", {})
 
         self.debug = config.get("debug", False)
 
         # Used to look up number of neurons per root id
         self.soma_table = self.nucleus_table
         self.soma_id_column = self.nucleus_id_column
 
@@ -135,8 +140,8 @@
         return bound_pt_root_id(self.ct_cell_type_point)
 
 
 def RegisterTable(pt, value_columns, config):
     config = copy.deepcopy(config)
     config.ct_cell_type_point = pt
     config.value_columns = [config.nucleus_id_column] + value_columns
-    return config
+    return config
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/dash_url_helper.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dash_url_helper.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/dataframe_utilities.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/dataframe_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,28 @@
 from .transform_utils import extract_depth
 import flask
 
 DESIRED_RESOLUTION = [1, 1, 1]
 
 
 def query_table_any(
-    table, root_id_column, root_ids, client, timestamp, extra_query={}, is_live=True
+    table,
+    root_id_column,
+    root_ids,
+    client,
+    timestamp,
+    extra_query={},
+    is_live=True,
 ):
     if root_ids is not None:
         root_ids = np.array(root_ids)
         root_ids = root_ids[root_ids != 0]
-    ref_table = table_metadata(table, client).get("reference_table")
+    meta = table_metadata(table, client)
+    ref_table = meta.get("reference_table")
+    print(f"Table metadata for table {table}:", meta)
     if ref_table is not None:
         return _query_table_join(
             table,
             root_id_column,
             root_ids,
             client,
             timestamp,
@@ -80,14 +88,15 @@
         )
     else:
         return client.materialize.query_table(
             table,
             split_positions=True,
             desired_resolution=DESIRED_RESOLUTION,
             metadata=False,
+            timestamp=timestamp,
             **filter_kwargs,
         )
 
 
 def _query_table_join(
     table, root_id_column, root_ids, client, timestamp, ref_table, extra_query, is_live
 ):
@@ -262,19 +271,21 @@
         repopulate_list(col, df)
     return df
 
 
 def _expand_column(df, column, len_column="num_syn"):
     def _expand_column(row):
         return [row[column]] * row[len_column]
+
     if len(df) > 0:
         return np.concatenate(list(df.apply(_expand_column, axis=1)))
     else:
         return np.array([])
 
+
 def _slam_column(df, column):
     if len(df) > 0:
         return np.concatenate(df[column].values)
     else:
         return np.array([])
 
 
@@ -287,15 +298,14 @@
     data_dict = {k: _slam_column(dfnn, k) for k in config.syn_pt_position_split}
 
     value_cols.append(config.soma_depth_column)
     for col in value_cols:
         if col != "":
             data_dict[col] = _expand_column(dfnn, col)
     df_rh = pd.DataFrame(data_dict).replace("nan", None)
-
     extract_depth(
         df_rh,
         config.synapse_depth_column,
         config.syn_pt_position,
         aligned_volume,
     )
     return df_rh
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/link_utilities.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/link_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,38 @@
 from .lookup_utilities import make_client
 from .schema_utils import bound_pt_position, bound_pt_root_id
 from .dataframe_utilities import rehydrate_dataframe
 
 EMPTY_INFO_CACHE = {"aligned_volume": {}, "cell_type_column": None}
 MAX_URL_LENGTH = 1_750_000
 DEFAULT_NGL = "https://neuromancer-seung-import.appspot.com/"
+DEFAULT_SPELUNKER = "https://spelunker.cave-explorer.org/"
+
+
+def get_viewer_site_from_target(viewer_site, target_site):
+    if target_site == "seunglab":
+        if viewer_site:
+            return viewer_site
+        else:
+            return DEFAULT_NGL
+    elif target_site == "mainline":
+        return DEFAULT_SPELUNKER
 
 
 def image_source(info_cache):
     if info_cache is None:
         return None
     return info_cache["aligned_volume"].get("image_source", "")
 
+
 def aligned_volume(info_cache):
     if info_cache is None:
         return None
-    return info_cache.get('aligned_volume', {}).get('name')
+    return info_cache.get("aligned_volume", {}).get("name")
+
 
 def seg_source(info_cache):
     if info_cache is None:
         return None
     return info_cache.get("segmentation_source", "")
 
 
@@ -61,31 +74,38 @@
             info_cache.get("viewer_resolution_z"),
         ]
         return vr
     except:
         return None
 
 
+def target_site(info_cache):
+    if info_cache is None:
+        return None
+    return info_cache.get("target_site", None)
+
+
 def statebuilder_kwargs(info_cache):
     return dict(
         url_prefix=viewer_site(info_cache),
         state_server=state_server(info_cache),
         resolution=voxel_resolution_from_info(info_cache),
+        target_site=target_site(info_cache),
     )
 
 
 def generate_statebuilder(
     info_cache,
     config,
     base_root_id=None,
     base_color="#ffffff",
     preselect_all=True,
     anno_column="post_pt_root_id",
     anno_layer="syns",
-    data_resolution=[1,1,1],
+    data_resolution=[1, 1, 1],
 ):
     img = statebuilder.ImageLayerConfig(
         image_source(info_cache),
         contrast_controls=True,
         black=config.image_black,
         white=config.image_white,
     )
@@ -130,17 +150,19 @@
         [img, seg, anno],
         **statebuilder_kwargs(info_cache),
     )
     return sb
 
 
 def generate_statebuilder_pre(
-    info_cache, config, preselect=False, data_resolution=[1,1,1],
+    info_cache,
+    config,
+    preselect=False,
+    data_resolution=[1, 1, 1],
 ):
-
     img = statebuilder.ImageLayerConfig(
         image_source(info_cache),
         contrast_controls=True,
         black=config.image_black,
         white=config.image_white,
     )
     seg = statebuilder.SegmentationLayerConfig(
@@ -166,15 +188,15 @@
     sb = statebuilder.StateBuilder(
         [img, seg, anno],
         **statebuilder_kwargs(info_cache),
     )
     return sb
 
 
-def generate_statebuilder_post(info_cache, config, data_resolution=[1,1,1]):
+def generate_statebuilder_post(info_cache, config, data_resolution=[1, 1, 1]):
     img = statebuilder.ImageLayerConfig(
         image_source(info_cache),
         contrast_controls=True,
         black=config.image_black,
         white=config.image_white,
     )
 
@@ -207,15 +229,15 @@
 
 def generate_statebuider_syn_grouped(
     info_cache,
     anno_name,
     config,
     fixed_id_color="#FFFFFF",
     preselect=False,
-    data_resolution=[1,1,1],
+    data_resolution=[1, 1, 1],
 ):
     points = statebuilder.PointMapper(
         point_column=config.syn_pt_position,
         linked_segmentation_column=config.root_id_col,
         group_column=config.root_id_col,
         split_positions=True,
         multipoint=True,
@@ -262,22 +284,21 @@
 
 def generate_url_cell_types(
     selected_rows,
     df,
     info_cache,
     config,
     pt_column,
-    cell_type_column='cell_type',
+    cell_type_column="cell_type",
     group_annotations=False,
     multipoint=False,
     fill_null=None,
     return_as="url",
-    data_resolution=[1,1,1],
+    data_resolution=[1, 1, 1],
 ):
-    
     if len(selected_rows) > 0 or selected_rows is None:
         df = df.iloc[selected_rows].reset_index(drop=True)
 
     img = statebuilder.ImageLayerConfig(
         image_source(info_cache),
         contrast_controls=True,
         black=config.image_black,
@@ -312,40 +333,44 @@
                     mapping_rules=statebuilder.PointMapper(
                         bound_pt_position(pt_column),
                         linked_segmentation_column=config.root_id_col,
                         set_position=True,
                         multipoint=multipoint,
                         split_positions=True,
                         mapping_set=ct,
-                    )
+                    ),
                 )
             )
-        sb = statebuilder.StateBuilder([img, seg] + annos, **statebuilder_kwargs(info_cache))
+        sb = statebuilder.StateBuilder(
+            [img, seg] + annos, **statebuilder_kwargs(info_cache)
+        )
         return sb.render_state(
             {ct: df.query(f"{cell_type_column}==@ct") for ct in cell_types},
             return_as=return_as,
         )
     else:
         if cell_type_column is not None:
-            if len(cell_type_column)==0:
-                cell_type_column=None
+            if len(cell_type_column) == 0:
+                cell_type_column = None
         anno = statebuilder.AnnotationLayerConfig(
-            'Annotations',
+            "Annotations",
             linked_segmentation_layer=seg.name,
             mapping_rules=statebuilder.PointMapper(
                 bound_pt_position(pt_column),
                 linked_segmentation_column=config.root_id_col,
                 split_positions=True,
                 multipoint=multipoint,
                 set_position=True,
                 description_column=cell_type_column,
             ),
             data_resolution=data_resolution,
         )
-        sb = statebuilder.StateBuilder([img, seg, anno], **statebuilder_kwargs(info_cache))
+        sb = statebuilder.StateBuilder(
+            [img, seg, anno], **statebuilder_kwargs(info_cache)
+        )
         return sb.render_state(
             df,
             return_as=return_as,
         )
 
     # for ct, clr in zip(cell_types, cycle(colors)):
     #     anno = statebuilder.AnnotationLayerConfig(
@@ -376,15 +401,15 @@
     info_cache,
     rows,
     config,
     cell_type_column="cell_type",
     group_annotations=True,
     multipoint=False,
     fill_null=None,
-    data_resolution=[1,1,1],
+    data_resolution=[1, 1, 1],
     include_no_type=True,
 ):
     df = rehydrate_dataframe(rows, config.syn_pt_position_split)
     if fill_null and include_no_type:
         df[cell_type_column].fillna(fill_null, inplace=True)
 
     cell_types = np.sort(pd.unique(df[cell_type_column].dropna()))
@@ -421,21 +446,23 @@
                 multipoint=multipoint,
                 split_positions=True,
                 mapping_set=ct,
             ),
             data_resolution=data_resolution,
         )
         annos.append(anno)
-            # statebuilder.StateBuilder(
-                # [anno],
-                # **statebuilder_kwargs(info_cache),
-            # )
+        # statebuilder.StateBuilder(
+        # [anno],
+        # **statebuilder_kwargs(info_cache),
+        # )
         # )
         # dfs.append(df.query(f"{cell_type_column} == @ct"))
-    sb = statebuilder.StateBuilder([img, seg] + annos, **statebuilder_kwargs(info_cache))
+    sb = statebuilder.StateBuilder(
+        [img, seg] + annos, **statebuilder_kwargs(info_cache)
+    )
     # csb = statebuilder.ChainedStateBuilder(sbs)
     df_dict = {ct: df.query(f'{cell_type_column}=="{ct}"') for ct in cell_types}
     return sb, df_dict
 
 
 def make_url_robust(df, sb, datastack, config):
     """Generate a url from a neuroglancer state. If too long, return through state server"""
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/lookup_utilities.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/lookup_utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,90 @@
 import flask
 from .schema_utils import get_table_info, populate_metadata_cache
 from caveclient.tools.caching import CachedClient as CAVEclient
 from .dataframe_utilities import query_table_any
 import numpy as np
+from cachetools import cached, TTLCache
+from cachetools.keys import hashkey
+from datetime import datetime
+import pytz
+
+
+def get_versions(client, n_years=1):
+    version_metadata = client.materialize.get_versions_metadata()
+    now = datetime.now(tz=pytz.UTC)
+    keep_versions = {}
+    latest_version = 0
+    for vmeta in version_metadata:
+        delta_days = (vmeta["expires_on"] - now).days
+        if delta_days >= n_years * 365:
+            keep_versions[f"v{vmeta['version']}"] = vmeta["version"]
+        if vmeta["version"] > latest_version:
+            latest_version = vmeta["version"]
+    keep_versions["latest"] = latest_version
+    return keep_versions
+
+
+def get_version_options(client, disallow_live_query):
+    mat_versions = get_versions(client)
+    version_options = []
+    if not disallow_live_query:
+        version_options.append(
+            {
+                "label": "Live Query",
+                "value": "live",
+            }
+        )
+    latest_version = mat_versions.pop("latest")
+    version_options.append(
+        {"label": f"Latest (v{latest_version})", "value": latest_version}
+    )
+
+    long_lived = sorted(mat_versions.keys())[::-1]
+    for k in long_lived:
+        if mat_versions[k] != latest_version:
+            version_options.append({"label": k, "value": mat_versions[k]})
+
+    if not disallow_live_query:
+        default_value = "live"
+    else:
+        default_value = latest_version
+    return version_options, default_value
+
 
 def table_is_value_source(table, client):
     if table is None:
         return False
     pt, vals = get_table_info(table, client)
     if pt is not None and len(vals) > 0:
         return True
     else:
         return False
 
-def get_all_schema_tables(
-    datastack,
-    config,
-):
-    client = make_client(datastack, config.server_address)
+
+def get_all_schema_tables(datastack, config, mat_version=None):
+    client = make_client(
+        datastack, config.server_address, materialize_version=mat_version
+    )
     tables = client.materialize.get_tables()
     populate_metadata_cache(tables, client)
     schema_tables = []
-    is_val_source = {t: table_is_value_source(t, client) for t in tables if t not in config.omit_cell_type_tables}
+    is_val_source = {
+        t: table_is_value_source(t, client)
+        for t in tables
+        if t not in config.omit_cell_type_tables
+    }
     schema_tables = [k for k, v in is_val_source.items() if v]
     return [{"label": t, "value": t} for t in sorted(schema_tables)]
 
-def get_type_tables(datastack, config):
-    tables = get_all_schema_tables(datastack, config)
+
+def get_type_tables(datastack, config, mat_version=None):
+    if mat_version == "" or mat_version == "live":
+        mat_version = None
+    tables = get_all_schema_tables(datastack, config, mat_version)
     named_options = config.cell_type_dropdown_options
     if named_options is None:
         return tables
     else:
         if len(named_options) == 0:
             named_option_dict = dict()
         named_option_dict = {r["value"]: r["label"] for r in named_options[::-1]}
@@ -42,15 +96,15 @@
                 {"label": named_option_dict.get(t["value"]), "value": t["value"]}
             ] + new_tables
         else:
             new_tables.append(t)
     return new_tables
 
 
-def make_client(datastack, server_address, **kwargs):
+def make_client(datastack, server_address, materialize_version=None, **kwargs):
     """Build a framework client with appropriate auth token
 
     Parameters
     ----------
     datastack : str
         Datastack name for client
     config : dict
@@ -59,15 +113,19 @@
         Global server address for the client, by default None. If None, uses the config dict.
 
     """
     try:
         auth_token = flask.g.get("auth_token", None)
     except:
         auth_token = None
-    client = CAVEclient(datastack, server_address=server_address, auth_token=auth_token, **kwargs)
+    client = CAVEclient(
+        datastack, server_address=server_address, auth_token=auth_token, **kwargs
+    )
+    if materialize_version:
+        client.materialize.version = materialize_version
     return client
 
 
 def get_root_id_from_nuc_id(
     nuc_id,
     client,
     nucleus_table,
@@ -92,22 +150,23 @@
 
     Returns
     -------
     [type]
         [description]
     """
     df = query_table_any(
-            nucleus_table,
-            config.soma_pt_root_id,
-            None,
-            client,
-            timestamp=timestamp,
-            extra_query={config.nucleus_id_column: [nuc_id]},
-            is_live=is_live,
+        nucleus_table,
+        config.soma_pt_root_id,
+        None,
+        client,
+        timestamp=timestamp,
+        extra_query={config.nucleus_id_column: [nuc_id]},
+        is_live=is_live,
     )
+
     if len(df) == 0:
         return None
     else:
         return df.iloc[0][config.soma_pt_root_id]
 
 
 def get_nucleus_id_from_root_id(
@@ -132,7 +191,24 @@
 
     if len(df) == 0:
         return None
     elif len(df) == 1:
         return df[config.nucleus_id_column].values[0]
     else:
         return df[config.nucleus_id_column].values
+
+
+table_option_cache = TTLCache(maxsize=128, ttl=3600)
+
+
+def table_hash(table_name, client):
+    return hashkey(
+        table_name, client.datastack_name, str(client.materialize.get_timestamp())
+    )
+
+
+@cached(cache=table_option_cache, key=table_hash)
+def get_unique_table_values(
+    table_name,
+    client,
+) -> dict:
+    return client.materialize.get_unique_string_values(table_name)
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/neuron_data_base.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/neuron_data_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import pandas as pd
 import numpy as np
 from dfbridge import DataframeBridge
 
 from dash_connectivity_viewer.common.lookup_utilities import (
     get_nucleus_id_from_root_id,
     get_root_id_from_nuc_id,
-    make_client
+    make_client,
 )
 
 from .dataframe_utilities import *
 from .link_utilities import voxel_resolution_from_info
 from multiprocessing import cpu_count
 from ..common.schema_utils import split_pt_position
 
+
 def _soma_property_entry(soma_table, c):
     return {
         soma_table: {
             "root_id": c.soma_pt_root_id,
             "include": split_pt_position(c.soma_pt_position) + [c.nucleus_id_column],
             "aggregate": {
                 c.num_soma_prefix: {
@@ -59,75 +60,95 @@
         client,
         config,
         timestamp=None,
         n_threads=None,
         id_type="root",
         is_live=True,
     ):
-
         if id_type == "root":
             self._root_id = object_id
             self._nucleus_id = None
         elif id_type == "nucleus":
             self._root_id = None
             self._nucleus_id = object_id
 
         self._client = make_client(
             datastack=client.datastack_name,
+            materialize_version=client.materialize.version,
             server_address=client.server_address,
             pool_block=True,
             pool_maxsize=config.pool_maxsize,
         )
 
         self._property_tables = {}
 
         if config.synapse_table is None:
             synapse_table = self._client.info.get_datastack_info().get("synapse_table")
         self._synapse_table = synapse_table
         self._synapse_table_properties = _synapse_properties(synapse_table, config)
 
-        
         self._soma_table = self._client.info.get_datastack_info().get("soma_table")
 
         self.config = config
 
         self._timestamp = timestamp
         self.old_root_id = None
 
         self.is_live = is_live
 
         self._pre_syn_df = None
         self._post_syn_df = None
-        self._synapse_data_resolution = np.array([1,1,1])
+        self._synapse_data_resolution = np.array([1, 1, 1])
 
         self._viewer_resolution = voxel_resolution_from_info(client.info.info_cache)
 
         if n_threads is None:
             n_threads = cpu_count()
         self.n_threads = n_threads
 
         self._partner_soma_table = None
         self._partner_root_ids = None
         if config.debug:
-            print("\nNew datastack: ", self._client.datastack_name, 'soma_table:', self._soma_table, '\n')
+            print(
+                "\nNew datastack: ",
+                self._client.datastack_name,
+                "soma_table:",
+                self._soma_table,
+                "\n",
+            )
         self.check_root_id()
         if self._soma_table is not None:
             self._property_tables.update(
                 _soma_property_entry(
                     self._soma_table,
                     config,
                 )
             )
         if config.debug:
-            print("\Confirm datastack: ", self._client.datastack_name, 'soma_table:', self._soma_table, '\n')
+            print(
+                "Confirm datastack: ",
+                self._client.datastack_name,
+                "soma_table:",
+                self._soma_table,
+                "\n",
+            )
             print(f"Property tables: \n{self._property_tables}\n")
- 
+
     @property
     def root_id(self):
         if self._root_id is None:
+            if self.config.debug:
+                print(
+                    "Get root id: ",
+                    self._nucleus_id,
+                    self.client.materialize.version,
+                    self.soma_table,
+                    self.timestamp,
+                    self.is_live,
+                )
             new_root_id = get_root_id_from_nuc_id(
                 self._nucleus_id,
                 self.client,
                 self.soma_table,
                 self.config,
                 self.timestamp,
                 self.is_live,
@@ -135,35 +156,40 @@
             if new_root_id is None:
                 raise Exception("Nucleus ID not found in soma table")
             else:
                 self._root_id = new_root_id
         return self._root_id
 
     def check_root_id(self):
-        if self.client.chunkedgraph.is_latest_roots([self.root_id])[0]:
+        if self.config.debug:
+            print("Check root id: ", self.timestamp, self.root_id)
+        if self.client.chunkedgraph.is_latest_roots(
+            [self.root_id], timestamp=self.timestamp
+        )[0]:
             pass
         else:
             self.old_root_id = self.root_id
             self._root_id = self.client.chunkedgraph.suggest_latest_roots(
                 self.root_id,
-                timestamp=self._timestamp,
+                timestamp=self.timestamp,
             )
         pass
 
     @property
     def nucleus_id(self):
         if self.soma_table is None:
             return None
         if self._nucleus_id is None:
             self._nucleus_id = get_nucleus_id_from_root_id(
                 self._root_id,
                 self.client,
                 self.soma_table,
                 self.config,
                 self.timestamp,
+                self.is_live,
             )
         return self._nucleus_id
 
     @property
     def client(self):
         return self._client
 
@@ -227,15 +253,15 @@
             np.concatenate(
                 (
                     self._pre_syn_df[self.config.post_pt_root_id].values,
                     self._post_syn_df[self.config.pre_pt_root_id].values,
                 )
             )
         )
-        return root_ids[root_ids!=0]
+        return root_ids[root_ids != 0]
 
     def partners_out(self, properties=True):
         return self._targ_table("pre", properties)
 
     def partners_in(self, properties=True):
         return self._targ_table("post", properties)
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/schema_utils.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/schema_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,80 @@
 from cachetools import cached, TTLCache, keys
+
 SPLIT_SUFFIXES = ["x", "y", "z"]
 
 
-#json schema column types that can act as potential columns for looking at tables
-ALLOW_COLUMN_TYPES = ['integer', 'boolean', 'string', 'float']
+# json schema column types that can act as potential columns for looking at tables
+ALLOW_COLUMN_TYPES = ["integer", "boolean", "string", "float"]
+
+
 # Helper functions for turning schema field names ot column names
 def bound_pt_position(pt):
     return f"{pt}_position"
 
+
 def bound_pt_root_id(pt):
     return f"{pt}_root_id"
 
+
 def split_pt_position(pt_position):
     return [f"{pt_position}_{suf}" for suf in SPLIT_SUFFIXES]
 
+
 _schema_cache = TTLCache(maxsize=128, ttl=86_400)
+
+
 def _schema_key(schema_name, client, **kwargs):
-    allow_types = kwargs.get('allow_types', ALLOW_COLUMN_TYPES)
-    key = keys.hashkey(schema_name, str(allow_types), client.datastack_name)
+    allow_types = kwargs.get("allow_types", ALLOW_COLUMN_TYPES)
+    key = keys.hashkey(
+        schema_name, str(allow_types), client.datastack_name, client.materialize.version
+    )
     return key
 
+
 @cached(cache=_schema_cache, key=_schema_key)
-def get_col_info(schema_name, client, spatial_point='BoundSpatialPoint', allow_types=ALLOW_COLUMN_TYPES, omit_fields=[]):
+def get_col_info(
+    schema_name,
+    client,
+    spatial_point="BoundSpatialPoint",
+    allow_types=ALLOW_COLUMN_TYPES,
+    omit_fields=[],
+):
     schema = client.schema.schema_definition(schema_name)
     sp_name = f"#/definitions/{spatial_point}"
     n_sp = 0
-    sn = schema['$ref'].split('/')[-1]
+    sn = schema["$ref"].split("/")[-1]
     add_cols = []
-    for k, v in schema['definitions'][sn]['properties'].items():
-        if v.get('$ref','') == sp_name:
+    for k, v in schema["definitions"][sn]["properties"].items():
+        if v.get("$ref", "") == sp_name:
             pt_name = k
-            n_sp+=1
+            n_sp += 1
         else:
             if k in omit_fields:
                 continue
             # Field type is format if exists, type otherwise
-            if v.get('format', v.get('type')) in allow_types:
+            if v.get("format", v.get("type")) in allow_types:
                 add_cols.append(k)
     if n_sp != 1:
         pt_name = None
     return pt_name, add_cols
 
+
 _table_cache = TTLCache(maxsize=128, ttl=86_400)
+
+
 def _table_key(table_name, client, **kwargs):
-    merge_schema = kwargs.get('merge_schema', True)
-    allow_types = kwargs.get('allow_types', ALLOW_COLUMN_TYPES)
-    key = keys.hashkey(table_name, merge_schema, str(allow_types))
+    merge_schema = kwargs.get("merge_schema", True)
+    allow_types = kwargs.get("allow_types", ALLOW_COLUMN_TYPES)
+    key = keys.hashkey(
+        table_name, merge_schema, str(allow_types), client.materialize.version
+    )
     return key
 
+
 @cached(cache=_table_cache, key=_table_key)
 def get_table_info(tn, client, allow_types=ALLOW_COLUMN_TYPES, merge_schema=True):
     """Get the point column and additional columns from a table
 
     Parameters
     ----------
     tn : str
@@ -67,45 +90,59 @@
         Point column prefix
     cols
         List of additional columns names
     """
     if tn is None:
         return None, []
     meta = table_metadata(tn, client)
-    ref_table = meta.get('reference_table')
-    if ref_table is None or merge_schema is False:
-        schema = meta['schema']
+    ref_table = meta.get("reference_table")
+    if ref_table is None or ref_table == "" or merge_schema is False:
+        schema = meta["schema"]
         extra_cols = []
     else:
-        schema = table_metadata(ref_table, client).get('schema')
-        _, extra_cols = get_col_info(meta['schema'], client, allow_types=allow_types, omit_fields=['target_id'])
+        schema = table_metadata(ref_table, client).get("schema")
+        _, extra_cols = get_col_info(
+            meta["schema"], client, allow_types=allow_types, omit_fields=["target_id"]
+        )
     pt, add_cols = get_col_info(schema, client, allow_types=allow_types)
     cols = add_cols + extra_cols
     return pt, cols
 
+
 _metadata_cache = TTLCache(maxsize=128, ttl=86_400)
+
+
 def _metadata_key(tn, client, **kwargs):
-    key = keys.hashkey(tn, client.datastack_name)
+    key = keys.hashkey(tn, client.datastack_name, client.materialize.version)
     return key
 
+
 @cached(cache=_metadata_cache, key=_metadata_key)
 def table_metadata(table_name, client, meta=None):
     "Caches getting table metadata"
     if table_name is None:
         return None
     if meta is None:
         meta = client.materialize.get_table_metadata(table_name)
     if "schema" not in meta:
-        meta["schema"] = meta.get('schema_type')
+        meta["schema"] = meta.get("schema_type")
     return meta
 
+
 _table_list_cache = TTLCache(maxsize=64, ttl=86_400)
+
+
 def _table_list_key(tables, client):
-    key = keys.hashkey('_'.join(tables), client.datastack_name)
+    key = keys.hashkey(
+        "_".join(tables), client.datastack_name, client.materialize.version
+    )
     return key
 
+
 @cached(cache=_table_list_cache, key=_table_list_key)
 def populate_metadata_cache(tables, client):
-    all_meta = client.materialize.get_tables_metadata()
+    all_meta = client.materialize.get_tables_metadata(
+        version=client.materialize.version
+    )
     for tn, meta in zip(tables, all_meta):
         table_metadata(tn, client, meta=meta)
-    pass
+    pass
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/table_lookup.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/table_lookup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,20 @@
         config,
         timestamp=None,
         id_query=None,
         id_query_type=None,
         column_query={},
         is_live=True,
     ):
-
         self._client = make_client(
             datastack=client.datastack_name,
             server_address=client.server_address,
         )
+        self._client.materialize.version = client.materialize.version
+
         pt, add_cols = get_table_info(table_name, self._client)
         config = RegisterTable(pt, add_cols, config)
         self.config = config
         self._cell_type_bridge_schema = _table_schema(config)
 
         if config.soma_table is None:
             soma_table = self._client.info.get_datastack_info().get("soma_table")
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/common/transform_utils.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/common/transform_utils.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/__init__.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/callbacks.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from dash import html
+import numpy as np
+import pytz
 from ..common.neuron_data_base import NeuronData
 from dash.dependencies import Input, Output, State
 from dash import callback_context
 
 from ..common.link_utilities import (
     generate_statebuider_syn_grouped,
     generate_statebuilder,
     generate_statebuilder_pre,
     generate_statebuilder_post,
     EMPTY_INFO_CACHE,
     MAX_URL_LENGTH,
     make_url_robust,
+    get_viewer_site_from_target,
 )
 from ..common.dataframe_utilities import (
-    stringify_root_ids, stringify_list, repopulate_list
+    stringify_root_ids,
+    stringify_list,
+    repopulate_list,
 )
 from ..common.dash_url_helper import _COMPONENT_ID_TYPE
-from ..common.lookup_utilities import make_client
+from ..common.lookup_utilities import make_client, get_version_options
 from .config import ConnectivityConfig
 
 import datetime
 import pandas as pd
 
 try:
     from loguru import logger
@@ -29,24 +34,27 @@
     logger = None
 
 
 InputDatastack = Input({"id_inner": "datastack", "type": _COMPONENT_ID_TYPE}, "value")
 OutputDatastack = Output({"id_inner": "datastack", "type": _COMPONENT_ID_TYPE}, "value")
 StateAnnoID = State({"id_inner": "anno-id", "type": _COMPONENT_ID_TYPE}, "value")
 StateAnnoType = State({"id_inner": "cell-id-type", "type": _COMPONENT_ID_TYPE}, "value")
-StateLiveQuery = State(
-    {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE}, "value"
-)
 
-OutputLiveQueryToggle = Output(
-    {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE},
-    "options",
+
+InputMaterializationVersion = Input(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
+)
+StateMaterializationVersion = State(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
 )
-OutputLiveQueryValue = Output(
-    {"id_inner": "live-query-toggle", "type": _COMPONENT_ID_TYPE}, "value"
+OutputMaterializeOptions = Output(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "options"
+)
+OutputMaterializeValue = Output(
+    {"id_inner": "mat-version", "type": _COMPONENT_ID_TYPE}, "value"
 )
 
 
 def register_callbacks(app, config):
     c = ConnectivityConfig(config)
 
     @app.callback(
@@ -54,77 +62,90 @@
         Input("reset-selection", "n_clicks"),
         Input("connectivity-tab", "value"),
     )
     def reset_selection(n_clicks, tab_value):
         return []
 
     @app.callback(
-        Output("header-bar", 'children'),
+        Output("header-bar", "children"),
         InputDatastack,
     )
     def set_header(datastack):
-        return html.H3(f"Connectivity Info — {datastack}", className="bg-primary text-white p-2 mb-2 text-center")
+        return html.H3(
+            f"Connectivity Info — {datastack}",
+            className="bg-primary text-white p-2 mb-2 text-center",
+        )
 
     @app.callback(
         Output("data-table", "columns"),
         InputDatastack,
     )
     def define_table_columns(_):
         return [{"name": i, "id": i} for i in c.table_columns]
 
     @app.callback(
+        OutputMaterializeOptions,
+        OutputMaterializeValue,
+        InputDatastack,
+    )
+    def get_materialization_versions(
+        datastack_name,
+    ):
+        # Produce ordered list of materialization versions to choose from
+        client = make_client(datastack_name, c.server_address)
+        version_options, default_value = get_version_options(
+            client, c.disallow_live_query
+        )
+        return version_options, default_value
+
+    @app.callback(
         OutputDatastack,
         InputDatastack,
     )
     def define_datastack(datastack):
         if datastack is None:
             datastack = ""
 
         if len(datastack) == 0:
             return c.default_datastack
         else:
             return datastack
 
     @app.callback(
-        OutputLiveQueryToggle,
-        OutputLiveQueryValue,
-        InputDatastack,
-        StateLiveQuery,
-    )
-    def disable_live_query(_, lq):
-        options_active = [{"label": "Live Query", "value": 1}]
-        options_disabled = [{"label": "Live Query", "value": 1, "disabled": True}]
-        if c.disallow_live_query:
-            return options_disabled, ""
-        else:
-            return options_active, lq
-
-    @app.callback(
         Output("target-table-json", "data"),
         Output("source-table-json", "data"),
         Output("output-tab", "label"),
         Output("input-tab", "label"),
         Output("reset-selection", "n_clicks"),
         Output("client-info-json", "data"),
         Output("loading-spinner", "children"),
         Output("message-text", "children"),
         Output("message-text", "color"),
         Output("synapse-table-resolution-json", "data"),
         Input("submit-button", "n_clicks"),
         InputDatastack,
         StateAnnoID,
         StateAnnoType,
-        StateLiveQuery,
+        StateMaterializationVersion,
     )
-    def update_data(_, datastack_name, anno_id, id_type, live_query_toggle):
+    def update_data(_, datastack_name, anno_id, id_type, mat_version):
         if logger is not None:
             t0 = time.time()
 
+        if mat_version == "live" or mat_version == "":
+            version = None
+        else:
+            version = mat_version
+
         try:
-            client = make_client(datastack_name, c.server_address)
+            client = make_client(
+                datastack_name, c.server_address, materialize_version=version
+            )
+            if version is None:
+                version = client.materialize.version
             info_cache = client.info.info_cache[datastack_name]
             info_cache["global_server"] = client.server_address
         except Exception as e:
             return (
                 [],
                 [],
                 "Output",
@@ -151,17 +172,20 @@
                 None,
             )
 
         if len(anno_id) == 0:
             anno_id = None
             id_type = "anno_id"
 
-        live_query = len(live_query_toggle) == 1
-        if live_query and not c.disallow_live_query:
-            timestamp = datetime.datetime.utcnow()
+        live_query = mat_version == "live"
+
+        if live_query:
+            timestamp = datetime.datetime.now(tz=pytz.UTC)
+            timestamp_ngl = None
+            info_cache["ngl_timestamp"] = None
         else:
             timestamp = client.materialize.get_timestamp()
             timestamp_ngl = client.materialize.get_timestamp()
             info_cache["ngl_timestamp"] = timestamp_ngl.timestamp()
 
         if anno_id is None:
             root_id = None
@@ -173,20 +197,21 @@
                 object_id = int(anno_id)
                 object_id_type = "nucleus"
             else:
                 raise ValueError('id_type must be either "root_id" or "nucleus_id"')
 
         try:
             nrn_data = NeuronData(
-                object_id,
-                client,
+                object_id=object_id,
+                client=client,
                 config=c,
                 timestamp=timestamp,
                 id_type=object_id_type,
                 n_threads=1,
+                is_live=live_query,
             )
 
             root_id = nrn_data.root_id
 
             pre_targ_df = nrn_data.partners_out()
             pre_targ_df = stringify_root_ids(
                 pre_targ_df, stringify_cols=[c.root_id_col]
@@ -200,23 +225,23 @@
                 stringify_list(col, pre_targ_df)
                 stringify_list(col, post_targ_df)
 
             n_syn_pre = pre_targ_df[c.num_syn_col].sum()
             n_syn_post = post_targ_df[c.num_syn_col].sum()
 
             info_cache["root_id"] = str(root_id)
-        
+
         except Exception as e:
             return (
                 [],
                 [],
                 "Output",
                 "Input",
                 1,
-                EMPTY_INFO_CACHE,
+                info_cache,
                 "",
                 str(e),
                 "danger",
                 None,
             )
 
         if logger is not None:
@@ -224,21 +249,29 @@
                 f"Data update for {root_id} | time:{time.time() - t0:.2f} s, syn_in: {n_syn_post} , syn_out: {n_syn_pre}"
             )
 
         if nrn_data.old_root_id is not None:
             change_root_id_text = f" Warning: {nrn_data.old_root_id} is not valid at timestamp queried! Showing data for the most overlapping valid root id. —"
             output_status = "warning"
         else:
-            change_root_id_text = ""        
+            change_root_id_text = ""
             output_status = "success"
 
-        if timestamp is not None:
-            output_message = f"{change_root_id_text}Current connectivity for root id {root_id}."
+        if nrn_data.nucleus_id is not None and nrn_data.soma_table is not None:
+            if np.issubdtype(type(nrn_data.nucleus_id), np.integer):
+                nuc_id_text = f"  (nucleus id: {nrn_data.nucleus_id})"
+            else:
+                nuc_id_text = f" (Multiple nucleus ids in segment: {', '.join([str(x) for x in nrn_data.nucleus_id])})"
+        else:
+            nuc_id_text = ""
+
+        if live_query:
+            output_message = f"{change_root_id_text}Current connectivity for root id {root_id}{nuc_id_text}."
         else:
-            output_message = f"{change_root_id_text}Connectivity for root id {root_id} materialized on {timestamp_ngl:%m/%d/%Y} (v{client.materialize.version})."
+            output_message = f"{change_root_id_text}Connectivity for root id {root_id}{nuc_id_text} materialized on {timestamp_ngl:%m/%d/%Y} (v{client.materialize.version})."
 
         return (
             pre_targ_df.to_dict("records"),
             post_targ_df.to_dict("records"),
             f"Output (n = {n_syn_pre})",
             f"Input (n = {n_syn_post})",
             1,
@@ -273,29 +306,37 @@
         Output("ngl_link", "disabled"),
         Output("link-loading", "children"),
         Input("connectivity-tab", "value"),
         Input("data-table", "derived_virtual_data"),
         Input("data-table", "derived_virtual_selected_rows"),
         Input("client-info-json", "data"),
         Input("synapse-table-resolution-json", "data"),
+        Input("ngl-target-site", "value"),
     )
     def update_link(
         tab_value,
         rows,
         selected_rows,
         info_cache,
         data_resolution,
+        target_site,
     ):
         large_state_text = "State Too Large - Please Filter"
+
         def small_state_text(n):
             return f"Neuroglancer: ({n} partners)"
 
         if info_cache is None:
             return "", "No datastack set", True, ""
 
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if rows is None or len(rows) == 0:
             rows = {}
             sb = generate_statebuilder(info_cache, c)
             return (
                 sb.render_state(None, return_as="url"),
                 small_state_text(0),
                 False,
@@ -345,28 +386,36 @@
         Output("all-input-link", "children"),
         Input("all-input-link-button", "n_clicks"),
         Input("submit-button", "n_clicks"),
         Input("source-table-json", "data"),
         Input("client-info-json", "data"),
         InputDatastack,
         Input("synapse-table-resolution-json", "data"),
+        Input("ngl-target-site", "value"),
         prevent_initial_call=True,
     )
-    def generate_all_input_link(_1, _2, rows, info_cache, datastack, data_resolution):
+    def generate_all_input_link(
+        _1, _2, rows, info_cache, datastack, data_resolution, target_site
+    ):
         ctx = callback_context
         if not ctx.triggered:
             return ""
         trigger_src = ctx.triggered[0]["prop_id"].split(".")[0]
         if (
             trigger_src == "submit-button"
             or trigger_src == "client-info-json"
             or trigger_src == "source-table-json"
         ):
             return ""
 
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if rows is None or len(rows) == 0:
             return html.Div("No inputs to show")
         else:
             syn_df = pd.DataFrame(rows)
             for col in c.syn_pt_position_split:
                 repopulate_list(col, syn_df)
 
@@ -390,28 +439,36 @@
         Output("all-output-link", "children"),
         Input("all-output-link-button", "n_clicks"),
         Input("submit-button", "n_clicks"),
         Input("target-table-json", "data"),
         Input("client-info-json", "data"),
         InputDatastack,
         Input("synapse-table-resolution-json", "data"),
+        Input("ngl-target-site", "value"),
         prevent_initial_call=True,
     )
-    def generate_all_output_link(_1, _2, rows, info_cache, datastack, data_resolution):
+    def generate_all_output_link(
+        _1, _2, rows, info_cache, datastack, data_resolution, target_site
+    ):
         ctx = callback_context
         if not ctx.triggered:
             return ""
         trigger_src = ctx.triggered[0]["prop_id"].split(".")[0]
         if (
             trigger_src == "submit-button"
             or trigger_src == "client-info-json"
             or trigger_src == "target-table-json"
         ):
             return ""
 
+        info_cache["target_site"] = target_site
+        info_cache["viewer_site"] = get_viewer_site_from_target(
+            info_cache.get("viewer_site"), target_site
+        )
+
         if rows is None or len(rows) == 0:
             return html.Div("No outputs to show")
         else:
             syn_df = pd.DataFrame(rows)
             for col in c.syn_pt_position_split:
                 repopulate_list(col, syn_df)
             sb = generate_statebuilder_pre(
@@ -427,8 +484,8 @@
                 )
             except Exception as e:
                 return html.Div(str(e))
         return html.A(
             "All Output Link", href=url, target="_blank", style={"font-size": "20px"}
         )
 
-    pass
+    pass
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/config.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/config.py`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer/connectivity_table/layout.py` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer/connectivity_table/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 url_bar_and_content_div = html.Div(
     [dcc.Location(id="url", refresh=False), html.Div(id="page-layout")]
 )
 
 
 def page_layout(state: State = None):
     state = state or {}
-    
+
     header_row = dbc.Row(
         [
             dbc.Col(
-                html.Div(id='header-bar'),
+                html.Div(id="header-bar"),
                 width={"size": 12},
             ),
         ],
     )
 
-
     input_row = [
         dbc.Row(
             [
                 dbc.Col(
                     [
                         html.Div("Cell ID:"),
                     ],
@@ -51,28 +50,30 @@
                             )
                         ),
                     ],
                     align="start",
                 ),
                 dbc.Col(
                     [
-                        dbc.Checklist(
+                        "Materialization:",
+                        dcc.Dropdown(
                             **create_component_kwargs(
                                 state,
-                                id_inner="live-query-toggle",
-                                options=[
-                                    {"label": "Live Query", "value": 1},
-                                ],
-                                value=[
-                                    1,
-                                ],
-                                switch=True,
+                                id_inner="mat-version",
+                                options=[{"label": "Latest", "value": ""}],
+                                value="",
+                                style={
+                                    "margin-left": "12px",
+                                    "font-size": "12px",
+                                },
+                                clearable=False,
                             )
                         ),
                     ],
+                    width={"size": 1, "offset": 1},
                     align="center",
                 ),
                 dbc.Col(
                     [
                         dbc.Button(
                             id="submit-button",
                             children="Submit",
@@ -229,14 +230,32 @@
                         id="ngl_link",
                         href="",
                         disabled=False,
                     ),
                 ],
             ),
             dbc.Col(
+                html.Div(
+                    [
+                        dcc.Dropdown(
+                            options={
+                                "seunglab": "Seung-lab Neuroglancer (classic)",
+                                "mainline": "Spelunker (experimental)",
+                            },
+                            value="seunglab",
+                            id="ngl-target-site",
+                            clearable=False,
+                        ),
+                    ],
+                    style={"font-size": "13px"},
+                ),
+                align="top",
+                width={"size": 2, "offset": 1},
+            ),
+            dbc.Col(
                 dbc.Button(
                     id="reset-selection",
                     children="Reset Selection",
                     color="warning",
                     size="sm",
                 ),
             ),
```

### Comparing `dash-connectivity-viewer-2.1.0/dash_connectivity_viewer.egg-info/SOURCES.txt` & `dash_connectivity_viewer-2.2.0/dash_connectivity_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash-connectivity-viewer-2.1.0/setup.py` & `dash_connectivity_viewer-2.2.0/setup.py`

 * *Files identical despite different names*

