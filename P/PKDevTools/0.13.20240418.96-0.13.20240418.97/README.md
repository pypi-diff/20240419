# Comparing `tmp/PKDevTools-0.13.20240418.96.tar.gz` & `tmp/PKDevTools-0.13.20240418.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240418.96.tar", last modified: Thu Apr 18 14:10:37 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240418.97.tar", last modified: Thu Apr 18 18:40:15 2024, max compression
```

## Comparing `PKDevTools-0.13.20240418.96.tar` & `PKDevTools-0.13.20240418.97.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/
--rw-rw-rw-   0        0        0     1086 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.678598 PKDevTools-0.13.20240418.96/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     4831 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6380 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     8048 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       27 2024-04-18 14:10:33.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:10:37.678598 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-18 14:10:32.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-18 14:10:37.000000 PKDevTools-0.13.20240418.96/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5202 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/README.md
--rw-rw-rw-   0        0        0       86 2024-04-18 14:10:37.694214 PKDevTools-0.13.20240418.96/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-18 14:09:35.000000 PKDevTools-0.13.20240418.96/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:40:15.943306 PKDevTools-0.13.20240418.97/
+-rw-rw-rw-   0        0        0     1086 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-18 18:40:15.927685 PKDevTools-0.13.20240418.97/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:40:15.943306 PKDevTools-0.13.20240418.97/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5007 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6380 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     8048 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       27 2024-04-18 18:40:09.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:40:15.927685 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5202 2024-04-18 18:40:15.000000 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-04-18 18:40:15.000000 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:40:15.000000 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-18 18:40:15.000000 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 18:40:08.000000 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-04-18 18:40:15.000000 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 18:40:15.000000 PKDevTools-0.13.20240418.97/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5202 2024-04-18 18:40:15.943306 PKDevTools-0.13.20240418.97/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-18 18:40:15.943306 PKDevTools-0.13.20240418.97/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-18 18:39:22.000000 PKDevTools-0.13.20240418.97/setup.py
```

### Comparing `PKDevTools-0.13.20240418.96/LICENSE` & `PKDevTools-0.13.20240418.97/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/__init__.py` & `PKDevTools-0.13.20240418.97/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/ColorText.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,23 +69,25 @@
         maxIndex = len(brandName) -1
         col_index = 0
         tab_lines_org = tabulated_data.splitlines()
         tab_lines_mod = []
         highlightRows = len(highlightedRows) >= 1
         highlightColumns = len(highlightedColumns) >= 1
         row_num = 0
+        findCellEnding1 = "--" if highlightCharacter=="\U0001F911" else "-"
+        findCellEnding2 = "==" if highlightCharacter=="\U0001F911" else "="
         for line in tab_lines_org:
             tab_line = line
             col_num = 0
             if line.startswith("+"):
                 tab_line = ""
                 columns = line.split("+")[1:]
                 for col in columns:
                     if highlightRows and highlightColumns and (row_num in highlightedRows) and (col_num in highlightedColumns):
-                        highlightValue = col.replace('--',highlightCharacter).replace('==',highlightCharacter)
+                        highlightValue = col.replace(findCellEnding1,highlightCharacter).replace(findCellEnding2,highlightCharacter)
                         tab_line = f"{tab_line}{brandName[col_index:col_index+1]}{highlightValue}"
                     else:
                         tab_line = f"{tab_line}{brandName[col_index:col_index+1]}{col}"
                     col_index += 1
                     if col_index > maxIndex:
                         col_index = 0
                     col_num += 1
```

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240418.97/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240418.97/PKDevTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240418.96
+Version: 0.13.20240418.97
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.96.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.97.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240418.96/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240418.97/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/PKG-INFO` & `PKDevTools-0.13.20240418.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240418.96
+Version: 0.13.20240418.97
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.96.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240418.97.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240418.96/README.md` & `PKDevTools-0.13.20240418.97/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240418.96/setup.py` & `PKDevTools-0.13.20240418.97/setup.py`

 * *Files identical despite different names*

