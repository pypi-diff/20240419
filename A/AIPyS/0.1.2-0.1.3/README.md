# Comparing `tmp/AIPyS-0.1.2.tar.gz` & `tmp/AIPyS-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPyS-0.1.2.tar", last modified: Wed Apr 17 20:07:40 2024, max compression
+gzip compressed data, was "AIPyS-0.1.3.tar", last modified: Fri Apr 19 20:26:59 2024, max compression
```

## Comparing `AIPyS-0.1.2.tar` & `AIPyS-0.1.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.604831 AIPyS-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:39.803697 AIPyS-0.1.2/AIPyS/
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.126187 AIPyS-0.1.2/AIPyS/CLI/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/CLI/__init__.py
--rw-rw-rw-   0        0        0     7565 2024-04-17 18:09:04.000000 AIPyS-0.1.2/AIPyS/CLI/aipys.py
--rw-rw-rw-   0        0        0     1284 2024-04-15 18:53:26.000000 AIPyS-0.1.2/AIPyS/CLI/area_analysis.py
--rw-rw-rw-   0        0        0     3292 2024-04-16 12:57:00.000000 AIPyS-0.1.2/AIPyS/CLI/loadParameters.py
--rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.1.2/AIPyS/CLI/promptParameters.py
--rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.1.2/AIPyS/CLI/set_parameters.py
--rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.1.2/AIPyS/CLI/test.py
--rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.1.2/AIPyS/DataLoad.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:39.741926 AIPyS-0.1.2/AIPyS/classification/
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.164431 AIPyS-0.1.2/AIPyS/classification/CNN/
--rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.1.2/AIPyS/classification/CNN/CNN_deploy.py
--rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/CNN/Taining_data_orgenizer.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/classification/CNN/__init__.py
--rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/CNN/mapSgRNA.py
--rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/CNN/model_builder.py
--rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/CNN/model_evaluation_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.231641 AIPyS-0.1.2/AIPyS/classification/bayes/
--rw-rw-rw-   0        0        0     2600 2024-04-17 18:29:24.000000 AIPyS-0.1.2/AIPyS/classification/bayes/BayesianModels.py
--rw-rw-rw-   0        0        0     6872 2024-04-17 18:23:38.000000 AIPyS-0.1.2/AIPyS/classification/bayes/Baysian_deploy.py
--rw-rw-rw-   0        0        0     7821 2024-04-17 20:06:15.000000 AIPyS-0.1.2/AIPyS/classification/bayes/Baysian_training.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/bayes/DisplayImageFrame.py
--rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.1.2/AIPyS/classification/bayes/GranulaityMesure.py
--rw-rw-rw-   0        0        0    18111 2024-04-15 19:16:12.000000 AIPyS-0.1.2/AIPyS/classification/bayes/GranularityDataGen.py
--rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/bayes/GranularityDeploy.py
--rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/bayes/RunningWindow.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.2/AIPyS/classification/bayes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.1.2/AIPyS/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:39.745916 AIPyS-0.1.2/AIPyS/segmentation/
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.303148 AIPyS-0.1.2/AIPyS/segmentation/cellpose/
--rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.1.2/AIPyS/segmentation/cellpose/AIPS_cellpose.py
--rw-rw-rw-   0        0        0     1666 2024-04-16 13:55:44.000000 AIPyS-0.1.2/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
--rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.1.2/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/segmentation/cellpose/__init__.py
--rw-rw-rw-   0        0        0     4727 2024-04-15 18:01:11.000000 AIPyS-0.1.2/AIPyS/segmentation/cellpose/plotObjectAreas.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.318529 AIPyS-0.1.2/AIPyS/segmentation/parametric/
--rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/segmentation/parametric/GlobalSeg.py
--rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.1.2/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/segmentation/parametric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.428593 AIPyS-0.1.2/AIPyS/supportFunctions/
--rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_file_display.py
--rw-rw-rw-   0        0        0    12982 2024-04-16 18:37:13.000000 AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_functions.py
--rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_granularity.py
--rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_module.py
--rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_simulate.py
--rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/Display_composit.py
--rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/GranularityFunc.py
--rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/Granularity_cellprofiler.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.1.2/AIPyS/supportFunctions/display_and_xml.py
--rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.1.2/AIPyS/supportFunctions/unpack_h5.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.549190 AIPyS-0.1.2/AIPyS.egg-info/
--rw-rw-rw-   0        0        0     3838 2024-04-17 20:07:39.000000 AIPyS-0.1.2/AIPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2209 2024-04-17 20:07:39.000000 AIPyS-0.1.2/AIPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 20:07:39.000000 AIPyS-0.1.2/AIPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-17 20:07:39.000000 AIPyS-0.1.2/AIPyS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      338 2024-04-17 20:07:39.000000 AIPyS-0.1.2/AIPyS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 20:07:39.000000 AIPyS-0.1.2/AIPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3838 2024-04-17 20:07:40.601839 AIPyS-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 20:07:40.605829 AIPyS-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1405 2024-04-17 20:07:32.000000 AIPyS-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:39.753892 AIPyS-0.1.2/web_app/
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.444797 AIPyS-0.1.2/web_app/AreasViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/web_app/AreasViz/__init__.py
--rw-rw-rw-   0        0        0     4059 2024-04-15 18:20:48.000000 AIPyS-0.1.2/web_app/AreasViz/app.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.474256 AIPyS-0.1.2/web_app/Image_labeling/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/web_app/Image_labeling/__init__.py
--rw-rw-rw-   0        0        0     6622 2024-04-11 19:13:34.000000 AIPyS-0.1.2/web_app/Image_labeling/app.py
--rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.1.2/web_app/Image_labeling/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.505817 AIPyS-0.1.2/web_app/TableViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/web_app/TableViz/__init__.py
--rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.1.2/web_app/TableViz/app.py
--rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.1.2/web_app/TableViz/distplot.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:07:40.544048 AIPyS-0.1.2/web_app/measure_length/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.2/web_app/measure_length/__init__.py
--rw-rw-rw-   0        0        0     4589 2024-04-16 18:40:03.000000 AIPyS-0.1.2/web_app/measure_length/app.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:59.048456 AIPyS-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.349150 AIPyS-0.1.3/AIPyS/
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.641764 AIPyS-0.1.3/AIPyS/CLI/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/CLI/__init__.py
+-rw-rw-rw-   0        0        0     7565 2024-04-17 18:09:04.000000 AIPyS-0.1.3/AIPyS/CLI/aipys.py
+-rw-rw-rw-   0        0        0     1284 2024-04-15 18:53:26.000000 AIPyS-0.1.3/AIPyS/CLI/area_analysis.py
+-rw-rw-rw-   0        0        0     3292 2024-04-16 12:57:00.000000 AIPyS-0.1.3/AIPyS/CLI/loadParameters.py
+-rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.1.3/AIPyS/CLI/promptParameters.py
+-rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.1.3/AIPyS/CLI/set_parameters.py
+-rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.1.3/AIPyS/CLI/test.py
+-rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.1.3/AIPyS/DataLoad.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.307752 AIPyS-0.1.3/AIPyS/classification/
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.698149 AIPyS-0.1.3/AIPyS/classification/CNN/
+-rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.1.3/AIPyS/classification/CNN/CNN_deploy.py
+-rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/CNN/Taining_data_orgenizer.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/classification/CNN/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/CNN/mapSgRNA.py
+-rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/CNN/model_builder.py
+-rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/CNN/model_evaluation_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.745192 AIPyS-0.1.3/AIPyS/classification/bayes/
+-rw-rw-rw-   0        0        0     2600 2024-04-17 18:29:24.000000 AIPyS-0.1.3/AIPyS/classification/bayes/BayesianModels.py
+-rw-rw-rw-   0        0        0     6872 2024-04-17 18:23:38.000000 AIPyS-0.1.3/AIPyS/classification/bayes/Baysian_deploy.py
+-rw-rw-rw-   0        0        0     7821 2024-04-17 20:06:15.000000 AIPyS-0.1.3/AIPyS/classification/bayes/Baysian_training.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/bayes/DisplayImageFrame.py
+-rw-rw-rw-   0        0        0     6173 2024-04-19 11:50:19.000000 AIPyS-0.1.3/AIPyS/classification/bayes/GranulaityMesure.py
+-rw-rw-rw-   0        0        0    18111 2024-04-15 19:16:12.000000 AIPyS-0.1.3/AIPyS/classification/bayes/GranularityDataGen.py
+-rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/bayes/GranularityDeploy.py
+-rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/bayes/RunningWindow.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.1.3/AIPyS/classification/bayes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.1.3/AIPyS/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.309748 AIPyS-0.1.3/AIPyS/segmentation/
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.804131 AIPyS-0.1.3/AIPyS/segmentation/cellpose/
+-rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.1.3/AIPyS/segmentation/cellpose/AIPS_cellpose.py
+-rw-rw-rw-   0        0        0     1666 2024-04-16 13:55:44.000000 AIPyS-0.1.3/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
+-rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.1.3/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/segmentation/cellpose/__init__.py
+-rw-rw-rw-   0        0        0     4727 2024-04-15 18:01:11.000000 AIPyS-0.1.3/AIPyS/segmentation/cellpose/plotObjectAreas.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.812815 AIPyS-0.1.3/AIPyS/segmentation/parametric/
+-rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/segmentation/parametric/GlobalSeg.py
+-rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.1.3/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/segmentation/parametric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.880501 AIPyS-0.1.3/AIPyS/supportFunctions/
+-rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_file_display.py
+-rw-rw-rw-   0        0        0    12982 2024-04-16 18:37:13.000000 AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_functions.py
+-rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_granularity.py
+-rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_module.py
+-rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_simulate.py
+-rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/Display_composit.py
+-rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/GranularityFunc.py
+-rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/Granularity_cellprofiler.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.1.3/AIPyS/supportFunctions/display_and_xml.py
+-rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.1.3/AIPyS/supportFunctions/unpack_h5.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:59.003202 AIPyS-0.1.3/AIPyS.egg-info/
+-rw-rw-rw-   0        0        0     3838 2024-04-19 20:26:57.000000 AIPyS-0.1.3/AIPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2024-04-19 20:26:58.000000 AIPyS-0.1.3/AIPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 20:26:57.000000 AIPyS-0.1.3/AIPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-19 20:26:57.000000 AIPyS-0.1.3/AIPyS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      338 2024-04-19 20:26:58.000000 AIPyS-0.1.3/AIPyS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 20:26:58.000000 AIPyS-0.1.3/AIPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3838 2024-04-19 20:26:59.046862 AIPyS-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-19 20:26:59.048456 AIPyS-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2024-04-19 20:24:08.000000 AIPyS-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.312738 AIPyS-0.1.3/web_app/
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.903437 AIPyS-0.1.3/web_app/AreasViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/web_app/AreasViz/__init__.py
+-rw-rw-rw-   0        0        0     4059 2024-04-15 18:20:48.000000 AIPyS-0.1.3/web_app/AreasViz/app.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.932654 AIPyS-0.1.3/web_app/Image_labeling/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/web_app/Image_labeling/__init__.py
+-rw-rw-rw-   0        0        0     6622 2024-04-11 19:13:34.000000 AIPyS-0.1.3/web_app/Image_labeling/app.py
+-rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.1.3/web_app/Image_labeling/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.967477 AIPyS-0.1.3/web_app/TableViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/web_app/TableViz/__init__.py
+-rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.1.3/web_app/TableViz/app.py
+-rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.1.3/web_app/TableViz/distplot.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:26:58.998204 AIPyS-0.1.3/web_app/measure_length/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.1.3/web_app/measure_length/__init__.py
+-rw-rw-rw-   0        0        0     4589 2024-04-16 18:40:03.000000 AIPyS-0.1.3/web_app/measure_length/app.py
```

### Comparing `AIPyS-0.1.2/AIPyS/CLI/aipys.py` & `AIPyS-0.1.3/AIPyS/CLI/aipys.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/CLI/area_analysis.py` & `AIPyS-0.1.3/AIPyS/CLI/area_analysis.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/CLI/loadParameters.py` & `AIPyS-0.1.3/AIPyS/CLI/loadParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/CLI/promptParameters.py` & `AIPyS-0.1.3/AIPyS/CLI/promptParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/CLI/set_parameters.py` & `AIPyS-0.1.3/AIPyS/CLI/set_parameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/CLI/test.py` & `AIPyS-0.1.3/AIPyS/CLI/test.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/DataLoad.py` & `AIPyS-0.1.3/AIPyS/DataLoad.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/CNN/CNN_deploy.py` & `AIPyS-0.1.3/AIPyS/classification/CNN/CNN_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/CNN/Taining_data_orgenizer.py` & `AIPyS-0.1.3/AIPyS/classification/CNN/Taining_data_orgenizer.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/CNN/mapSgRNA.py` & `AIPyS-0.1.3/AIPyS/classification/CNN/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/CNN/model_builder.py` & `AIPyS-0.1.3/AIPyS/classification/CNN/model_builder.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/CNN/model_evaluation_utils.py` & `AIPyS-0.1.3/AIPyS/classification/CNN/model_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/bayes/BayesianModels.py` & `AIPyS-0.1.3/AIPyS/classification/bayes/BayesianModels.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/bayes/Baysian_deploy.py` & `AIPyS-0.1.3/AIPyS/classification/bayes/Baysian_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/bayes/Baysian_training.py` & `AIPyS-0.1.3/AIPyS/classification/bayes/Baysian_training.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/bayes/GranulaityMesure.py` & `AIPyS-0.1.3/AIPyS/classification/bayes/GranulaityMesure.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         mask, table = self.cellpose_segmentation(image_input = image)
         # single cell randomly selected:
         img_label = table['label'].sample(n=1).iloc[0]
         stack_img, stack_mask = self.stackObjects_cellpose_ebimage_parametrs_method(image,mask,table,img_label)
         frame_obj = Compsite_display(stack_img, stack_mask, 2)
         frame = resize(image=frame_obj.rgb_out, width=self.outputImageSize, hight=self.outputImageSize)  # resize(image,width,hight)
         video = cv2.VideoWriter(os.path.join(self.outPath,self.videoName), cv2.VideoWriter_fourcc(*'MJPG'),1.0,(self.outputImageSize,self.outputImageSize),  isColor = True)
