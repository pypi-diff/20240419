# Comparing `tmp/talipp-2.2.0.tar.gz` & `tmp/talipp-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talipp-2.2.0.tar", last modified: Fri Apr  5 19:53:11 2024, max compression
+gzip compressed data, was "talipp-2.2.1.tar", last modified: Fri Apr 19 19:55:22 2024, max compression
```

## Comparing `talipp-2.2.0.tar` & `talipp-2.2.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:53:11.593505 talipp-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 19:53:00.000000 talipp-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 19:53:00.000000 talipp-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-05 19:53:11.593505 talipp-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-04-05 19:53:00.000000 talipp-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:53:00.000000 talipp-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:53:11.593505 talipp-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-05 19:53:00.000000 talipp-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:53:11.573505 talipp-2.2.0/talipp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicator_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:53:11.585505 talipp-2.2.0/talipp/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ADX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ALMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/AO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ATR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/AccuDist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/Aroon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/BB.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/BOP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/CCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/CHOP.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ChaikinOsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ChandeKrollStop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/CoppockCurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/DEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/DPO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/DonchianChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/EMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/EMV.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/FibRetracement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ForceIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/HMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/IBS.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/Ichimoku.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/Indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/KAMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/KST.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/KVO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/KeltnerChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/MACD.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/MassIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/McGinleyDynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/MeanDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/OBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ParabolicSAR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/PivotsHL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ROC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/RSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/SFX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/SMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/SMMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/SOBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/STC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/StdDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/Stoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/StochRSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/SuperTrend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/T3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/TEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/TRIX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/TSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/TTM.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/UO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/VTX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/VWAP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/VWMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/WMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/ZLEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/indicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/ma.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-05 19:53:00.000000 talipp-2.2.0/talipp/ohlcv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:53:11.573505 talipp-2.2.0/talipp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-05 19:53:11.000000 talipp-2.2.0/talipp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-05 19:53:11.000000 talipp-2.2.0/talipp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:53:11.000000 talipp-2.2.0/talipp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 19:53:11.000000 talipp-2.2.0/talipp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:53:11.593505 talipp-2.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ADX.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ALMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_AO.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ATR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_AccuDist.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_Aroon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_BB.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_BOP.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_CCI.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_CHOP.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ChaikinOsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ChandeKrollStop.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_CoppockCurve.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_DEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_DPO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_DonchianChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_EMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_EMV.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ForceIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_HMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_IBS.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_KAMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_KST.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_KVO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_KeltnerChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_MACD.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_MassIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_McGinleyDynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_MeanDev.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_OBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_OHLCV.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ParabolicSAR.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ROC.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_RSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_SFX.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_SMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_SMMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_SOBV.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_STC.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_StdDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_Stoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_StochRSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_SuperTrend.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_T3.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_TEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_TRIX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_TSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_TTM.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_UO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_VTX.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_VWAP.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_VWMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_WMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_ZLEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_indicator_chaining.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_indicator_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_indicator_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-05 19:53:00.000000 talipp-2.2.0/test/test_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.209199 talipp-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 19:55:11.000000 talipp-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 19:55:11.000000 talipp-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-19 19:55:22.209199 talipp-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-19 19:55:11.000000 talipp-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:11.000000 talipp-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:55:22.209199 talipp-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-19 19:55:11.000000 talipp-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.193199 talipp-2.2.1/talipp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicator_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.201199 talipp-2.2.1/talipp/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ADX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ALMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/AO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ATR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/AccuDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/BB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/BOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/CCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/CHOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ChaikinOsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ChandeKrollStop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/CoppockCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/DEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/DPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/DonchianChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/EMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/EMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/FibRetracement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ForceIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/HMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/IBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Ichimoku.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KAMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KST.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KVO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KeltnerChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/MACD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/MassIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/McGinleyDynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/MeanDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/OBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ParabolicSAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/PivotsHL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ROC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/RSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SFX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SMMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SOBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/STC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/StdDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/StochRSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SuperTrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/T3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TRIX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/UO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/VTX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/VWAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/VWMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/WMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ZLEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/ma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/ohlcv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.193199 talipp-2.2.1/talipp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-19 19:55:21.000000 talipp-2.2.1/talipp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-19 19:55:22.000000 talipp-2.2.1/talipp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:55:21.000000 talipp-2.2.1/talipp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 19:55:21.000000 talipp-2.2.1/talipp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.209199 talipp-2.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ADX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ALMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_AO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ATR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_AccuDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_Aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_BB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_BOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_CCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_CHOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ChaikinOsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ChandeKrollStop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_CoppockCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_DEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_DPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_DonchianChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_EMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_EMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ForceIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_HMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_IBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KAMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KST.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KVO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KeltnerChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_MACD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_MassIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_McGinleyDynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_MeanDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_OBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_OHLCV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ParabolicSAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ROC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_RSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SFX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SMMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SOBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_STC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_StdDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_Stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_StochRSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SuperTrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_T3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TRIX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_UO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_VTX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_VWAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_VWMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_WMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ZLEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_indicator_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_indicator_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_indicator_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_input.py
```

### Comparing `talipp-2.2.0/LICENSE` & `talipp-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/PKG-INFO` & `talipp-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: talipp
-Version: 2.2.0
+Version: 2.2.1
 Summary: talipp - Incremental Technical Analysis Library
 Home-page: https://github.com/nardew/talipp
 Author: nardew
 Author-email: talipp.pyth@gmail.com
 License: UNKNOWN
 Description: # talipp - Incremental Technical Analysis Library
         
