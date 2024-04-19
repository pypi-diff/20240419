# Comparing `tmp/PyLLSM5DTools-1.0.3.tar.gz` & `tmp/pyllsm5dtools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLLSM5DTools-1.0.3.tar", last modified: Wed Apr 10 02:04:58 2024, max compression
+gzip compressed data, was "pyllsm5dtools-1.0.4.tar", last modified: Fri Apr 19 06:32:15 2024, max compression
```

## Comparing `PyLLSM5DTools-1.0.3.tar` & `pyllsm5dtools-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/
--rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 PyLLSM5DTools-1.0.3/LICENSE.txt
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-10 02:04:58.756821 PyLLSM5DTools-1.0.3/PyLLSM5DTools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2885 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_MIP_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_crop_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_decon_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6542 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2782 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_resample_dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-10 01:58:39.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/generatePythonWrapper.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools/generate_config_file.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-10 02:04:58.000000 PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 PyLLSM5DTools-1.0.3/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-10 02:04:58.760821 PyLLSM5DTools-1.0.3/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-10 01:59:56.000000 PyLLSM5DTools-1.0.3/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      819 2024-03-05 21:34:03.000000 pyllsm5dtools-1.0.4/LICENSE.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/PyLLSM5DTools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3463 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_FSC_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2885 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_MIP_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3130 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_crop_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6463 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_decon_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5031 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2640 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6542 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_matlab_stitching_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8046 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3179 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3055 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3219 2024-04-19 06:26:41.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_resample_dataset.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3313 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_tiffToZarr_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2062 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_zarrToTiff_wrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      957 2024-04-19 06:26:42.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8944 2024-04-05 00:37:52.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/generatePythonWrapper.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1122 2024-03-27 21:30:52.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools/generate_config_file.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)      414 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      879 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       14 2024-04-19 06:32:15.000000 pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1206 2024-03-27 20:42:06.000000 pyllsm5dtools-1.0.4/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-19 06:32:15.899747 pyllsm5dtools-1.0.4/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3638 2024-04-19 06:30:57.000000 pyllsm5dtools-1.0.4/setup.py
```

### Comparing `PyLLSM5DTools-1.0.3/LICENSE.txt` & `pyllsm5dtools-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_FSC_analysis_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_FSC_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_MIP_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_MIP_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_crop_dataset.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_decon_data_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_decon_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_deskew_rotate_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_fftSpectrumComputingWrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_matlab_stitching_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_matlab_stitching_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_microscopeAutomaticProcessing.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_analysis_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_psf_detection_and_analysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_resample_dataset.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_resample_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import os
 import subprocess
 
 
-def XR_resample_dataset(dataPath, resultPath, rsfactor, **kwargs):
+def XR_resample_dataset(dataPaths, rsfactor, **kwargs):
     function_name = "XR_resample_dataset"
     XR_resample_dataset_dict = {
+        "outDirStr": [kwargs.get("outDirStr", "resampled"), "char"],
+        "ChannelPatterns": [kwargs.get("ChannelPatterns", ['CamA_ch0','CamA_ch1','CamB_ch0','CamB_ch1']), "cell"],
+        "bbox": [kwargs.get("bbox", []), "numericScalar"],
         "Interp": [kwargs.get("Interp", "linear"), "char"],
         "Save16bit": [kwargs.get("Save16bit", True), "logical"],
         "zarrFile": [kwargs.get("zarrFile", False), "logical"],
+        "largeZarr": [kwargs.get("largeZarr", False), "logical"],
         "saveZarr": [kwargs.get("saveZarr", False), "logical"],
+        "blockSize": [kwargs.get("blockSize", [256,256,256]), "numericArr"],
+        "batchSize": [kwargs.get("batchSize", [512,512,512]), "numericArr"],
+        "BorderSize": [kwargs.get("BorderSize", [5,5,5]), "numericArr"],
         "parseCluster": [kwargs.get("parseCluster", False), "logical"],
         "jobLogDir": [kwargs.get("jobLogDir", "../job_logs"), "char"],
         "masterCompute": [kwargs.get("masterCompute", True), "logical"],
         "cpusPerTask": [kwargs.get("cpusPerTask", 2), "numericScalar"],
         "uuid": [kwargs.get("uuid", ""), "char"],
         "mccMode": [kwargs.get("mccMode", False), "logical"],
         "ConfigFile": [kwargs.get("ConfigFile", ""), "char"]
     }
 
     mccMasterLoc = f"{os.path.dirname(os.path.abspath(__file__))}/LLSM5DTools/mcc/linux/run_mccMaster.sh"
     matlabRuntimeLoc = f"{os.path.dirname(os.path.abspath(__file__))}/MATLAB_Runtime/R2023a"
-    dataPathString = "{" + ",".join(f"'{item}'" for item in dataPath) + "}"
-    resultPathString = "{" + ",".join(f"'{item}'" for item in resultPath) + "}"
+    dataPathsString = "{" + ",".join(f"'{item}'" for item in dataPaths) + "}"
     rsfactorString = "[" + ",".join(str(item) for item in rsfactor) + "]"
-    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPath}\" \"{resultPath}\" \"{rsfactorString}\" "
+    cmdString = f"\"{mccMasterLoc}\" \"{matlabRuntimeLoc}\" {function_name} \"{dataPathsString}\" \"{rsfactorString}\" "
     
     for key, value in XR_resample_dataset_dict.items():
         if value[1] == "char":
             if not value[0]:
                 continue
             cmdString += f"\"{key}\" \"{value[0]}\" "
         elif value[1] == "cell":
```

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_tiffToZarr_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_tiffToZarr_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_visualize_OTF_mask_segmentation.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/XR_zarrToTiff_wrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/XR_zarrToTiff_wrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/__init__.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/generatePythonWrapper.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/generatePythonWrapper.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools/generate_config_file.py` & `pyllsm5dtools-1.0.4/PyLLSM5DTools/generate_config_file.py`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/PyLLSM5DTools.egg-info/SOURCES.txt` & `pyllsm5dtools-1.0.4/PyLLSM5DTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/README.md` & `pyllsm5dtools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PyLLSM5DTools-1.0.3/setup.py` & `pyllsm5dtools-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 matlab_runtime_url = ("https://ssd.mathworks.com/supportfiles/downloads/R2023a/Release/6/deployment_files"
                       "/installer/complete/glnxa64/MATLAB_Runtime_R2023a_Update_6_glnxa64.zip")
 name = 'PyLLSM5DTools'
-version = '1.0.3'
+version = '1.0.4'
 
 
 class CustomInstall(install):
     def download_and_extract_matlab_runtime(self, install_dir):
         llsm5dtools_url = "https://github.com/abcucberkeley/LLSM5DTools/archive/refs/heads/main.zip"
         llsm5dtools_github_dir = os.path.join(install_dir, "LLSM5DTools-main")
         llsm5dtools_dir = os.path.join(install_dir, "LLSM5DTools")
```