+        video.write(frame)
         prev_image = stack_img
         print('analysis might take a few minutes')
         for i, opning in enumerate(open_vec):
             openImage_curr = openingOperation(kernel=opning, image=prev_image)
             if np.sum(prev_image[stack_mask > 0]) == 0:
                 denominator = np.sum(prev_image[stack_mask > 0]) + 0.000001
             else:
```

### Comparing `AIPyS-0.1.2/AIPyS/classification/bayes/GranularityDataGen.py` & `AIPyS-0.1.3/AIPyS/classification/bayes/GranularityDataGen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/bayes/GranularityDeploy.py` & `AIPyS-0.1.3/AIPyS/classification/bayes/GranularityDeploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/classification/bayes/RunningWindow.py` & `AIPyS-0.1.3/AIPyS/classification/bayes/RunningWindow.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/segmentation/cellpose/AIPS_cellpose.py` & `AIPyS-0.1.3/AIPyS/segmentation/cellpose/AIPS_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py` & `AIPyS-0.1.3/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/segmentation/cellpose/StackObjects_cellpose.py` & `AIPyS-0.1.3/AIPyS/segmentation/cellpose/StackObjects_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/segmentation/cellpose/plotObjectAreas.py` & `AIPyS-0.1.3/AIPyS/segmentation/cellpose/plotObjectAreas.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/segmentation/parametric/GlobalSeg.py` & `AIPyS-0.1.3/AIPyS/segmentation/parametric/GlobalSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py` & `AIPyS-0.1.3/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_file_display.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_file_display.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_functions.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_functions.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_granularity.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_granularity.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_module.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_module.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/AIPS_simulate.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/AIPS_simulate.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/Display_composit.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/Display_composit.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/GranularityFunc.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/GranularityFunc.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/Granularity_cellprofiler.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/Granularity_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS/supportFunctions/display_and_xml.py` & `AIPyS-0.1.3/AIPyS/supportFunctions/display_and_xml.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/AIPyS.egg-info/PKG-INFO` & `AIPyS-0.1.3/AIPyS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.1.2
+Version: 0.1.3
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.1.2/AIPyS.egg-info/SOURCES.txt` & `AIPyS-0.1.3/AIPyS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/LICENSE` & `AIPyS-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/PKG-INFO` & `AIPyS-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.1.2
+Version: 0.1.3
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.1.2/setup.py` & `AIPyS-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 setup(
     name="AIPyS",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(include=['AIPyS','AIPyS.CLI','AIPyS.classification.bayes','AIPyS.classification.CNN',
                                     'AIPyS.segmentation.cellpose','AIPyS.segmentation.parametric','AIPyS.supportFunctions',
                                     'web_app.Image_labeling','web_app.measure_length','web_app.measure_length','web_app.TableViz', 'web_app.AreasViz',]),
     install_requires=required,
     entry_points={
         'console_scripts': [
            'aipys=AIPyS.CLI.aipys:main',
```

### Comparing `AIPyS-0.1.2/web_app/AreasViz/app.py` & `AIPyS-0.1.3/web_app/AreasViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/web_app/Image_labeling/app.py` & `AIPyS-0.1.3/web_app/Image_labeling/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/web_app/Image_labeling/draft.py` & `AIPyS-0.1.3/web_app/Image_labeling/draft.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/web_app/TableViz/app.py` & `AIPyS-0.1.3/web_app/TableViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/web_app/TableViz/distplot.py` & `AIPyS-0.1.3/web_app/TableViz/distplot.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.1.2/web_app/measure_length/app.py` & `AIPyS-0.1.3/web_app/measure_length/app.py`

 * *Files identical despite different names*