-        ![](https://img.shields.io/badge/python-3.8-blue.svg) 
-        ![](https://img.shields.io/badge/python-3.9-blue.svg)
-        ![](https://img.shields.io/badge/python-3.10-blue.svg)
-        ![](https://img.shields.io/badge/python-3.11-blue.svg)
+        ![python](https://img.shields.io/pypi/pyversions/talipp?logo=python)
         ![PyPy](https://img.shields.io/badge/pypy-3-blue.svg)
         ![unit tests](https://github.com/nardew/talipp/workflows/unit%20tests/badge.svg)
         
         ---
         
         ## !!! [New documentation page available](https://nardew.github.io/talipp) !!!
```

### Comparing `talipp-2.2.0/README.md` & `talipp-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # talipp - Incremental Technical Analysis Library
 
-![](https://img.shields.io/badge/python-3.8-blue.svg) 
-![](https://img.shields.io/badge/python-3.9-blue.svg)
-![](https://img.shields.io/badge/python-3.10-blue.svg)
-![](https://img.shields.io/badge/python-3.11-blue.svg)
+![python](https://img.shields.io/pypi/pyversions/talipp?logo=python)
 ![PyPy](https://img.shields.io/badge/pypy-3-blue.svg)
 ![unit tests](https://github.com/nardew/talipp/workflows/unit%20tests/badge.svg)
 
 ---
 
 ## !!! [New documentation page available](https://nardew.github.io/talipp) !!!
```

### Comparing `talipp-2.2.0/setup.py` & `talipp-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicator_util.py` & `talipp-2.2.1/talipp/indicator_util.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ADX.py` & `talipp-2.2.1/talipp/indicators/ADX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ALMA.py` & `talipp-2.2.1/talipp/indicators/ALMA.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.offset = offset
         self.sigma = sigma
 
         # calculate weights and normalisation factor (w_sum)
         self.w = []
         self.w_sum = 0.0
         s = self.period / float(self.sigma)
-        m = int((self.period - 1) * self.offset)
+        m = (self.period - 1) * self.offset
         for i in range(0, self.period):
             self.w.append(exp(-1 * (i - m) * (i - m) / (2 * s * s)))
             self.w_sum += self.w[-1]
 
         self.initialize(input_values, input_indicator)
 
     def _calculate_new_value(self) -> Any:
```

### Comparing `talipp-2.2.0/talipp/indicators/AO.py` & `talipp-2.2.1/talipp/indicators/AO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ATR.py` & `talipp-2.2.1/talipp/indicators/ATR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/AccuDist.py` & `talipp-2.2.1/talipp/indicators/AccuDist.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/Aroon.py` & `talipp-2.2.1/talipp/indicators/Aroon.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/BB.py` & `talipp-2.2.1/talipp/indicators/BB.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/BOP.py` & `talipp-2.2.1/talipp/indicators/BOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/CCI.py` & `talipp-2.2.1/talipp/indicators/CCI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/CHOP.py` & `talipp-2.2.1/talipp/indicators/CHOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ChaikinOsc.py` & `talipp-2.2.1/talipp/indicators/ChaikinOsc.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ChandeKrollStop.py` & `talipp-2.2.1/talipp/indicators/ChandeKrollStop.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/CoppockCurve.py` & `talipp-2.2.1/talipp/indicators/CoppockCurve.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/DEMA.py` & `talipp-2.2.1/talipp/indicators/DEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/DPO.py` & `talipp-2.2.1/talipp/indicators/DPO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/DonchianChannels.py` & `talipp-2.2.1/talipp/indicators/DonchianChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/EMA.py` & `talipp-2.2.1/talipp/indicators/EMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/EMV.py` & `talipp-2.2.1/talipp/indicators/EMV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ForceIndex.py` & `talipp-2.2.1/talipp/indicators/ForceIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/HMA.py` & `talipp-2.2.1/talipp/indicators/HMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/IBS.py` & `talipp-2.2.1/talipp/indicators/IBS.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from talipp.input import SamplingPeriodType
 from talipp.ohlcv import OHLCV
 
 
 class IBS(Indicator):
     """Internal Bar Strength.
 
-    Input type: [OHLCV][talipp.ohlcv.OHLCV]`
+    Input type: [OHLCV][talipp.ohlcv.OHLCV]
 
     Output type: `float`
 
     Args:
         input_values: List of input values.
         input_indicator: Input indicator.
         input_modifier: Input modifier.
```

### Comparing `talipp-2.2.0/talipp/indicators/Ichimoku.py` & `talipp-2.2.1/talipp/indicators/Ichimoku.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/Indicator.py` & `talipp-2.2.1/talipp/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/KAMA.py` & `talipp-2.2.1/talipp/indicators/KAMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/KST.py` & `talipp-2.2.1/talipp/indicators/KST.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/KVO.py` & `talipp-2.2.1/talipp/indicators/KVO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/KeltnerChannels.py` & `talipp-2.2.1/talipp/indicators/KeltnerChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/MACD.py` & `talipp-2.2.1/talipp/indicators/MACD.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/MassIndex.py` & `talipp-2.2.1/talipp/indicators/MassIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/McGinleyDynamic.py` & `talipp-2.2.1/talipp/indicators/McGinleyDynamic.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/MeanDev.py` & `talipp-2.2.1/talipp/indicators/MeanDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/OBV.py` & `talipp-2.2.1/talipp/indicators/OBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ParabolicSAR.py` & `talipp-2.2.1/talipp/indicators/ParabolicSAR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/PivotsHL.py` & `talipp-2.2.1/talipp/indicators/PivotsHL.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ROC.py` & `talipp-2.2.1/talipp/indicators/ROC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/RSI.py` & `talipp-2.2.1/talipp/indicators/RSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/SFX.py` & `talipp-2.2.1/talipp/indicators/SFX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/SMA.py` & `talipp-2.2.1/talipp/indicators/SMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/SMMA.py` & `talipp-2.2.1/talipp/indicators/SMMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/SOBV.py` & `talipp-2.2.1/talipp/indicators/SOBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/STC.py` & `talipp-2.2.1/talipp/indicators/STC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/StdDev.py` & `talipp-2.2.1/talipp/indicators/StdDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/Stoch.py` & `talipp-2.2.1/talipp/indicators/Stoch.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/StochRSI.py` & `talipp-2.2.1/talipp/indicators/StochRSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/SuperTrend.py` & `talipp-2.2.1/talipp/indicators/SuperTrend.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/T3.py` & `talipp-2.2.1/talipp/indicators/T3.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/TEMA.py` & `talipp-2.2.1/talipp/indicators/TEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/TRIX.py` & `talipp-2.2.1/talipp/indicators/TRIX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/TSI.py` & `talipp-2.2.1/talipp/indicators/TSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/TTM.py` & `talipp-2.2.1/talipp/indicators/TTM.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/UO.py` & `talipp-2.2.1/talipp/indicators/UO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/VTX.py` & `talipp-2.2.1/talipp/indicators/VTX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/VWAP.py` & `talipp-2.2.1/talipp/indicators/VWAP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/VWMA.py` & `talipp-2.2.1/talipp/indicators/VWMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/WMA.py` & `talipp-2.2.1/talipp/indicators/WMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/ZLEMA.py` & `talipp-2.2.1/talipp/indicators/ZLEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/indicators/__init__.py` & `talipp-2.2.1/talipp/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/input.py` & `talipp-2.2.1/talipp/input.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/ma.py` & `talipp-2.2.1/talipp/ma.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp/ohlcv.py` & `talipp-2.2.1/talipp/ohlcv.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/talipp.egg-info/PKG-INFO` & `talipp-2.2.1/talipp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: talipp
-Version: 2.2.0
+Version: 2.2.1
 Summary: talipp - Incremental Technical Analysis Library
 Home-page: https://github.com/nardew/talipp
 Author: nardew
 Author-email: talipp.pyth@gmail.com
 License: UNKNOWN
 Description: # talipp - Incremental Technical Analysis Library
         
-        ![](https://img.shields.io/badge/python-3.8-blue.svg) 
-        ![](https://img.shields.io/badge/python-3.9-blue.svg)
-        ![](https://img.shields.io/badge/python-3.10-blue.svg)
-        ![](https://img.shields.io/badge/python-3.11-blue.svg)
+        ![python](https://img.shields.io/pypi/pyversions/talipp?logo=python)
         ![PyPy](https://img.shields.io/badge/pypy-3-blue.svg)
         ![unit tests](https://github.com/nardew/talipp/workflows/unit%20tests/badge.svg)
         
         ---
         
         ## !!! [New documentation page available](https://nardew.github.io/talipp) !!!
```

### Comparing `talipp-2.2.0/talipp.egg-info/SOURCES.txt` & `talipp-2.2.1/talipp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ADX.py` & `talipp-2.2.1/test/test_ADX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ALMA.py` & `talipp-2.2.1/test/test_ALMA.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
         self.input_values = list(TalippTest.CLOSE_TMPL)
 
     def test_init(self):
         ind = ALMA(9, 0.85, 6, self.input_values)
 
         print(ind)
 
-        self.assertAlmostEqual(ind[-3], 9.795859, places = 5)
-        self.assertAlmostEqual(ind[-2], 10.121439, places = 5)
-        self.assertAlmostEqual(ind[-1], 10.257038, places = 5)
+        self.assertAlmostEqual(ind[-3], 10.053326, places = 5)
+        self.assertAlmostEqual(ind[-2], 10.267585, places = 5)
+        self.assertAlmostEqual(ind[-1], 10.264363, places = 5)
 
     def test_update(self):
         self.assertIndicatorUpdate(ALMA(9, 0.85, 6, self.input_values))
 
     def test_delete(self):
         self.assertIndicatorDelete(ALMA(9, 0.85, 6, self.input_values))
```

### Comparing `talipp-2.2.0/test/test_AO.py` & `talipp-2.2.1/test/test_AO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ATR.py` & `talipp-2.2.1/test/test_ATR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_AccuDist.py` & `talipp-2.2.1/test/test_AccuDist.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_Aroon.py` & `talipp-2.2.1/test/test_Aroon.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_BB.py` & `talipp-2.2.1/test/test_BB.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_BOP.py` & `talipp-2.2.1/test/test_BOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_CCI.py` & `talipp-2.2.1/test/test_CCI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_CHOP.py` & `talipp-2.2.1/test/test_CHOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ChaikinOsc.py` & `talipp-2.2.1/test/test_ChaikinOsc.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ChandeKrollStop.py` & `talipp-2.2.1/test/test_ChandeKrollStop.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_CoppockCurve.py` & `talipp-2.2.1/test/test_CoppockCurve.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_DEMA.py` & `talipp-2.2.1/test/test_DEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_DPO.py` & `talipp-2.2.1/test/test_DPO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_DonchianChannels.py` & `talipp-2.2.1/test/test_DonchianChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_EMA.py` & `talipp-2.2.1/test/test_EMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_EMV.py` & `talipp-2.2.1/test/test_EMV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ForceIndex.py` & `talipp-2.2.1/test/test_ForceIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_HMA.py` & `talipp-2.2.1/test/test_HMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_IBS.py` & `talipp-2.2.1/test/test_IBS.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_KAMA.py` & `talipp-2.2.1/test/test_KAMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_KST.py` & `talipp-2.2.1/test/test_KST.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_KVO.py` & `talipp-2.2.1/test/test_KVO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_KeltnerChannels.py` & `talipp-2.2.1/test/test_KeltnerChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_MACD.py` & `talipp-2.2.1/test/test_MACD.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_MassIndex.py` & `talipp-2.2.1/test/test_MassIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_McGinleyDynamic.py` & `talipp-2.2.1/test/test_McGinleyDynamic.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_MeanDev.py` & `talipp-2.2.1/test/test_MeanDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_OBV.py` & `talipp-2.2.1/test/test_OBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_OHLCV.py` & `talipp-2.2.1/test/test_OHLCV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ParabolicSAR.py` & `talipp-2.2.1/test/test_ParabolicSAR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ROC.py` & `talipp-2.2.1/test/test_ROC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_RSI.py` & `talipp-2.2.1/test/test_RSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_SFX.py` & `talipp-2.2.1/test/test_SFX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_SMA.py` & `talipp-2.2.1/test/test_SMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_SMMA.py` & `talipp-2.2.1/test/test_SMMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_SOBV.py` & `talipp-2.2.1/test/test_SOBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_STC.py` & `talipp-2.2.1/test/test_STC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_StdDev.py` & `talipp-2.2.1/test/test_StdDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_Stoch.py` & `talipp-2.2.1/test/test_Stoch.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_StochRSI.py` & `talipp-2.2.1/test/test_StochRSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_SuperTrend.py` & `talipp-2.2.1/test/test_SuperTrend.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_T3.py` & `talipp-2.2.1/test/test_T3.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_TEMA.py` & `talipp-2.2.1/test/test_TEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_TRIX.py` & `talipp-2.2.1/test/test_TRIX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_TSI.py` & `talipp-2.2.1/test/test_TSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_TTM.py` & `talipp-2.2.1/test/test_TTM.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_UO.py` & `talipp-2.2.1/test/test_UO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_VTX.py` & `talipp-2.2.1/test/test_VTX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_VWAP.py` & `talipp-2.2.1/test/test_VWAP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_VWMA.py` & `talipp-2.2.1/test/test_VWMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_WMA.py` & `talipp-2.2.1/test/test_WMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_ZLEMA.py` & `talipp-2.2.1/test/test_ZLEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_indicator_chaining.py` & `talipp-2.2.1/test/test_indicator_chaining.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_indicator_sampling.py` & `talipp-2.2.1/test/test_indicator_sampling.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_indicator_util.py` & `talipp-2.2.1/test/test_indicator_util.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.0/test/test_input.py` & `talipp-2.2.1/test/test_input.py`

 * *Files identical despite different names*

