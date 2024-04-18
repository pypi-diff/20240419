# Comparing `tmp/MobileInventoryCLI-0.4.60.tar.gz` & `tmp/MobileInventoryCLI-0.4.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.60.tar", last modified: Wed Apr 17 20:32:34 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.61.tar", last modified: Thu Apr 18 23:42:02 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.60.tar` & `MobileInventoryCLI-0.4.61.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.409286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.409286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.412620 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.412620 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.412620 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.412620 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   104673 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    16709 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    64732 2024-04-17 20:30:31.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.415953 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-17 20:32:28.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1230 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-16 18:32:40.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-17 20:32:34.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5020 2024-04-17 20:32:34.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-17 20:32:34.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-17 20:32:34.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-17 20:32:34.000000 MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-17 20:32:34.419286 MobileInventoryCLI-0.4.60/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-17 20:32:34.000000 MobileInventoryCLI-0.4.60/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.388585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.388585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.391918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.391918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.391918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   104673 2024-04-18 23:11:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.395252 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    16709 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    67488 2024-04-18 23:41:14.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-18 23:41:57.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1230 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.398585 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-17 20:32:43.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-18 23:42:02.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5020 2024-04-18 23:42:02.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-18 23:42:02.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-18 23:42:02.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-18 23:42:02.000000 MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-18 23:42:02.401918 MobileInventoryCLI-0.4.61/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-18 23:42:02.000000 MobileInventoryCLI-0.4.61/setup.py
```

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
 
 
-    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False):
+    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=1,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote='',userUpdated=False):
         if EntryId:
             self.EntryId=EntryId
         self.CRV=CRV
         self.userUpdated=userUpdated
         self.Tax=Tax
         self.TaxNote=TaxNote
         self.Barcode=Barcode
```

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,31 +194,57 @@
                             break
                         pc.PossibleCodes(scanned=code)
                         pc.PossibleCodesEAN13(scanned=code)
                             
                         value=0
                         def mkT(text,self):
                             try:
-                                return float(eval(text)),text
+                                tmp=text.split(',')
+                                if len(tmp) == 2:
+                                    text,suffix=tmp
+                                    if suffix.lower() not in ['s','e','u',' ','','c']:
+                                        suffix=''
+                                else:
+                                    suffix=''
+                                    for i in ['s','e','u','c']:
+                                        if text.endswith(i):
+                                            suffix=i
+                                            text=text[:-1]
+                                            break
+
+                                return float(eval(text)),text,suffix
                             except Exception as e:
-                                return float(0),text
+                                print(e)
+                                return float(0),text,''
 
                         p=Prompt.__init2__(None,func=mkT,ptext="amount|+amount|-amount",helpText=self.helpText_barcodes,data=self)
                         if p:
-                            value,text=p
+                            value,text,suffix=p
                         else:
                             continue
                         try:
                             color1=Fore.red
                             color2=Fore.yellow
                             color3=Fore.cyan
                             color4=Fore.green_yellow 
                             if text.startswith("-") or text.startswith("+"):
                                 result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code)).first()
                                 if result:
+                                    if suffix.lower() in ['c',]:
+                                        if result.CaseCount in [None,]:
+                                            result.CaseCount=1
+                                            session.commit()
+                                            session.flush()
+                                            session.refresh(result)
+                                        if result.CaseCount < 1:
+                                            result.CaseCount=1
+                                            session.commit()
+                                            session.flush()
+                                            session.refresh(result)
+                                        value=float(value)*result.CaseCount
                                     setattr(result,fieldname,getattr(result,fieldname)+float(value))
                                     result.InList=True
                                     session.commit()
                                     session.flush()
                                     session.refresh(result)
                                     print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
                                     print(f"{m}\n{hr}")
@@ -257,14 +283,26 @@
                                         result=n
                                         print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
 
                                         print(f"{m}\n{hr}")
                             else:
                                 result=session.query(Entry).filter(or_(Entry.Barcode==code,Entry.Code==code)).first()
                                 if result:
+                                    if suffix.lower() in ['c',]:
+                                        if result.CaseCount in [None,]:
+                                            result.CaseCount=1
+                                            session.commit()
+                                            session.flush()
+                                            session.refresh(result)
+                                        if result.CaseCount < 1:
+                                            result.CaseCount=1
+                                            session.commit()
+                                            session.flush()
+                                            session.refresh(result)
+                                        value=float(value)*result.CaseCount
                                     setattr(result,fieldname,value)
                                     result.InList=True
                                     session.commit()
                                     session.flush()
                                     session.refresh(result)
                                     print(f"{Fore.red}0{Style.reset} -> {color1}{result.Name}{Style.reset}|{color2}{result.Barcode}{Style.reset}|{color3}{result.Code}{Style.reset}|{color4}{getattr(result,fieldname)}{Style.reset}|{color4}{getattr(result,'EntryId')}{Style.reset}")
 
@@ -311,16 +349,26 @@
                         except Exception as e:
                             print(e)
             else:
                 #code for tags,caseId[br,6w,ld],
                 self.processSpecial(fieldname)
                 break
     helpText_barcodes=f"""
-    1. Enter the EntryId into the prompt
-    2. if an entry is found you will be prompted for a code to be saved
+1. Enter the EntryId into the prompt
+2. if an entry is found you will be prompted for a code to be saved
+Quantity Modifiers:
+(SEP=',' or No Sep) Suffixes Singles: s|e|u|' '|'' == units/singles/eaches/no multipliers
+(SEP=',' or No Sep) Suffixes CaseCount: c == (qty*casecount+old_value_if_any
+Valid Examples:
++1-2u - do operation in units and remove from qty 
+-1+2c - do operation in cases and remove from qty
+1c - cases set
+1u - units set
+remember, formula is calculated first, then that value is removed from qty if -/+
+if CaseCount is less than 1, or not set, assume casecount == 1
     """
     def setBarcodes(self,fieldname):
          while True:
             try:
                 def mkT(text,self):
                     return text
                 cmd=Prompt.__init2__(None,func=mkT,ptext='Do What[help/q/b/$EntryId]?',helpText=self.helpText_barcodes,data=self)
```

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.60
+Version: 0.4.61
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.60/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.61/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.60/PKG-INFO` & `MobileInventoryCLI-0.4.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.60
+Version: 0.4.61
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.60/setup.py` & `MobileInventoryCLI-0.4.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.60'
+version='0.4.61'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

