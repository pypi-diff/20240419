# Comparing `tmp/RsCMPX_UwbMeas-4.0.80.tar.gz` & `tmp/RsCMPX_UwbMeas-5.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_UwbMeas-4.0.80.tar", last modified: Tue Dec 20 09:29:19 2022, max compression
+gzip compressed data, was "dist\RsCMPX_UwbMeas-5.0.20.tar", last modified: Fri Apr 19 08:52:32 2024, max compression
```

## Comparing `RsCMPX_UwbMeas-4.0.80.tar` & `RsCMPX_UwbMeas-5.0.20.tar`

### file list

```diff
@@ -1,472 +1,512 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.706301 RsCMPX_UwbMeas-4.0.80/
--rw-rw-rw-   0        0        0     3136 2022-12-20 09:29:19.704349 RsCMPX_UwbMeas-4.0.80/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.728048 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.752449 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/
--rw-rw-rw-   0        0        0       90 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3727 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4916 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    21638 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.754401 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.759280 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/
--rw-rw-rw-   0        0        0      875 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/UwbMeas.py
--rw-rw-rw-   0        0        0     1033 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.761233 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.763185 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.777824 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.780753 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.797344 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/
--rw-rw-rw-   0        0        0     2225 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/CcError.py
--rw-rw-rw-   0        0        0     2241 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Foffset.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.802225 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/
--rw-rw-rw-   0        0        0     2232 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/Nrmse.py
--rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/__init__.py
--rw-rw-rw-   0        0        0     2313 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Plevel.py
--rw-rw-rw-   0        0        0     2251 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/PmlWidth.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.807108 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/
--rw-rw-rw-   0        0        0     2240 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/Nrmse.py
--rw-rw-rw-   0        0        0     1012 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.812961 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/
--rw-rw-rw-   0        0        0     2232 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/Nrmse.py
--rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/__init__.py
--rw-rw-rw-   0        0        0     2223 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SlPeak.py
--rw-rw-rw-   0        0        0     2289 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SmAccuracy.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.816864 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/
--rw-rw-rw-   0        0        0     2232 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/Nrmse.py
--rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/__init__.py
--rw-rw-rw-   0        0        0     3125 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/__init__.py
--rw-rw-rw-   0        0        0     1040 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py
--rw-rw-rw-   0        0        0      850 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.818817 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.823698 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/
--rw-rw-rw-   0        0        0     2261 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Area.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.828578 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/
--rw-rw-rw-   0        0        0     3111 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/Area.py
--rw-rw-rw-   0        0        0     1009 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.832480 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/
--rw-rw-rw-   0        0        0     3153 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/Area.py
--rw-rw-rw-   0        0        0     1009 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py
--rw-rw-rw-   0        0        0     1463 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/__init__.py
--rw-rw-rw-   0        0        0     1013 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/__init__.py
--rw-rw-rw-   0        0        0     1267 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Ppdu.py
--rw-rw-rw-   0        0        0      850 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu.py
--rw-rw-rw-   0        0        0     4401 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py
--rw-rw-rw-   0        0        0     2896 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Spectrum.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.834433 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.840289 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/
--rw-rw-rw-   0        0        0     3972 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py
--rw-rw-rw-   0        0        0     1007 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py
--rw-rw-rw-   0        0        0    21130 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.842241 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.847120 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/
--rw-rw-rw-   0        0        0     2068 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/Range.py
--rw-rw-rw-   0        0        0     2104 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/__init__.py
--rw-rw-rw-   0        0        0     5615 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py
--rw-rw-rw-   0        0        0     1321 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py
--rw-rw-rw-   0        0        0     1044 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.850048 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.854930 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/
--rw-rw-rw-   0        0        0     1388 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py
--rw-rw-rw-   0        0        0     2015 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/__init__.py
--rw-rw-rw-   0        0        0     1023 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.857857 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.859809 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.864689 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/
--rw-rw-rw-   0        0        0     1025 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     7676 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1051 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/__init__.py
--rw-rw-rw-   0        0        0     1033 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.866640 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.868592 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.879329 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/
--rw-rw-rw-   0        0        0     2280 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Clength.py
--rw-rw-rw-   0        0        0     2562 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Content.py
--rw-rw-rw-   0        0        0     2506 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/RsParity.py
--rw-rw-rw-   0        0        0     1543 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.893969 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/
--rw-rw-rw-   0        0        0     5265 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Average.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.906659 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/
--rw-rw-rw-   0        0        0     3148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Average.py
--rw-rw-rw-   0        0        0     4468 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Current.py
--rw-rw-rw-   0        0        0     3148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Extreme.py
--rw-rw-rw-   0        0        0     3190 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/StandardDev.py
--rw-rw-rw-   0        0        0     1804 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.919346 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/
--rw-rw-rw-   0        0        0     2148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Average.py
--rw-rw-rw-   0        0        0     3422 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Current.py
--rw-rw-rw-   0        0        0     2148 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Extreme.py
--rw-rw-rw-   0        0        0     2180 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/StandardDev.py
--rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.931057 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/
--rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Average.py
--rw-rw-rw-   0        0        0     3574 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Current.py
--rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Extreme.py
--rw-rw-rw-   0        0        0     2332 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/StandardDev.py
--rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.945697 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/
--rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Average.py
--rw-rw-rw-   0        0        0     3472 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Current.py
--rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Extreme.py
--rw-rw-rw-   0        0        0     2230 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/StandardDev.py
--rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/__init__.py
--rw-rw-rw-   0        0        0     6538 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Current.py
--rw-rw-rw-   0        0        0     5265 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Extreme.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.958385 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/
--rw-rw-rw-   0        0        0     3235 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Average.py
--rw-rw-rw-   0        0        0     4555 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Current.py
--rw-rw-rw-   0        0        0     3235 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Extreme.py
--rw-rw-rw-   0        0        0     3277 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/StandardDev.py
--rw-rw-rw-   0        0        0     1804 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.970097 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/
--rw-rw-rw-   0        0        0     2242 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Average.py
--rw-rw-rw-   0        0        0     3516 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Current.py
--rw-rw-rw-   0        0        0     2242 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Extreme.py
--rw-rw-rw-   0        0        0     2274 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/StandardDev.py
--rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.984737 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/
--rw-rw-rw-   0        0        0     2156 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Average.py
--rw-rw-rw-   0        0        0     3430 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Current.py
--rw-rw-rw-   0        0        0     2156 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Extreme.py
--rw-rw-rw-   0        0        0     2188 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/StandardDev.py
--rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.997424 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/
--rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Average.py
--rw-rw-rw-   0        0        0     3574 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Current.py
--rw-rw-rw-   0        0        0     2300 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Extreme.py
--rw-rw-rw-   0        0        0     2332 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/StandardDev.py
--rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/__init__.py
--rw-rw-rw-   0        0        0     2130 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Otolerance.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.000352 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.011089 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/
--rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Average.py
--rw-rw-rw-   0        0        0     4527 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Current.py
--rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Extreme.py
--rw-rw-rw-   0        0        0     3248 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/StandardDev.py
--rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.026704 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/
--rw-rw-rw-   0        0        0     2318 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Average.py
--rw-rw-rw-   0        0        0     4638 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Current.py
--rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Maximum.py
--rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Minimum.py
--rw-rw-rw-   0        0        0     3359 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/StandardDev.py
--rw-rw-rw-   0        0        0     2045 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/__init__.py
--rw-rw-rw-   0        0        0     1240 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.042324 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/
--rw-rw-rw-   0        0        0     4288 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Average.py
--rw-rw-rw-   0        0        0     5608 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Current.py
--rw-rw-rw-   0        0        0     4288 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Maximum.py
--rw-rw-rw-   0        0        0     4288 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Minimum.py
--rw-rw-rw-   0        0        0     4330 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/StandardDev.py
--rw-rw-rw-   0        0        0     2043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.055009 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/
--rw-rw-rw-   0        0        0     3115 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Average.py
--rw-rw-rw-   0        0        0     4435 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Current.py
--rw-rw-rw-   0        0        0     3115 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Extreme.py
--rw-rw-rw-   0        0        0     3157 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/StandardDev.py
--rw-rw-rw-   0        0        0     1809 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.057938 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.068673 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/
--rw-rw-rw-   0        0        0     3218 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Average.py
--rw-rw-rw-   0        0        0     4539 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Current.py
--rw-rw-rw-   0        0        0     3218 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Extreme.py
--rw-rw-rw-   0        0        0     3260 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/StandardDev.py
--rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.083313 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/
--rw-rw-rw-   0        0        0     2326 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Average.py
--rw-rw-rw-   0        0        0     4650 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Current.py
--rw-rw-rw-   0        0        0     3329 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Maximum.py
--rw-rw-rw-   0        0        0     3329 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Minimum.py
--rw-rw-rw-   0        0        0     3371 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/StandardDev.py
--rw-rw-rw-   0        0        0     2045 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/__init__.py
--rw-rw-rw-   0        0        0     1245 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.095025 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/
--rw-rw-rw-   0        0        0     2162 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Average.py
--rw-rw-rw-   0        0        0     3436 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Current.py
--rw-rw-rw-   0        0        0     2162 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Extreme.py
--rw-rw-rw-   0        0        0     2194 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/StandardDev.py
--rw-rw-rw-   0        0        0     1803 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.108690 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/
--rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Average.py
--rw-rw-rw-   0        0        0     3432 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Current.py
--rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Extreme.py
--rw-rw-rw-   0        0        0     2190 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/StandardDev.py
--rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.110641 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.118449 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/
--rw-rw-rw-   0        0        0     3761 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Current.py
--rw-rw-rw-   0        0        0     2486 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Extreme.py
--rw-rw-rw-   0        0        0     1300 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/__init__.py
--rw-rw-rw-   0        0        0     1043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.120402 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.136017 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/
--rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Average.py
--rw-rw-rw-   0        0        0     4527 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Current.py
--rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Extreme.py
--rw-rw-rw-   0        0        0     3248 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/StandardDev.py
--rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/__init__.py
--rw-rw-rw-   0        0        0     1004 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.149681 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/
--rw-rw-rw-   0        0        0     3460 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Average.py
--rw-rw-rw-   0        0        0     4780 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Current.py
--rw-rw-rw-   0        0        0     3460 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Extreme.py
--rw-rw-rw-   0        0        0     3502 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/StandardDev.py
--rw-rw-rw-   0        0        0     1799 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.165297 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/
--rw-rw-rw-   0        0        0     3463 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Average.py
--rw-rw-rw-   0        0        0     4783 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Current.py
--rw-rw-rw-   0        0        0     3463 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Extreme.py
--rw-rw-rw-   0        0        0     3505 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/StandardDev.py
--rw-rw-rw-   0        0        0     1819 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.180445 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/
--rw-rw-rw-   0        0        0     2274 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Average.py
--rw-rw-rw-   0        0        0     3548 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Current.py
--rw-rw-rw-   0        0        0     2274 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Extreme.py
--rw-rw-rw-   0        0        0     2306 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/StandardDev.py
--rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.194109 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/
--rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Average.py
--rw-rw-rw-   0        0        0     3472 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Current.py
--rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Extreme.py
--rw-rw-rw-   0        0        0     2230 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/StandardDev.py
--rw-rw-rw-   0        0        0     1808 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/__init__.py
--rw-rw-rw-   0        0        0     5297 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StandardDev.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.196060 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.207774 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/
--rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Average.py
--rw-rw-rw-   0        0        0     4527 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Current.py
--rw-rw-rw-   0        0        0     3206 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Extreme.py
--rw-rw-rw-   0        0        0     3248 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/StandardDev.py
--rw-rw-rw-   0        0        0     1796 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.214604 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/
--rw-rw-rw-   0        0        0     3761 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Current.py
--rw-rw-rw-   0        0        0     2486 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Extreme.py
--rw-rw-rw-   0        0        0     1300 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.229245 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/
--rw-rw-rw-   0        0        0     2318 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Average.py
--rw-rw-rw-   0        0        0     4638 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Current.py
--rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Maximum.py
--rw-rw-rw-   0        0        0     3317 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Minimum.py
--rw-rw-rw-   0        0        0     3359 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/StandardDev.py
--rw-rw-rw-   0        0        0     2045 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/__init__.py
--rw-rw-rw-   0        0        0     1508 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.232173 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.239981 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/
--rw-rw-rw-   0        0        0     4182 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Current.py
--rw-rw-rw-   0        0        0     2907 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Extreme.py
--rw-rw-rw-   0        0        0     1300 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/__init__.py
--rw-rw-rw-   0        0        0     1048 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/__init__.py
--rw-rw-rw-   0        0        0     7239 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.244861 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.246812 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.251694 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/
--rw-rw-rw-   0        0        0     3443 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/Margin.py
--rw-rw-rw-   0        0        0     1831 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/__init__.py
--rw-rw-rw-   0        0        0     1005 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.254621 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.261453 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/
--rw-rw-rw-   0        0        0     3568 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/Current.py
--rw-rw-rw-   0        0        0     1839 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.268544 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/
--rw-rw-rw-   0        0        0     3721 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Current.py
--rw-rw-rw-   0        0        0     2446 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Extreme.py
--rw-rw-rw-   0        0        0     1305 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/__init__.py
--rw-rw-rw-   0        0        0     1286 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/__init__.py
--rw-rw-rw-   0        0        0     1676 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Otolerance.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.270498 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.275376 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/
--rw-rw-rw-   0        0        0     3443 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/Margin.py
--rw-rw-rw-   0        0        0     1831 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/__init__.py
--rw-rw-rw-   0        0        0     1005 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/__init__.py
--rw-rw-rw-   0        0        0     1744 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.289041 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/
--rw-rw-rw-   0        0        0     3077 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Average.py
--rw-rw-rw-   0        0        0     4350 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Current.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.304658 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/
--rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Average.py
--rw-rw-rw-   0        0        0     3432 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Current.py
--rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Maximum.py
--rw-rw-rw-   0        0        0     2158 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Minimum.py
--rw-rw-rw-   0        0        0     2190 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/StandardDev.py
--rw-rw-rw-   0        0        0     2048 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.320274 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/
--rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Average.py
--rw-rw-rw-   0        0        0     3426 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Current.py
--rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Maximum.py
--rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Minimum.py
--rw-rw-rw-   0        0        0     2184 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/StandardDev.py
--rw-rw-rw-   0        0        0     2043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/__init__.py
--rw-rw-rw-   0        0        0     3077 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Maximum.py
--rw-rw-rw-   0        0        0     3077 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Minimum.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.335888 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/
--rw-rw-rw-   0        0        0     2206 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Average.py
--rw-rw-rw-   0        0        0     3480 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Current.py
--rw-rw-rw-   0        0        0     2206 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Maximum.py
--rw-rw-rw-   0        0        0     2206 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Minimum.py
--rw-rw-rw-   0        0        0     2238 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/StandardDev.py
--rw-rw-rw-   0        0        0     2048 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.350528 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/
--rw-rw-rw-   0        0        0     2214 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Average.py
--rw-rw-rw-   0        0        0     3488 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Current.py
--rw-rw-rw-   0        0        0     2214 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Maximum.py
--rw-rw-rw-   0        0        0     2214 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Minimum.py
--rw-rw-rw-   0        0        0     2246 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/StandardDev.py
--rw-rw-rw-   0        0        0     2053 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.369581 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/
--rw-rw-rw-   0        0        0     2166 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Average.py
--rw-rw-rw-   0        0        0     3440 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Current.py
--rw-rw-rw-   0        0        0     2166 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Maximum.py
--rw-rw-rw-   0        0        0     2166 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Minimum.py
--rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py
--rw-rw-rw-   0        0        0     2048 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.391058 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/
--rw-rw-rw-   0        0        0     2160 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Average.py
--rw-rw-rw-   0        0        0     3434 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Current.py
--rw-rw-rw-   0        0        0     2160 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py
--rw-rw-rw-   0        0        0     2160 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py
--rw-rw-rw-   0        0        0     2192 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/StandardDev.py
--rw-rw-rw-   0        0        0     2043 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py
--rw-rw-rw-   0        0        0     3109 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/StandardDev.py
--rw-rw-rw-   0        0        0     3493 2022-12-20 09:29:14.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.426189 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/
--rw-rw-rw-   0        0        0     2170 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py
--rw-rw-rw-   0        0        0     2049 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Cindex.py
--rw-rw-rw-   0        0        0     2109 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/CsLength.py
--rw-rw-rw-   0        0        0     2150 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dlength.py
--rw-rw-rw-   0        0        0     1681 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dppdu.py
--rw-rw-rw-   0        0        0     2102 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Drate.py
--rw-rw-rw-   0        0        0     2305 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/FcsCheck.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.436925 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/
--rw-rw-rw-   0        0        0     2198 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/AsSymbols.py
--rw-rw-rw-   0        0        0     2989 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Bitrate.py
--rw-rw-rw-   0        0        0     2289 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py
--rw-rw-rw-   0        0        0     1491 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.446686 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/
--rw-rw-rw-   0        0        0     2064 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py
--rw-rw-rw-   0        0        0     2103 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py
--rw-rw-rw-   0        0        0     1228 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py
--rw-rw-rw-   0        0        0     3056 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/PstGap.py
--rw-rw-rw-   0        0        0     2092 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/RaBit.py
--rw-rw-rw-   0        0        0     2096 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/ReBit.py
--rw-rw-rw-   0        0        0     2152 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Sfd.py
--rw-rw-rw-   0        0        0     2118 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/SfdLength.py
--rw-rw-rw-   0        0        0     8135 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.451564 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/
--rw-rw-rw-   0        0        0     2110 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/All.py
--rw-rw-rw-   0        0        0     2751 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.454492 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.466205 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/
--rw-rw-rw-   0        0        0     1870 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py
--rw-rw-rw-   0        0        0     3592 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Current.py
--rw-rw-rw-   0        0        0     1780 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py
--rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.475965 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/
--rw-rw-rw-   0        0        0     1868 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py
--rw-rw-rw-   0        0        0     3590 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Current.py
--rw-rw-rw-   0        0        0     1776 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Xvalues.py
--rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.486701 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/
--rw-rw-rw-   0        0        0     1936 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Average.py
--rw-rw-rw-   0        0        0     3658 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Current.py
--rw-rw-rw-   0        0        0     1788 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Xvalues.py
--rw-rw-rw-   0        0        0     1522 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.497436 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/
--rw-rw-rw-   0        0        0     3560 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Current.py
--rw-rw-rw-   0        0        0     1768 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Xvalues.py
--rw-rw-rw-   0        0        0     1273 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.509148 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/
--rw-rw-rw-   0        0        0     2384 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Maximum.py
--rw-rw-rw-   0        0        0     2384 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Minimum.py
--rw-rw-rw-   0        0        0     1768 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Xvalues.py
--rw-rw-rw-   0        0        0     1547 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.520860 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/
--rw-rw-rw-   0        0        0     1848 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Average.py
--rw-rw-rw-   0        0        0     3570 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Current.py
--rw-rw-rw-   0        0        0     1760 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Xvalues.py
--rw-rw-rw-   0        0        0     1512 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.531596 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/
--rw-rw-rw-   0        0        0     1846 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Average.py
--rw-rw-rw-   0        0        0     3568 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Current.py
--rw-rw-rw-   0        0        0     1758 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Xvalues.py
--rw-rw-rw-   0        0        0     1512 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.542334 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/
--rw-rw-rw-   0        0        0     1882 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Average.py
--rw-rw-rw-   0        0        0     3604 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Current.py
--rw-rw-rw-   0        0        0     1784 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Xvalues.py
--rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.552093 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/
--rw-rw-rw-   0        0        0     1880 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Average.py
--rw-rw-rw-   0        0        0     3602 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Current.py
--rw-rw-rw-   0        0        0     1780 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Xvalues.py
--rw-rw-rw-   0        0        0     1532 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.565757 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/
--rw-rw-rw-   0        0        0     1866 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Average.py
--rw-rw-rw-   0        0        0     3588 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Current.py
--rw-rw-rw-   0        0        0     1776 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Xvalues.py
--rw-rw-rw-   0        0        0     1522 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/__init__.py
--rw-rw-rw-   0        0        0     3209 2022-12-20 09:29:15.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.573565 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.576493 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.588205 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/
--rw-rw-rw-   0        0        0     2432 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Average.py
--rw-rw-rw-   0        0        0     3667 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Current.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.598940 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/
--rw-rw-rw-   0        0        0     3701 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py
--rw-rw-rw-   0        0        0     4954 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Current.py
--rw-rw-rw-   0        0        0     1287 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.607726 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/
--rw-rw-rw-   0        0        0     3701 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py
--rw-rw-rw-   0        0        0     4954 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Current.py
--rw-rw-rw-   0        0        0     1287 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py
--rw-rw-rw-   0        0        0     2572 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/__init__.py
--rw-rw-rw-   0        0        0     1011 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/__init__.py
--rw-rw-rw-   0        0        0     2102 2022-12-20 09:29:13.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Otolerance.py
--rw-rw-rw-   0        0        0     1293 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/__init__.py
--rw-rw-rw-   0        0        0     5413 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1051 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:19.701421 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/
--rw-rw-rw-   0        0        0      586 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4165 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1116 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1145 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9097 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5751 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3439 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2546 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5238 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    25292 2022-12-19 08:08:03.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3781 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4812 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    12772 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Core.py
--rw-rw-rw-   0        0        0     1386 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/GlobalData.py
--rw-rw-rw-   0        0        0    59235 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Instrument.py
--rw-rw-rw-   0        0        0     4785 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2225 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0    12709 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3518 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4390 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     4289 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4745 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ScpiEnums.py
--rw-rw-rw-   0        0        0    34488 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ScpiLogger.py
--rw-rw-rw-   0        0        0     5098 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     5856 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1114 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StructBase.py
--rw-rw-rw-   0        0        0     3608 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Types.py
--rw-rw-rw-   0        0        0     5498 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Utilities.py
--rw-rw-rw-   0        0        0     5632 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    49606 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     7361 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0       29 2022-10-18 11:56:41.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/__init__.py
--rw-rw-rw-   0        0        0    12875 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/RsCMPX_UwbMeas.py
--rw-rw-rw-   0        0        0      932 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/__init__.py
--rw-rw-rw-   0        0        0     3542 2022-12-20 09:29:12.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/enums.py
--rw-rw-rw-   0        0        0     3166 2022-12-20 09:29:10.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/repcap.py
-drwxrwxrwx   0        0        0        0 2022-12-20 09:29:18.742689 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/
--rw-rw-rw-   0        0        0     3136 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    26592 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-12-20 09:29:18.000000 RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-20 09:29:19.706301 RsCMPX_UwbMeas-4.0.80/setup.cfg
--rw-rw-rw-   0        0        0     1435 2022-12-20 09:29:16.000000 RsCMPX_UwbMeas-4.0.80/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.382318 RsCMPX_UwbMeas-5.0.20/
+-rw-rw-rw-   0        0        0     3200 2024-04-19 08:52:32.382318 RsCMPX_UwbMeas-5.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0     1668 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.285249 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.316168 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/
+-rw-rw-rw-   0        0        0       90 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3725 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4916 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    21859 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.319158 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.324145 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Catalog/
+-rw-rw-rw-   0        0        0      880 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Catalog/UwbMeas.py
+-rw-rw-rw-   0        0        0     1033 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Catalog/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.327137 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.329133 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.356060 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.358056 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.377004 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/
+-rw-rw-rw-   0        0        0     2225 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/CcError.py
+-rw-rw-rw-   0        0        0     2241 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Foffset.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.381990 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/
+-rw-rw-rw-   0        0        0     2232 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/Nrmse.py
+-rw-rw-rw-   0        0        0     1007 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/__init__.py
+-rw-rw-rw-   0        0        0     2313 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Plevel.py
+-rw-rw-rw-   0        0        0     2249 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/PmlWidth.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.387976 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/
+-rw-rw-rw-   0        0        0     2240 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/Nrmse.py
+-rw-rw-rw-   0        0        0     1012 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.393960 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/
+-rw-rw-rw-   0        0        0     2232 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/Nrmse.py
+-rw-rw-rw-   0        0        0     1007 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/__init__.py
+-rw-rw-rw-   0        0        0     2221 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SlPeak.py
+-rw-rw-rw-   0        0        0     2289 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SmAccuracy.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.398946 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/
+-rw-rw-rw-   0        0        0     2232 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/Nrmse.py
+-rw-rw-rw-   0        0        0     1007 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/__init__.py
+-rw-rw-rw-   0        0        0     3125 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/__init__.py
+-rw-rw-rw-   0        0        0     1040 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py
+-rw-rw-rw-   0        0        0     1139 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/MprFrequency.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.404929 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr/
+-rw-rw-rw-   0        0        0     2366 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr/Bitrate.py
+-rw-rw-rw-   0        0        0     1019 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr/__init__.py
+-rw-rw-rw-   0        0        0     2682 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PhrRate.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.406924 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.411910 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/
+-rw-rw-rw-   0        0        0     2261 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Area.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.417894 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/
+-rw-rw-rw-   0        0        0     3111 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/Area.py
+-rw-rw-rw-   0        0        0     1009 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.437842 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/
+-rw-rw-rw-   0        0        0     3153 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/Area.py
+-rw-rw-rw-   0        0        0     1009 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py
+-rw-rw-rw-   0        0        0     1463 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/__init__.py
+-rw-rw-rw-   0        0        0     1013 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/__init__.py
+-rw-rw-rw-   0        0        0     2060 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PpLength.py
+-rw-rw-rw-   0        0        0     3102 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Ppdu.py
+-rw-rw-rw-   0        0        0     1110 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PrfMode.py
+-rw-rw-rw-   0        0        0     1856 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PsFormat.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.443826 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu/
+-rw-rw-rw-   0        0        0     2363 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu/Bitrate.py
+-rw-rw-rw-   0        0        0     1024 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu/__init__.py
+-rw-rw-rw-   0        0        0     4421 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py
+-rw-rw-rw-   0        0        0     2896 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Spectrum.py
+-rw-rw-rw-   0        0        0     1898 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StSegments.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.448812 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StsGap/
+-rw-rw-rw-   0        0        0     1180 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StsGap/Chip.py
+-rw-rw-rw-   0        0        0     2705 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StsGap/__init__.py
+-rw-rw-rw-   0        0        0     2010 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StsLength.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.451804 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.459783 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/
+-rw-rw-rw-   0        0        0     3972 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py
+-rw-rw-rw-   0        0        0     2275 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/TdbBandwidth.py
+-rw-rw-rw-   0        0        0     1291 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/__init__.py
+-rw-rw-rw-   0        0        0     1018 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py
+-rw-rw-rw-   0        0        0    16287 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.462775 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.467761 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/
+-rw-rw-rw-   0        0        0     2068 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/Range.py
+-rw-rw-rw-   0        0        0     2140 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/__init__.py
+-rw-rw-rw-   0        0        0     5807 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py
+-rw-rw-rw-   0        0        0     1321 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.470753 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.476737 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/
+-rw-rw-rw-   0        0        0     1388 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py
+-rw-rw-rw-   0        0        0     2085 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     1023 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.478732 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.480727 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.484716 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/
+-rw-rw-rw-   0        0        0     1025 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     7678 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1051 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     1033 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.486710 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.489703 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.499677 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/
+-rw-rw-rw-   0        0        0     2280 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Clength.py
+-rw-rw-rw-   0        0        0     2568 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Content.py
+-rw-rw-rw-   0        0        0     2506 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/RsParity.py
+-rw-rw-rw-   0        0        0     1543 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.517628 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/
+-rw-rw-rw-   0        0        0     5265 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Average.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.530593 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/
+-rw-rw-rw-   0        0        0     3148 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Average.py
+-rw-rw-rw-   0        0        0     4468 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Current.py
+-rw-rw-rw-   0        0        0     3148 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Extreme.py
+-rw-rw-rw-   0        0        0     3190 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/StandardDev.py
+-rw-rw-rw-   0        0        0     1804 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.542562 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/
+-rw-rw-rw-   0        0        0     2148 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Average.py
+-rw-rw-rw-   0        0        0     3422 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Current.py
+-rw-rw-rw-   0        0        0     2148 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Extreme.py
+-rw-rw-rw-   0        0        0     2180 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.554529 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/
+-rw-rw-rw-   0        0        0     2300 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Average.py
+-rw-rw-rw-   0        0        0     3574 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Current.py
+-rw-rw-rw-   0        0        0     2300 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2332 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.568493 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/
+-rw-rw-rw-   0        0        0     2198 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Average.py
+-rw-rw-rw-   0        0        0     3472 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Current.py
+-rw-rw-rw-   0        0        0     2198 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2230 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/__init__.py
+-rw-rw-rw-   0        0        0     6538 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Current.py
+-rw-rw-rw-   0        0        0     5265 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Extreme.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.582455 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/
+-rw-rw-rw-   0        0        0     3235 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Average.py
+-rw-rw-rw-   0        0        0     4555 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Current.py
+-rw-rw-rw-   0        0        0     3235 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Extreme.py
+-rw-rw-rw-   0        0        0     3277 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/StandardDev.py
+-rw-rw-rw-   0        0        0     1804 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.593425 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/
+-rw-rw-rw-   0        0        0     2242 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Average.py
+-rw-rw-rw-   0        0        0     3516 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Current.py
+-rw-rw-rw-   0        0        0     2242 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Extreme.py
+-rw-rw-rw-   0        0        0     2274 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.606391 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/
+-rw-rw-rw-   0        0        0     2156 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Average.py
+-rw-rw-rw-   0        0        0     3430 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Current.py
+-rw-rw-rw-   0        0        0     2156 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Extreme.py
+-rw-rw-rw-   0        0        0     2188 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.621355 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/
+-rw-rw-rw-   0        0        0     2300 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Average.py
+-rw-rw-rw-   0        0        0     3574 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Current.py
+-rw-rw-rw-   0        0        0     2300 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Extreme.py
+-rw-rw-rw-   0        0        0     2332 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/__init__.py
+-rw-rw-rw-   0        0        0     2130 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Otolerance.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.624343 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.638305 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/
+-rw-rw-rw-   0        0        0     3206 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4527 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3206 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3248 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.654264 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/
+-rw-rw-rw-   0        0        0     2326 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Average.py
+-rw-rw-rw-   0        0        0     4650 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Current.py
+-rw-rw-rw-   0        0        0     3329 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     3329 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     3371 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2045 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/__init__.py
+-rw-rw-rw-   0        0        0     1240 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.668225 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/
+-rw-rw-rw-   0        0        0     4300 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Average.py
+-rw-rw-rw-   0        0        0     5620 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Current.py
+-rw-rw-rw-   0        0        0     4300 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     4300 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     4342 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2043 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.680194 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/
+-rw-rw-rw-   0        0        0     3112 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Average.py
+-rw-rw-rw-   0        0        0     4432 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Current.py
+-rw-rw-rw-   0        0        0     3112 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Extreme.py
+-rw-rw-rw-   0        0        0     3154 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/StandardDev.py
+-rw-rw-rw-   0        0        0     1809 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.682189 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.695153 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/
+-rw-rw-rw-   0        0        0     3218 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4539 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3218 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3260 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.724076 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/
+-rw-rw-rw-   0        0        0     2334 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Average.py
+-rw-rw-rw-   0        0        0     4662 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Current.py
+-rw-rw-rw-   0        0        0     3341 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     3341 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     3383 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2045 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/__init__.py
+-rw-rw-rw-   0        0        0     1245 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.745021 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/
+-rw-rw-rw-   0        0        0     2162 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Average.py
+-rw-rw-rw-   0        0        0     3436 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Current.py
+-rw-rw-rw-   0        0        0     2162 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Extreme.py
+-rw-rw-rw-   0        0        0     2194 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/StandardDev.py
+-rw-rw-rw-   0        0        0     1803 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.759980 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/
+-rw-rw-rw-   0        0        0     2158 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Average.py
+-rw-rw-rw-   0        0        0     3432 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Current.py
+-rw-rw-rw-   0        0        0     2158 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Extreme.py
+-rw-rw-rw-   0        0        0     2190 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/StandardDev.py
+-rw-rw-rw-   0        0        0     1788 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.761975 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.769953 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/
+-rw-rw-rw-   0        0        0     3761 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Current.py
+-rw-rw-rw-   0        0        0     2486 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Extreme.py
+-rw-rw-rw-   0        0        0     1300 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/__init__.py
+-rw-rw-rw-   0        0        0     1043 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.772946 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.785911 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/
+-rw-rw-rw-   0        0        0     3206 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4527 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3206 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3248 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/__init__.py
+-rw-rw-rw-   0        0        0     1004 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.796882 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/
+-rw-rw-rw-   0        0        0     3454 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Average.py
+-rw-rw-rw-   0        0        0     4774 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Current.py
+-rw-rw-rw-   0        0        0     3454 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Extreme.py
+-rw-rw-rw-   0        0        0     3496 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/StandardDev.py
+-rw-rw-rw-   0        0        0     1799 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.813837 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/
+-rw-rw-rw-   0        0        0     3463 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Average.py
+-rw-rw-rw-   0        0        0     4783 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Current.py
+-rw-rw-rw-   0        0        0     3463 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Extreme.py
+-rw-rw-rw-   0        0        0     3505 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/StandardDev.py
+-rw-rw-rw-   0        0        0     1819 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.826802 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/
+-rw-rw-rw-   0        0        0     2274 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Average.py
+-rw-rw-rw-   0        0        0     3548 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Current.py
+-rw-rw-rw-   0        0        0     2274 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2306 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.839768 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/
+-rw-rw-rw-   0        0        0     2198 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Average.py
+-rw-rw-rw-   0        0        0     3472 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Current.py
+-rw-rw-rw-   0        0        0     2198 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Extreme.py
+-rw-rw-rw-   0        0        0     2230 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/StandardDev.py
+-rw-rw-rw-   0        0        0     1808 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/__init__.py
+-rw-rw-rw-   0        0        0     5297 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StandardDev.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.842759 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.855726 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/
+-rw-rw-rw-   0        0        0     3206 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Average.py
+-rw-rw-rw-   0        0        0     4527 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Current.py
+-rw-rw-rw-   0        0        0     3206 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Extreme.py
+-rw-rw-rw-   0        0        0     3248 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/StandardDev.py
+-rw-rw-rw-   0        0        0     1796 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.862706 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/
+-rw-rw-rw-   0        0        0     3761 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Current.py
+-rw-rw-rw-   0        0        0     2486 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Extreme.py
+-rw-rw-rw-   0        0        0     1300 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.878663 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/
+-rw-rw-rw-   0        0        0     2326 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Average.py
+-rw-rw-rw-   0        0        0     4650 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Current.py
+-rw-rw-rw-   0        0        0     3329 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Maximum.py
+-rw-rw-rw-   0        0        0     3329 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Minimum.py
+-rw-rw-rw-   0        0        0     3371 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/StandardDev.py
+-rw-rw-rw-   0        0        0     2045 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/__init__.py
+-rw-rw-rw-   0        0        0     1508 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.881655 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.889635 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/
+-rw-rw-rw-   0        0        0     4182 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Current.py
+-rw-rw-rw-   0        0        0     2907 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Extreme.py
+-rw-rw-rw-   0        0        0     1300 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/__init__.py
+-rw-rw-rw-   0        0        0     1048 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/__init__.py
+-rw-rw-rw-   0        0        0     7239 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.895618 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.898611 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.903597 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/
+-rw-rw-rw-   0        0        0     3443 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/Margin.py
+-rw-rw-rw-   0        0        0     1831 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/__init__.py
+-rw-rw-rw-   0        0        0     1005 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.905592 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.913570 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/
+-rw-rw-rw-   0        0        0     3568 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/Current.py
+-rw-rw-rw-   0        0        0     1839 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.922547 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/
+-rw-rw-rw-   0        0        0     3721 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Current.py
+-rw-rw-rw-   0        0        0     2446 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Extreme.py
+-rw-rw-rw-   0        0        0     1305 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/__init__.py
+-rw-rw-rw-   0        0        0     1676 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Otolerance.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.925538 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.932519 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/
+-rw-rw-rw-   0        0        0     3443 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/Margin.py
+-rw-rw-rw-   0        0        0     1831 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/__init__.py
+-rw-rw-rw-   0        0        0     1005 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/__init__.py
+-rw-rw-rw-   0        0        0     1744 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.951469 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/
+-rw-rw-rw-   0        0        0     3336 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Average.py
+-rw-rw-rw-   0        0        0     4609 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.968424 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/
+-rw-rw-rw-   0        0        0     2158 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Average.py
+-rw-rw-rw-   0        0        0     3432 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Current.py
+-rw-rw-rw-   0        0        0     2158 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Maximum.py
+-rw-rw-rw-   0        0        0     2158 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Minimum.py
+-rw-rw-rw-   0        0        0     2190 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.985378 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/
+-rw-rw-rw-   0        0        0     2152 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Average.py
+-rw-rw-rw-   0        0        0     3426 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Current.py
+-rw-rw-rw-   0        0        0     2152 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Maximum.py
+-rw-rw-rw-   0        0        0     2152 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Minimum.py
+-rw-rw-rw-   0        0        0     2184 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/StandardDev.py
+-rw-rw-rw-   0        0        0     2043 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/__init__.py
+-rw-rw-rw-   0        0        0     3336 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Maximum.py
+-rw-rw-rw-   0        0        0     3336 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Minimum.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.001336 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/
+-rw-rw-rw-   0        0        0     2206 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Average.py
+-rw-rw-rw-   0        0        0     3480 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Current.py
+-rw-rw-rw-   0        0        0     2206 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Maximum.py
+-rw-rw-rw-   0        0        0     2206 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Minimum.py
+-rw-rw-rw-   0        0        0     2238 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.018290 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/
+-rw-rw-rw-   0        0        0     2214 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Average.py
+-rw-rw-rw-   0        0        0     3488 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Current.py
+-rw-rw-rw-   0        0        0     2214 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Maximum.py
+-rw-rw-rw-   0        0        0     2214 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Minimum.py
+-rw-rw-rw-   0        0        0     2246 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2053 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.034248 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/
+-rw-rw-rw-   0        0        0     2166 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Average.py
+-rw-rw-rw-   0        0        0     3440 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Current.py
+-rw-rw-rw-   0        0        0     2166 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Maximum.py
+-rw-rw-rw-   0        0        0     2166 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Minimum.py
+-rw-rw-rw-   0        0        0     2198 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.048210 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/
+-rw-rw-rw-   0        0        0     2168 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Average.py
+-rw-rw-rw-   0        0        0     3442 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Current.py
+-rw-rw-rw-   0        0        0     2168 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Maximum.py
+-rw-rw-rw-   0        0        0     2168 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Minimum.py
+-rw-rw-rw-   0        0        0     2200 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.066163 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/
+-rw-rw-rw-   0        0        0     2226 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Average.py
+-rw-rw-rw-   0        0        0     2226 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Current.py
+-rw-rw-rw-   0        0        0     2226 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Maximum.py
+-rw-rw-rw-   0        0        0     2226 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Minimum.py
+-rw-rw-rw-   0        0        0     2258 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/StandardDev.py
+-rw-rw-rw-   0        0        0     2844 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.084114 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/
+-rw-rw-rw-   0        0        0     2160 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Average.py
+-rw-rw-rw-   0        0        0     3434 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Current.py
+-rw-rw-rw-   0        0        0     2160 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py
+-rw-rw-rw-   0        0        0     2160 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py
+-rw-rw-rw-   0        0        0     2192 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/StandardDev.py
+-rw-rw-rw-   0        0        0     2043 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py
+-rw-rw-rw-   0        0        0     3368 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/StandardDev.py
+-rw-rw-rw-   0        0        0     3957 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.118023 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/
+-rw-rw-rw-   0        0        0     2170 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py
+-rw-rw-rw-   0        0        0     2049 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Cindex.py
+-rw-rw-rw-   0        0        0     2109 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/CsLength.py
+-rw-rw-rw-   0        0        0     2150 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dlength.py
+-rw-rw-rw-   0        0        0     1681 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dppdu.py
+-rw-rw-rw-   0        0        0     2102 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Drate.py
+-rw-rw-rw-   0        0        0     2305 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/FcsCheck.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.132984 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/
+-rw-rw-rw-   0        0        0     2198 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/AsSymbols.py
+-rw-rw-rw-   0        0        0     1715 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Bitrate.py
+-rw-rw-rw-   0        0        0     2289 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py
+-rw-rw-rw-   0        0        0     1491 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.141961 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/
+-rw-rw-rw-   0        0        0     2064 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py
+-rw-rw-rw-   0        0        0     2103 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py
+-rw-rw-rw-   0        0        0     1228 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py
+-rw-rw-rw-   0        0        0     3056 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/PstGap.py
+-rw-rw-rw-   0        0        0     2092 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/RaBit.py
+-rw-rw-rw-   0        0        0     2096 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/ReBit.py
+-rw-rw-rw-   0        0        0     2152 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Sfd.py
+-rw-rw-rw-   0        0        0     2118 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/SfdLength.py
+-rw-rw-rw-   0        0        0     8135 2024-04-19 08:52:27.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.146947 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/
+-rw-rw-rw-   0        0        0     2110 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/All.py
+-rw-rw-rw-   0        0        0     2751 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.155924 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/StsSequence/
+-rw-rw-rw-   0        0        0     2366 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/StsSequence/Clength.py
+-rw-rw-rw-   0        0        0     2444 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/StsSequence/Content.py
+-rw-rw-rw-   0        0        0     1301 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/StsSequence/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.157918 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.167890 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/
+-rw-rw-rw-   0        0        0     1870 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py
+-rw-rw-rw-   0        0        0     3592 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Current.py
+-rw-rw-rw-   0        0        0     1780 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.177864 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/
+-rw-rw-rw-   0        0        0     1868 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py
+-rw-rw-rw-   0        0        0     3590 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Current.py
+-rw-rw-rw-   0        0        0     1776 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.186839 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/
+-rw-rw-rw-   0        0        0     1936 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Average.py
+-rw-rw-rw-   0        0        0     3658 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Current.py
+-rw-rw-rw-   0        0        0     1788 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Xvalues.py
+-rw-rw-rw-   0        0        0     1522 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.195816 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/
+-rw-rw-rw-   0        0        0     3560 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Current.py
+-rw-rw-rw-   0        0        0     1768 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Xvalues.py
+-rw-rw-rw-   0        0        0     1273 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.204792 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/
+-rw-rw-rw-   0        0        0     2384 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Maximum.py
+-rw-rw-rw-   0        0        0     2384 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Minimum.py
+-rw-rw-rw-   0        0        0     1768 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Xvalues.py
+-rw-rw-rw-   0        0        0     1547 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.213769 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/
+-rw-rw-rw-   0        0        0     1848 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Average.py
+-rw-rw-rw-   0        0        0     3570 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Current.py
+-rw-rw-rw-   0        0        0     1760 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Xvalues.py
+-rw-rw-rw-   0        0        0     1512 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.222744 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/
+-rw-rw-rw-   0        0        0     1846 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Average.py
+-rw-rw-rw-   0        0        0     3568 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Current.py
+-rw-rw-rw-   0        0        0     1758 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Xvalues.py
+-rw-rw-rw-   0        0        0     1512 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.232717 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/
+-rw-rw-rw-   0        0        0     1882 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Average.py
+-rw-rw-rw-   0        0        0     3604 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Current.py
+-rw-rw-rw-   0        0        0     1784 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.241694 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/
+-rw-rw-rw-   0        0        0     1880 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Average.py
+-rw-rw-rw-   0        0        0     3602 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Current.py
+-rw-rw-rw-   0        0        0     1780 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Xvalues.py
+-rw-rw-rw-   0        0        0     1532 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.251667 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/
+-rw-rw-rw-   0        0        0     1844 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Average.py
+-rw-rw-rw-   0        0        0     3566 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Current.py
+-rw-rw-rw-   0        0        0     1776 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Xvalues.py
+-rw-rw-rw-   0        0        0     1522 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/__init__.py
+-rw-rw-rw-   0        0        0     3209 2024-04-19 08:52:28.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.257651 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.259645 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.266626 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/
+-rw-rw-rw-   0        0        0     2421 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Average.py
+-rw-rw-rw-   0        0        0     3656 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.273609 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/
+-rw-rw-rw-   0        0        0     3679 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py
+-rw-rw-rw-   0        0        0     4932 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Current.py
+-rw-rw-rw-   0        0        0     1287 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.281587 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/
+-rw-rw-rw-   0        0        0     3679 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py
+-rw-rw-rw-   0        0        0     4932 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Current.py
+-rw-rw-rw-   0        0        0     1287 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py
+-rw-rw-rw-   0        0        0     2572 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/__init__.py
+-rw-rw-rw-   0        0        0     1011 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/__init__.py
+-rw-rw-rw-   0        0        0     2102 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Otolerance.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.286573 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.292557 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/Frequency/
+-rw-rw-rw-   0        0        0     1576 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/Frequency/Fhfl.py
+-rw-rw-rw-   0        0        0     3196 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/Frequency/__init__.py
+-rw-rw-rw-   0        0        0     2632 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/PsPower.py
+-rw-rw-rw-   0        0        0     1324 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/__init__.py
+-rw-rw-rw-   0        0        0     1577 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/__init__.py
+-rw-rw-rw-   0        0        0     5668 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1051 2024-04-19 08:52:26.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:32.379326 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/
+-rw-rw-rw-   0        0        0      586 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4165 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1116 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1145 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9097 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5751 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3439 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2546 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5238 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    25419 2024-04-03 11:15:31.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3775 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4768 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    14213 2024-04-03 11:15:31.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Core.py
+-rw-rw-rw-   0        0        0     1386 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/GlobalData.py
+-rw-rw-rw-   0        0        0    60862 2024-04-03 11:15:31.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4785 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2225 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0    16156 2024-04-03 11:15:31.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3518 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4390 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0      387 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Properties.py
+-rw-rw-rw-   0        0        0     4289 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4745 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ScpiEnums.py
+-rw-rw-rw-   0        0        0    35525 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ScpiLogger.py
+-rw-rw-rw-   0        0        0     5098 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5856 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1114 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3608 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Types.py
+-rw-rw-rw-   0        0        0     5498 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5716 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    51976 2024-04-03 11:15:31.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7512 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0       29 2024-02-28 16:27:53.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/__init__.py
+-rw-rw-rw-   0        0        0    13052 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/RsCMPX_UwbMeas.py
+-rw-rw-rw-   0        0        0      932 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/__init__.py
+-rw-rw-rw-   0        0        0     3560 2024-04-19 08:52:25.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/enums.py
+-rw-rw-rw-   0        0        0     2288 2024-04-19 08:52:23.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/repcap.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:52:31.303201 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/
+-rw-rw-rw-   0        0        0     3200 2024-04-19 08:52:30.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    28975 2024-04-19 08:52:31.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:52:30.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-19 08:52:30.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-19 08:52:30.000000 RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:52:32.383315 RsCMPX_UwbMeas-5.0.20/setup.cfg
+-rw-rw-rw-   0        0        0     1493 2024-04-19 08:52:29.000000 RsCMPX_UwbMeas-5.0.20/setup.py
```

### Comparing `RsCMPX_UwbMeas-4.0.80/PKG-INFO` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: RsCMPX_UwbMeas
-Version: 4.0.80
-Summary: CMP/CMX Ultra Wideband Measurement Remote-control module
+Name: RsCMPX-UwbMeas
+Version: 5.0.20
+Summary: CMP200 Ultra Wideband Measurement Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_UwbMeas
         ==================================
         
@@ -20,43 +20,50 @@
         
         .. image:: https://img.shields.io/pypi/pyversions/pybadges.svg
            :target: https://img.shields.io/pypi/pyversions/pybadges.svg
         
         .. image:: https://img.shields.io/pypi/dm/RsCMPX_UwbMeas.svg
            :target: https://pypi.python.org/pypi/RsCMPX_UwbMeas/
         
-        Rohde & Schwarz CMP/CMX Ultra Wideband Measurement RsCMPX_UwbMeas instrument driver.
+        Rohde & Schwarz CMP200 Ultra Wideband Measurement RsCMPX_UwbMeas instrument driver.
         
         Basic Hello-World code:
         
         .. code-block:: python
         
             from RsCMPX_UwbMeas import *
         
-            instr = RsCMPX_UwbMeas('TCPIP::192.168.56.101::5025::SOCKET', reset=True)
+            instr = RsCMPX_UwbMeas('TCPIP::192.168.2.101::hislip0')
             idn = instr.query('*IDN?')
             print('Hello, I am: ' + idn)
         
-        Check out the full documentation on `ReadTheDocs <https://RsCMPX_UwbMeas.readthedocs.io/>`_.
+        Supported instruments: CMP200
         
-        Supported instruments: CMX500, CMP200
+        The package is hosted here: https://pypi.org/project/RsCMPX-UwbMeas/
         
-        The package is hosted here: https://pypi.org/project/RsCMPX_UwbMeas/
-        
-        Documentation: https://RsCMPX_UwbMeas.readthedocs.io/
+        Documentation: https://RsCMPX-UwbMeas.readthedocs.io/
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
-        Version history:
+        Version history
         ----------------
         
-        	Latest release notes summary: Update of RsCMPX_UwbMeas to FW 4.0.80 from the complete FW package 7.10.0
+        	Latest release notes summary: Update for FW 5.0.20
+        
+        	Version 5.0.20
+        		- Update for FW 5.0.20
+        
+        	Version 4.0.171
+        		- Fixed documentation
+        
+        	Version 4.0.170
+        		- Update for FW 4.0.170
         
-        	Version 4.0.80.16
+        	Version 4.0.80
         		- Update of RsCMPX_UwbMeas to FW 4.0.80 from the complete FW package 7.10.0
         
         	Version 4.0.70
         		- Update of RsCMPX_UwbMeas to FW 4.0.70
         		
         	Version 4.0.12
         		- Update of RsCMPX_UwbMeas to FW 4.0.12
@@ -73,9 +80,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
```

### Comparing `RsCMPX_UwbMeas-4.0.80/README.rst` & `RsCMPX_UwbMeas-5.0.20/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -13,43 +13,50 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/pybadges.svg
    :target: https://img.shields.io/pypi/pyversions/pybadges.svg
 
 .. image:: https://img.shields.io/pypi/dm/RsCMPX_UwbMeas.svg
    :target: https://pypi.python.org/pypi/RsCMPX_UwbMeas/
 
-Rohde & Schwarz CMP/CMX Ultra Wideband Measurement RsCMPX_UwbMeas instrument driver.
+Rohde & Schwarz CMP200 Ultra Wideband Measurement RsCMPX_UwbMeas instrument driver.
 
 Basic Hello-World code:
 
 .. code-block:: python
 
     from RsCMPX_UwbMeas import *
 
-    instr = RsCMPX_UwbMeas('TCPIP::192.168.56.101::5025::SOCKET', reset=True)
+    instr = RsCMPX_UwbMeas('TCPIP::192.168.2.101::hislip0')
     idn = instr.query('*IDN?')
     print('Hello, I am: ' + idn)
 
-Check out the full documentation on `ReadTheDocs <https://RsCMPX_UwbMeas.readthedocs.io/>`_.
+Supported instruments: CMP200
 
-Supported instruments: CMX500, CMP200
+The package is hosted here: https://pypi.org/project/RsCMPX-UwbMeas/
 
-The package is hosted here: https://pypi.org/project/RsCMPX_UwbMeas/
-
-Documentation: https://RsCMPX_UwbMeas.readthedocs.io/
+Documentation: https://RsCMPX-UwbMeas.readthedocs.io/
 
 Examples: https://github.com/Rohde-Schwarz/Examples/
 
 
-Version history:
+Version history
 ----------------
 
-	Latest release notes summary: Update of RsCMPX_UwbMeas to FW 4.0.80 from the complete FW package 7.10.0
+	Latest release notes summary: Update for FW 5.0.20
+
+	Version 5.0.20
+		- Update for FW 5.0.20
+
+	Version 4.0.171
+		- Fixed documentation
+
+	Version 4.0.170
+		- Update for FW 4.0.170
 
-	Version 4.0.80.16
+	Version 4.0.80
 		- Update of RsCMPX_UwbMeas to FW 4.0.80 from the complete FW package 7.10.0
 
 	Version 4.0.70
 		- Update of RsCMPX_UwbMeas to FW 4.0.70
 		
 	Version 4.0.12
 		- Update of RsCMPX_UwbMeas to FW 4.0.12
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/events.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	@property
 	def io_events_include_data(self) -> bool:
 		"""Returns the current state of the io_events_include_data See the setter for more details."""
 		return self._core.io.io_events_include_data
 
 	@io_events_include_data.setter
 	def io_events_include_data(self, value: bool) -> None:
-		"""If True, the on_write and on_read events include also the sent/received data.
+		"""If True, the on_write and on_read events include also the transferred data.
 		Default value is False, to avoid handling potentially big data."""
 		self._core.io.io_events_include_data = value
 
 	@property
 	def before_write_handler(self) -> Callable:
 		"""Returns the handler of before_write events. \n
 		:return: current ``before_write_handler``"""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/reliability.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/CustomFiles/utilities.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/CustomFiles/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,14 +410,22 @@
 		Set the ``append_to_pc_file`` to True if you want to append the read content to the end of the existing PC file"""
 		self._core.io.read_file_from_instrument_to_pc(source_instr_file, target_pc_file, append_to_pc_file)
 
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
 		return self._core.get_last_sent_cmd()
 
+	def go_to_local(self) -> None:
+		"""Puts the instrument into local state."""
+		self._core.io.go_to_local()
+
+	def go_to_remote(self) -> None:
+		"""Puts the instrument into remote state."""
+		self._core.io.go_to_remote()
+
 	def get_lock(self) -> threading.RLock:
 		"""Returns the thread lock for the current session. \n
 		By default:
 			- If you create standard new RsCMPX_UwbMeas instance with new VISA session, the session gets a new thread lock. You can assign it to other RsCMPX_UwbMeas sessions in order to share one physical instrument with a multi-thread access.
 			- If you create new RsCMPX_UwbMeas from an existing session, the thread lock is shared automatically making both instances multi-thread safe.
 		You can always assign new thread lock by calling ``driver.utilities.assign_lock()``"""
 		return self._core.io.get_lock()
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/UwbMeas.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Catalog/UwbMeas.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("uwbMeas", core, parent)
 
 	def get_spath(self) -> List[str]:
 		"""SCPI: CATalog:UWB:MEAS<instance>:SPATh \n
 		Snippet: value: List[str] = driver.catalog.uwbMeas.get_spath() \n
-		Returns the names of the available signal paths. \n
-			:return: name_signal_path: Comma-separated list of strings, one string per signal path
+		Returns the names of the available RF connections. \n
+			:return: name_signal_path: Comma-separated list of strings, one string per RF connection.
 		"""
 		response = self._core.io.query_str('CATalog:UWB:MEAS<Instance>:SPATh?')
 		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Catalog/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/CcError.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/CcError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Foffset.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Foffset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/Nrmse.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/Nrmse.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Plevel.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Plevel.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/PmlWidth.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/PmlWidth.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("pmlWidth", core, parent)
 
 	def set(self, enable: bool, limit: float) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:PMLWidth \n
 		Snippet: driver.configure.uwbMeas.multiEval.modulation.limit.pmlWidth.set(enable = False, limit = 1.0) \n
-		Activates and defines a lower limit for the pulse main lobe width. \n
+		Activates and defines a lower limit for the pulse mainlobe width. \n
 			:param enable: No help available
 			:param limit: No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('limit', limit, DataType.Float))
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:PMLWidth {param}'.rstrip())
 
 	# noinspection PyTypeChecker
@@ -38,10 +38,10 @@
 			StructBase.__init__(self, self)
 			self.Enable: bool = None
 			self.Limit: float = None
 
 	def get(self) -> PmlWidthStruct:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:PMLWidth \n
 		Snippet: value: PmlWidthStruct = driver.configure.uwbMeas.multiEval.modulation.limit.pmlWidth.get() \n
-		Activates and defines a lower limit for the pulse main lobe width. \n
+		Activates and defines a lower limit for the pulse mainlobe width. \n
 			:return: structure: for return value, see the help for PmlWidthStruct structure arguments."""
 		return self._core.io.query_struct(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:PMLWidth?', self.__class__.PmlWidthStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/Nrmse.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/Nrmse.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/Nrmse.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/Nrmse.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SlPeak.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SlPeak.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("slPeak", core, parent)
 
 	def set(self, enable: bool, limit: float) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:SLPeak \n
 		Snippet: driver.configure.uwbMeas.multiEval.modulation.limit.slPeak.set(enable = False, limit = 1.0) \n
-		Activates and defines an upper limit for the pulse side lobe peak. \n
+		Activates and defines an upper limit for the pulse sidelobe peak. \n
 			:param enable: No help available
 			:param limit: No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('limit', limit, DataType.Float))
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:SLPeak {param}'.rstrip())
 
 	# noinspection PyTypeChecker
@@ -38,10 +38,10 @@
 			StructBase.__init__(self, self)
 			self.Enable: bool = None
 			self.Limit: float = None
 
 	def get(self) -> SlPeakStruct:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:SLPeak \n
 		Snippet: value: SlPeakStruct = driver.configure.uwbMeas.multiEval.modulation.limit.slPeak.get() \n
-		Activates and defines an upper limit for the pulse side lobe peak. \n
+		Activates and defines an upper limit for the pulse sidelobe peak. \n
 			:return: structure: for return value, see the help for SlPeakStruct structure arguments."""
 		return self._core.io.query_struct(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:MODulation:LIMit:SLPeak?', self.__class__.SlPeakStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SmAccuracy.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SmAccuracy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/Nrmse.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/Nrmse.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/Catalog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from typing import List
+
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal.Utilities import trim_str_response
+from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class PhrCls:
-	"""Phr commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
+class CatalogCls:
+	"""Catalog commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("phr", core, parent)
+		self._cmd_group = CommandsGroup("catalog", core, parent)
 
-	def get_bitrate(self) -> str:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PHR:BITRate \n
-		Snippet: value: str = driver.configure.uwbMeas.multiEval.phr.get_bitrate() \n
-		Queries the data rate of the PHR. \n
-			:return: phr_bitrate: No help available
+	def get_source(self) -> List[str]:
+		"""SCPI: TRIGger:UWB:MEASurement<Instance>:MEValuation:CATalog:SOURce \n
+		Snippet: value: List[str] = driver.trigger.uwbMeas.multiEval.catalog.get_source() \n
+		Lists all trigger source values that can be set using method RsCMPX_UwbMeas.Trigger.UwbMeas.MultiEval.source. \n
+			:return: trigger_sources: Comma-separated list of all supported values, one string per value.
 		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PHR:BITRate?')
-		return trim_str_response(response)
+		response = self._core.io.query_str('TRIGger:UWB:MEASurement<Instance>:MEValuation:CATalog:SOURce?')
+		return Conversions.str_to_str_list(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Area.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Area.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/Area.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/Area.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/Area.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/Area.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,75 +10,75 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("result", core, parent)
 
 	def get_ts_mask(self) -> bool:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask \n
 		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_ts_mask() \n
-		Enables or disables the evaluation of spectrum emission mask results. \n
-			:return: enable: OFF: Do not evaluate results ON: Evaluate results
+		Enables or disables the evaluation of spectrum results. \n
+			:return: enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask?')
 		return Conversions.str_to_bool(response)
 
 	def set_ts_mask(self, enable: bool) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask \n
 		Snippet: driver.configure.uwbMeas.multiEval.result.set_ts_mask(enable = False) \n
-		Enables or disables the evaluation of spectrum emission mask results. \n
-			:param enable: OFF: Do not evaluate results ON: Evaluate results
+		Enables or disables the evaluation of spectrum results. \n
+			:param enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:TSMask {param}')
 
 	def get_power_vs_time(self) -> bool:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime \n
 		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_power_vs_time() \n
 		Enables or disables the evaluation of power results. \n
-			:return: enable: OFF: Do not evaluate results ON: Evaluate results
+			:return: enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime?')
 		return Conversions.str_to_bool(response)
 
 	def set_power_vs_time(self, enable: bool) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime \n
 		Snippet: driver.configure.uwbMeas.multiEval.result.set_power_vs_time(enable = False) \n
 		Enables or disables the evaluation of power results. \n
-			:param enable: OFF: Do not evaluate results ON: Evaluate results
+			:param enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:PVTime {param}')
 
 	def get_emodulation(self) -> bool:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation \n
 		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_emodulation() \n
 		Enables or disables the evaluation of modulation and jitter results. \n
-			:return: enable: OFF: Do not evaluate results ON: Evaluate results
+			:return: enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation?')
 		return Conversions.str_to_bool(response)
 
 	def set_emodulation(self, enable: bool) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation \n
 		Snippet: driver.configure.uwbMeas.multiEval.result.set_emodulation(enable = False) \n
 		Enables or disables the evaluation of modulation and jitter results. \n
-			:param enable: OFF: Do not evaluate results ON: Evaluate results
+			:param enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:EMODulation {param}')
 
 	def get_ddecoding(self) -> bool:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding \n
 		Snippet: value: bool = driver.configure.uwbMeas.multiEval.result.get_ddecoding() \n
 		Enables or disables the evaluation of the PPDU payload contents. \n
-			:return: enable: OFF: Do not evaluate results ON: Evaluate results
+			:return: enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding?')
 		return Conversions.str_to_bool(response)
 
 	def set_ddecoding(self, enable: bool) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding \n
 		Snippet: driver.configure.uwbMeas.multiEval.result.set_ddecoding(enable = False) \n
 		Enables or disables the evaluation of the PPDU payload contents. \n
-			:param enable: OFF: Do not evaluate results ON: Evaluate results
+			:param enable: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:RESult:DDECoding {param}')
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Spectrum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Spectrum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from .......Internal.Core import Core
 from .......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class LimitCls:
-	"""Limit commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+	"""Limit commands group definition. 2 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("limit", core, parent)
 
 	@property
 	def area(self):
 		"""area commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_area'):
 			from .Area import AreaCls
 			self._area = AreaCls(self._core, self._cmd_group)
 		return self._area
 
+	@property
+	def tdbBandwidth(self):
+		"""tdbBandwidth commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_tdbBandwidth'):
+			from .TdbBandwidth import TdbBandwidthCls
+			self._tdbBandwidth = TdbBandwidthCls(self._core, self._cmd_group)
+		return self._tdbBandwidth
+
 	def clone(self) -> 'LimitCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = LimitCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class TsMaskCls:
-	"""TsMask commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+	"""TsMask commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("tsMask", core, parent)
 
 	@property
 	def limit(self):
-		"""limit commands group. 1 Sub-classes, 0 commands."""
+		"""limit commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_limit'):
 			from .Limit import LimitCls
 			self._limit = LimitCls(self._core, self._cmd_group)
 		return self._limit
 
 	def clone(self) -> 'TsMaskCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,116 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
-from .....Internal.Utilities import trim_str_response
 from ..... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MultiEvalCls:
-	"""MultiEval commands group definition. 39 total commands, 8 Subgroups, 16 group commands"""
+	"""MultiEval commands group definition. 44 total commands, 16 Subgroups, 9 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("multiEval", core, parent)
 
 	@property
+	def ppdu(self):
+		"""ppdu commands group. 0 Sub-classes, 3 commands."""
+		if not hasattr(self, '_ppdu'):
+			from .Ppdu import PpduCls
+			self._ppdu = PpduCls(self._core, self._cmd_group)
+		return self._ppdu
+
+	@property
 	def phr(self):
-		"""phr commands group. 0 Sub-classes, 1 commands."""
+		"""phr commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_phr'):
 			from .Phr import PhrCls
 			self._phr = PhrCls(self._core, self._cmd_group)
 		return self._phr
 
 	@property
 	def psdu(self):
-		"""psdu commands group. 0 Sub-classes, 1 commands."""
+		"""psdu commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_psdu'):
 			from .Psdu import PsduCls
 			self._psdu = PsduCls(self._core, self._cmd_group)
 		return self._psdu
 
 	@property
+	def mprFrequency(self):
+		"""mprFrequency commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_mprFrequency'):
+			from .MprFrequency import MprFrequencyCls
+			self._mprFrequency = MprFrequencyCls(self._core, self._cmd_group)
+		return self._mprFrequency
+
+	@property
+	def prfMode(self):
+		"""prfMode commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_prfMode'):
+			from .PrfMode import PrfModeCls
+			self._prfMode = PrfModeCls(self._core, self._cmd_group)
+		return self._prfMode
+
+	@property
+	def psFormat(self):
+		"""psFormat commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_psFormat'):
+			from .PsFormat import PsFormatCls
+			self._psFormat = PsFormatCls(self._core, self._cmd_group)
+		return self._psFormat
+
+	@property
+	def ppLength(self):
+		"""ppLength commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ppLength'):
+			from .PpLength import PpLengthCls
+			self._ppLength = PpLengthCls(self._core, self._cmd_group)
+		return self._ppLength
+
+	@property
+	def stSegments(self):
+		"""stSegments commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_stSegments'):
+			from .StSegments import StSegmentsCls
+			self._stSegments = StSegmentsCls(self._core, self._cmd_group)
+		return self._stSegments
+
+	@property
+	def stsLength(self):
+		"""stsLength commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_stsLength'):
+			from .StsLength import StsLengthCls
+			self._stsLength = StsLengthCls(self._core, self._cmd_group)
+		return self._stsLength
+
+	@property
+	def stsGap(self):
+		"""stsGap commands group. 1 Sub-classes, 1 commands."""
+		if not hasattr(self, '_stsGap'):
+			from .StsGap import StsGapCls
+			self._stsGap = StsGapCls(self._core, self._cmd_group)
+		return self._stsGap
+
+	@property
 	def spectrum(self):
 		"""spectrum commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_spectrum'):
 			from .Spectrum import SpectrumCls
 			self._spectrum = SpectrumCls(self._core, self._cmd_group)
 		return self._spectrum
 
 	@property
-	def ppdu(self):
-		"""ppdu commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_ppdu'):
-			from .Ppdu import PpduCls
-			self._ppdu = PpduCls(self._core, self._cmd_group)
-		return self._ppdu
+	def phrRate(self):
+		"""phrRate commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_phrRate'):
+			from .PhrRate import PhrRateCls
+			self._phrRate = PhrRateCls(self._core, self._cmd_group)
+		return self._phrRate
 
 	@property
 	def result(self):
 		"""result commands group. 0 Sub-classes, 4 commands."""
 		if not hasattr(self, '_result'):
 			from .Result import ResultCls
 			self._result = ResultCls(self._core, self._cmd_group)
@@ -73,31 +136,31 @@
 	def pmask(self):
 		"""pmask commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_pmask'):
 			from .Pmask import PmaskCls
 			self._pmask = PmaskCls(self._core, self._cmd_group)
 		return self._pmask
 
-	def get_mpr_frequency(self) -> str:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:MPRFrequency \n
-		Snippet: value: str = driver.configure.uwbMeas.multiEval.get_mpr_frequency() \n
-		Queries the mean pulse repetition frequency. \n
-			:return: mpr_frequency: No help available
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:MPRFrequency?')
-		return trim_str_response(response)
-
-	def get_prf_mode(self) -> str:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PRFMode \n
-		Snippet: value: str = driver.configure.uwbMeas.multiEval.get_prf_mode() \n
-		Queries the pulse repetition frequency mode. \n
-			:return: prf_mode: BPRF HPRF ---
+	def get_ptracking(self) -> bool:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PTRacking \n
+		Snippet: value: bool = driver.configure.uwbMeas.multiEval.get_ptracking() \n
+		Enables or disables phase tracking. \n
+			:return: enable: No help available
+		"""
+		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PTRacking?')
+		return Conversions.str_to_bool(response)
+
+	def set_ptracking(self, enable: bool) -> None:
+		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PTRacking \n
+		Snippet: driver.configure.uwbMeas.multiEval.set_ptracking(enable = False) \n
+		Enables or disables phase tracking. \n
+			:param enable: No help available
 		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PRFMode?')
-		return trim_str_response(response)
+		param = Conversions.bool_to_str(enable)
+		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PTRacking {param}')
 
 	# noinspection PyTypeChecker
 	def get_pmode(self) -> enums.PpduMode:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PMODe \n
 		Snippet: value: enums.PpduMode = driver.configure.uwbMeas.multiEval.get_pmode() \n
 		Selects the measurement mode. \n
 			:return: ppdu_mode: SPPDu: single PPDU packet analysis MPPDu: multi PPDU packet analysis
@@ -116,25 +179,25 @@
 
 	# noinspection PyTypeChecker
 	def get_scondition(self) -> enums.StopCondition:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:SCONdition \n
 		Snippet: value: enums.StopCondition = driver.configure.uwbMeas.multiEval.get_scondition() \n
 		Qualifies whether the measurement is stopped after a failed limit check or continued. SLFail means that the measurement
 		is stopped and reaches the RDY state when one of the results exceeds the limits. \n
-			:return: stop_condition: NONE: Continue measurement irrespective of the limit check SLFail: Stop measurement on limit failure
+			:return: stop_condition: NONE: Continue irrespective of the limit check. SLFail: Stop the measurement on limit failure.
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:SCONdition?')
 		return Conversions.str_to_scalar_enum(response, enums.StopCondition)
 
 	def set_scondition(self, stop_condition: enums.StopCondition) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:SCONdition \n
 		Snippet: driver.configure.uwbMeas.multiEval.set_scondition(stop_condition = enums.StopCondition.NONE) \n
 		Qualifies whether the measurement is stopped after a failed limit check or continued. SLFail means that the measurement
 		is stopped and reaches the RDY state when one of the results exceeds the limits. \n
-			:param stop_condition: NONE: Continue measurement irrespective of the limit check SLFail: Stop measurement on limit failure
+			:param stop_condition: NONE: Continue irrespective of the limit check. SLFail: Stop the measurement on limit failure.
 		"""
 		param = Conversions.enum_scalar_to_str(stop_condition, enums.StopCondition)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:SCONdition {param}')
 
 	def get_timeout(self) -> float:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:TOUT \n
 		Snippet: value: float = driver.configure.uwbMeas.multiEval.get_timeout() \n
@@ -222,128 +285,14 @@
 		Snippet: driver.configure.uwbMeas.multiEval.set_mo_exception(meas_on_exception = False) \n
 		Specifies whether measurement results identified as faulty or inaccurate are rejected. \n
 			:param meas_on_exception: OFF: Faulty results are rejected. ON: Results are never rejected.
 		"""
 		param = Conversions.bool_to_str(meas_on_exception)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:MOEXception {param}')
 
-	def get_ps_format(self) -> int:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PSFormat \n
-		Snippet: value: int = driver.configure.uwbMeas.multiEval.get_ps_format() \n
-		Specifies the PPDU STS packet structure configuration. See also 'HRP-ERDEV'. \n
-			:return: ppdu_sts_format: No help available
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PSFormat?')
-		return Conversions.str_to_int(response)
-
-	def set_ps_format(self, ppdu_sts_format: int) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PSFormat \n
-		Snippet: driver.configure.uwbMeas.multiEval.set_ps_format(ppdu_sts_format = 1) \n
-		Specifies the PPDU STS packet structure configuration. See also 'HRP-ERDEV'. \n
-			:param ppdu_sts_format: No help available
-		"""
-		param = Conversions.decimal_value_to_str(ppdu_sts_format)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PSFormat {param}')
-
-	def get_pp_length(self) -> int:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength \n
-		Snippet: value: int = driver.configure.uwbMeas.multiEval.get_pp_length() \n
-		Specifies the bit length of the PHR payload length field. This setting is only relevant in HPRF mode (RHML or RHMH set
-		via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.phrRate ) . \n
-			:return: phr_payload_len: No help available
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength?')
-		return Conversions.str_to_int(response)
-
-	def set_pp_length(self, phr_payload_len: int) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength \n
-		Snippet: driver.configure.uwbMeas.multiEval.set_pp_length(phr_payload_len = 1) \n
-		Specifies the bit length of the PHR payload length field. This setting is only relevant in HPRF mode (RHML or RHMH set
-		via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.phrRate ) . \n
-			:param phr_payload_len: No help available
-		"""
-		param = Conversions.decimal_value_to_str(phr_payload_len)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PPLength {param}')
-
-	def get_st_segments(self) -> int:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSegments \n
-		Snippet: value: int = driver.configure.uwbMeas.multiEval.get_st_segments() \n
-		Specifies the number of STS segments inserted according to the STS packet configuration. \n
-			:return: no_sts_segments: No help available
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:STSegments?')
-		return Conversions.str_to_int(response)
-
-	def set_st_segments(self, no_sts_segments: int) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSegments \n
-		Snippet: driver.configure.uwbMeas.multiEval.set_st_segments(no_sts_segments = 1) \n
-		Specifies the number of STS segments inserted according to the STS packet configuration. \n
-			:param no_sts_segments: No help available
-		"""
-		param = Conversions.decimal_value_to_str(no_sts_segments)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:STSegments {param}')
-
-	# noinspection PyTypeChecker
-	def get_sts_length(self) -> enums.StsSegmentLen:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSLength \n
-		Snippet: value: enums.StsSegmentLen = driver.configure.uwbMeas.multiEval.get_sts_length() \n
-		Specifies the length of the STS segment in units of 512 chips. \n
-			:return: sts_segment_len: No help available
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:STSLength?')
-		return Conversions.str_to_scalar_enum(response, enums.StsSegmentLen)
-
-	def set_sts_length(self, sts_segment_len: enums.StsSegmentLen) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSLength \n
-		Snippet: driver.configure.uwbMeas.multiEval.set_sts_length(sts_segment_len = enums.StsSegmentLen.L128) \n
-		Specifies the length of the STS segment in units of 512 chips. \n
-			:param sts_segment_len: No help available
-		"""
-		param = Conversions.enum_scalar_to_str(sts_segment_len, enums.StsSegmentLen)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:STSLength {param}')
-
-	def get_sts_gap(self) -> int:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap \n
-		Snippet: value: int = driver.configure.uwbMeas.multiEval.get_sts_gap() \n
-		Specifies additional gaps between the payload and the STS in unit of 4 chips. This setting is only relevant for PPDU STS
-		packet structure configuration two set via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.psFormat) . \n
-			:return: sts_gap: No help available
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap?')
-		return Conversions.str_to_int(response)
-
-	def set_sts_gap(self, sts_gap: int) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap \n
-		Snippet: driver.configure.uwbMeas.multiEval.set_sts_gap(sts_gap = 1) \n
-		Specifies additional gaps between the payload and the STS in unit of 4 chips. This setting is only relevant for PPDU STS
-		packet structure configuration two set via method RsCMPX_UwbMeas.Configure.UwbMeas.MultiEval.psFormat) . \n
-			:param sts_gap: No help available
-		"""
-		param = Conversions.decimal_value_to_str(sts_gap)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:STSGap {param}')
-
-	# noinspection PyTypeChecker
-	def get_phr_rate(self) -> enums.PhrDataRate:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate \n
-		Snippet: value: enums.PhrDataRate = driver.configure.uwbMeas.multiEval.get_phr_rate() \n
-		Specifies the data rate of the PHY header (PHR) . \n
-			:return: phr_data_rate: DRMD: 110 kb/s or 850 kb/s (DRMDR) DRLP: 850 kb/s (DRBM_LP) DRHP: 6.8 Mb/s (DRBM_HP) RHML: 3.9 Mb/s or 7.8 Mb/s (DRHM_LR) RHMH: 15.6 Mb/s or 31.2 Mb/s (DRHM_HR) SYNC: PPDU contains only SYNC field (SYNC_ONLY)
-		"""
-		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate?')
-		return Conversions.str_to_scalar_enum(response, enums.PhrDataRate)
-
-	def set_phr_rate(self, phr_data_rate: enums.PhrDataRate) -> None:
-		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate \n
-		Snippet: driver.configure.uwbMeas.multiEval.set_phr_rate(phr_data_rate = enums.PhrDataRate.DRHP) \n
-		Specifies the data rate of the PHY header (PHR) . \n
-			:param phr_data_rate: DRMD: 110 kb/s or 850 kb/s (DRMDR) DRLP: 850 kb/s (DRBM_LP) DRHP: 6.8 Mb/s (DRBM_HP) RHML: 3.9 Mb/s or 7.8 Mb/s (DRHM_LR) RHMH: 15.6 Mb/s or 31.2 Mb/s (DRHM_HR) SYNC: PPDU contains only SYNC field (SYNC_ONLY)
-		"""
-		param = Conversions.enum_scalar_to_str(phr_data_rate, enums.PhrDataRate)
-		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:MEValuation:PHRRate {param}')
-
 	def get_cap_length(self) -> float:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:MEValuation:CAPLength \n
 		Snippet: value: float = driver.configure.uwbMeas.multiEval.get_cap_length() \n
 		Defines the length to capture the signal. \n
 			:return: capture_length: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:MEValuation:CAPLength?')
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/Range.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/Range.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 			from .Range import RangeCls
 			self._range = RangeCls(self._core, self._cmd_group)
 		return self._range
 
 	def get_value(self) -> float:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency \n
 		Snippet: value: float = driver.configure.uwbMeas.rfSettings.frequency.get_value() \n
-		Selects the center frequency of the measured carrier. For the supported frequency range, see 'Frequency ranges'. \n
+		Selects the center frequency of the measured carrier for UWB signals. For the supported frequency range, see 'Frequency
+		ranges'. \n
 			:return: analyzer_freq: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency?')
 		return Conversions.str_to_float(response)
 
 	def set_value(self, analyzer_freq: float) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency \n
 		Snippet: driver.configure.uwbMeas.rfSettings.frequency.set_value(analyzer_freq = 1.0) \n
-		Selects the center frequency of the measured carrier. For the supported frequency range, see 'Frequency ranges'. \n
+		Selects the center frequency of the measured carrier for UWB signals. For the supported frequency range, see 'Frequency
+		ranges'. \n
 			:param analyzer_freq: No help available
 		"""
 		param = Conversions.decimal_value_to_str(analyzer_freq)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:RFSettings:FREQuency {param}')
 
 	def clone(self) -> 'FrequencyCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,64 +36,66 @@
 		"""
 		param = Conversions.decimal_value_to_str(analyzer_chan)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:RFSettings:CHANnel {param}')
 
 	def get_envelope_power(self) -> float:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:ENPower \n
 		Snippet: value: float = driver.configure.uwbMeas.rfSettings.get_envelope_power() \n
-		Sets the expected nominal power of the measured signal. \n
-			:return: exp_nominal_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+		Sets the expected nominal power of the measured UWB signal. \n
+			:return: exp_nominal_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:RFSettings:ENPower?')
 		return Conversions.str_to_float(response)
 
 	def set_envelope_power(self, exp_nominal_power: float) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:ENPower \n
 		Snippet: driver.configure.uwbMeas.rfSettings.set_envelope_power(exp_nominal_power = 1.0) \n
-		Sets the expected nominal power of the measured signal. \n
-			:param exp_nominal_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+		Sets the expected nominal power of the measured UWB signal. \n
+			:param exp_nominal_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 		"""
 		param = Conversions.decimal_value_to_str(exp_nominal_power)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:RFSettings:ENPower {param}')
 
 	def get_eattenuation(self) -> float:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:EATTenuation \n
 		Snippet: value: float = driver.configure.uwbMeas.rfSettings.get_eattenuation() \n
-		Defines an external attenuation (or gain, if the value is negative) , to be applied to the input connector. \n
+		Defines an external attenuation (or gain, if the value is negative) , to be applied to the input connector.
+		For measurement of UWB signals. \n
 			:return: rf_input_ext_att: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:RFSettings:EATTenuation?')
 		return Conversions.str_to_float(response)
 
 	def set_eattenuation(self, rf_input_ext_att: float) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:EATTenuation \n
 		Snippet: driver.configure.uwbMeas.rfSettings.set_eattenuation(rf_input_ext_att = 1.0) \n
-		Defines an external attenuation (or gain, if the value is negative) , to be applied to the input connector. \n
+		Defines an external attenuation (or gain, if the value is negative) , to be applied to the input connector.
+		For measurement of UWB signals. \n
 			:param rf_input_ext_att: No help available
 		"""
 		param = Conversions.decimal_value_to_str(rf_input_ext_att)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:RFSettings:EATTenuation {param}')
 
 	def get_umargin(self) -> float:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:UMARgin \n
 		Snippet: value: float = driver.configure.uwbMeas.rfSettings.get_umargin() \n
 		Sets the margin that the measurement adds to the expected nominal power to determine the reference power. The reference
 		power minus the external input attenuation must be within the power range of the selected input connector. Refer to the
-		data sheet. \n
+		specifications document. For measurement of UWB signals. \n
 			:return: user_margin: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:UWB:MEASurement<Instance>:RFSettings:UMARgin?')
 		return Conversions.str_to_float(response)
 
 	def set_umargin(self, user_margin: float) -> None:
 		"""SCPI: CONFigure:UWB:MEASurement<Instance>:RFSettings:UMARgin \n
 		Snippet: driver.configure.uwbMeas.rfSettings.set_umargin(user_margin = 1.0) \n
 		Sets the margin that the measurement adds to the expected nominal power to determine the reference power. The reference
 		power minus the external input attenuation must be within the power range of the selected input connector. Refer to the
-		data sheet. \n
+		specifications document. For measurement of UWB signals. \n
 			:param user_margin: No help available
 		"""
 		param = Conversions.decimal_value_to_str(user_margin)
 		self._core.io.write(f'CONFigure:UWB:MEASurement<Instance>:RFSettings:UMARgin {param}')
 
 	def clone(self) -> 'RfSettingsCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class UwbMeasCls:
-	"""UwbMeas commands group definition. 45 total commands, 2 Subgroups, 0 group commands"""
+	"""UwbMeas commands group definition. 50 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("uwbMeas", core, parent)
 
 	@property
 	def multiEval(self):
-		"""multiEval commands group. 8 Sub-classes, 16 commands."""
+		"""multiEval commands group. 16 Sub-classes, 9 commands."""
 		if not hasattr(self, '_multiEval'):
 			from .MultiEval import MultiEvalCls
 			self._multiEval = MultiEvalCls(self._core, self._cmd_group)
 		return self._multiEval
 
 	@property
 	def rfSettings(self):
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Configure/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class ConfigureCls:
-	"""Configure commands group definition. 45 total commands, 1 Subgroups, 0 group commands"""
+class RouteCls:
+	"""Route commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("configure", core, parent)
+		self._cmd_group = CommandsGroup("route", core, parent)
 
 	@property
 	def uwbMeas(self):
-		"""uwbMeas commands group. 2 Sub-classes, 0 commands."""
+		"""uwbMeas commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_uwbMeas'):
 			from .UwbMeas import UwbMeasCls
 			self._uwbMeas = UwbMeasCls(self._core, self._cmd_group)
 		return self._uwbMeas
 
-	def clone(self) -> 'ConfigureCls':
+	def clone(self) -> 'RouteCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = ConfigureCls(self._core, self._cmd_group.parent)
+		new_group = RouteCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Route/UwbMeas/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 			from .RfSettings import RfSettingsCls
 			self._rfSettings = RfSettingsCls(self._core, self._cmd_group)
 		return self._rfSettings
 
 	def get_spath(self) -> str:
 		"""SCPI: ROUTe:UWB:MEAS<instance>:SPATh \n
 		Snippet: value: str = driver.route.uwbMeas.get_spath() \n
-		Selects the signal path for the measured signal. For possible values, see method RsCMPX_UwbMeas.Catalog.UwbMeas.spath. \n
+		Selects the RF connection (signal input path) for the measured signal. For possible connection names, see method
+		RsCMPX_UwbMeas.Catalog.UwbMeas.spath. \n
 			:return: signal_path: No help available
 		"""
 		response = self._core.io.query_str('ROUTe:UWB:MEAS<Instance>:SPATh?')
 		return trim_str_response(response)
 
 	def set_spath(self, signal_path: str) -> None:
 		"""SCPI: ROUTe:UWB:MEAS<instance>:SPATh \n
-		Snippet: driver.route.uwbMeas.set_spath(signal_path = '1') \n
-		Selects the signal path for the measured signal. For possible values, see method RsCMPX_UwbMeas.Catalog.UwbMeas.spath. \n
+		Snippet: driver.route.uwbMeas.set_spath(signal_path = 'abc') \n
+		Selects the RF connection (signal input path) for the measured signal. For possible connection names, see method
+		RsCMPX_UwbMeas.Catalog.UwbMeas.spath. \n
 			:param signal_path: No help available
 		"""
 		param = Conversions.value_to_quoted_str(signal_path)
 		self._core.io.write(f'ROUTe:UWB:MEAS<Instance>:SPATh {param}')
 
 	def clone(self) -> 'UwbMeasCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Route/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class RouteCls:
-	"""Route commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
+class TriggerCls:
+	"""Trigger commands group definition. 7 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("route", core, parent)
+		self._cmd_group = CommandsGroup("trigger", core, parent)
 
 	@property
 	def uwbMeas(self):
-		"""uwbMeas commands group. 1 Sub-classes, 1 commands."""
+		"""uwbMeas commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_uwbMeas'):
 			from .UwbMeas import UwbMeasCls
 			self._uwbMeas = UwbMeasCls(self._core, self._cmd_group)
 		return self._uwbMeas
 
-	def clone(self) -> 'RouteCls':
+	def clone(self) -> 'TriggerCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = RouteCls(self._core, self._cmd_group.parent)
+		new_group = TriggerCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/MultiEval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 				- 'Free Run': Free run without synchronization
 				- 'IF Power': Power trigger (received RF power) """
 		response = self._core.io.query_str('TRIGger:UWB:MEASurement<Instance>:MEValuation:SOURce?')
 		return trim_str_response(response)
 
 	def set_source(self, source: str) -> None:
 		"""SCPI: TRIGger:UWB:MEASurement<Instance>:MEValuation:SOURce \n
-		Snippet: driver.trigger.uwbMeas.multiEval.set_source(source = '1') \n
+		Snippet: driver.trigger.uwbMeas.multiEval.set_source(source = 'abc') \n
 		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
 		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
 		:CATalog:SOURce?. \n
 			:param source:
 				- 'Free Run': Free run without synchronization
 				- 'IF Power': Power trigger (received RF power) """
 		param = Conversions.value_to_quoted_str(source)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Trigger/UwbMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/Trigger/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class TriggerCls:
-	"""Trigger commands group definition. 7 total commands, 1 Subgroups, 0 group commands"""
+class PhrCls:
+	"""Phr commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("trigger", core, parent)
+		self._cmd_group = CommandsGroup("phr", core, parent)
 
 	@property
-	def uwbMeas(self):
-		"""uwbMeas commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_uwbMeas'):
-			from .UwbMeas import UwbMeasCls
-			self._uwbMeas = UwbMeasCls(self._core, self._cmd_group)
-		return self._uwbMeas
+	def bitrate(self):
+		"""bitrate commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_bitrate'):
+			from .Bitrate import BitrateCls
+			self._bitrate = BitrateCls(self._core, self._cmd_group)
+		return self._bitrate
 
-	def clone(self) -> 'TriggerCls':
+	def clone(self) -> 'PhrCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = TriggerCls(self._core, self._cmd_group.parent)
+		new_group = PhrCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Clength.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Clength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Content.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/Content.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("content", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliabiltiy: int: 'Reliability indicator'
-			- Content: List[str]: Comma-separated list of hexadecimal values. The number of values can be queried via [CMDLINK: READ:UWB:MEASi:MEValuation:DDECoding:CLENgthPPDU? CMDLINK]."""
+			- Content: List[str]: Comma-separated list of hexadecimal values. The number of values can be queried via [CMDLINKRESOLVED UwbMeas.MultiEval.Ddecoding.Clength#Read CMDLINKRESOLVED]."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliabiltiy'),
 			ArgStruct('Content', DataType.RawStringList, None, False, True, 1)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliabiltiy: int = None
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/RsParity.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/RsParity.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Ddecoding/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CcError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Cevm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CpJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/CtJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Foffset/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Fofh/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/IqOffset/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Nmse/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Otolerance.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Otolerance.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Nrmse/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Average.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.average.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Current.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,40 +28,40 @@
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Default) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:CURRent<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.phr.plevel.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.maximum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.phr.plevel.maximum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/Minimum.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("minimum", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MINimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.minimum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MINimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.minimum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MINimum<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.phr.plevel.minimum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/StandardDev.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.phr.plevel.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.phr.plevel.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PHR pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PHR pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PHR:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/Plevel/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Phr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Average.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 			self.Phr_Plevel: float = None
 			self.Psdu_Plevel: float = None
 			self.Sts_Plevel: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:AVERage<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:AVERage<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.average.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
@@ -71,12 +71,12 @@
 			self.Phr_Plevel: enums.ResultStatus2 = None
 			self.Psdu_Plevel: enums.ResultStatus2 = None
 			self.Sts_Plevel: enums.ResultStatus2 = None
 
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> CalculateStruct:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:AVERage<PPDU> \n
 		Snippet: value: CalculateStruct = driver.uwbMeas.multiEval.modulation.plevel.average.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:AVERage{ppdu_cmd_val}?', self.__class__.CalculateStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,24 +47,24 @@
 			self.Phr_Plevel: float = None
 			self.Psdu_Plevel: float = None
 			self.Sts_Plevel: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:CURRent<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:CURRent<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
@@ -85,15 +85,15 @@
 			self.Phr_Plevel: enums.ResultStatus2 = None
 			self.Psdu_Plevel: enums.ResultStatus2 = None
 			self.Sts_Plevel: enums.ResultStatus2 = None
 
 	def calculate(self, ppdu=repcap.Ppdu.Default) -> CalculateStruct:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:CURRent<PPDU> \n
 		Snippet: value: CalculateStruct = driver.uwbMeas.multiEval.modulation.plevel.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:CURRent{ppdu_cmd_val}?', self.__class__.CalculateStruct())
 
 	def clone(self) -> 'CurrentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 			self.Phr_Plevel: float = None
 			self.Psdu_Plevel: float = None
 			self.Sts_Plevel: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MAXimum{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.maximum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MAXimum{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
@@ -71,12 +71,12 @@
 			self.Phr_Plevel: enums.ResultStatus2 = None
 			self.Psdu_Plevel: enums.ResultStatus2 = None
 			self.Sts_Plevel: enums.ResultStatus2 = None
 
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> CalculateStruct:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: CalculateStruct = driver.uwbMeas.multiEval.modulation.plevel.maximum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MAXimum{ppdu_cmd_val}?', self.__class__.CalculateStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/Minimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 			self.Phr_Plevel: float = None
 			self.Psdu_Plevel: float = None
 			self.Sts_Plevel: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MINimum<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.minimum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MINimum{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MINimum<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.minimum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MINimum{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
@@ -71,12 +71,12 @@
 			self.Phr_Plevel: enums.ResultStatus2 = None
 			self.Psdu_Plevel: enums.ResultStatus2 = None
 			self.Sts_Plevel: enums.ResultStatus2 = None
 
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> CalculateStruct:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MINimum<PPDU> \n
 		Snippet: value: CalculateStruct = driver.uwbMeas.multiEval.modulation.plevel.minimum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:MINimum{ppdu_cmd_val}?', self.__class__.CalculateStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/StandardDev.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 			self.Phr_Plevel: float = None
 			self.Psdu_Plevel: float = None
 			self.Sts_Plevel: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:SDEViation{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.modulation.plevel.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:SDEViation{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
@@ -71,12 +71,12 @@
 			self.Phr_Plevel: enums.ResultStatus2 = None
 			self.Psdu_Plevel: enums.ResultStatus2 = None
 			self.Sts_Plevel: enums.ResultStatus2 = None
 
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> CalculateStruct:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: CalculateStruct = driver.uwbMeas.multiEval.modulation.plevel.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns pulse levels according to FIRA specification, relative to the SHR pulse level. \n
+		Returns pulse levels according to the FIRA specification, relative to the SHR pulse level. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PLEVel:SDEViation{ppdu_cmd_val}?', self.__class__.CalculateStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Plevel/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Average.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.average.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.average.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,40 +28,40 @@
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Default) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/Extreme.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("extreme", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/StandardDev.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.pmlWidth.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.pmlWidth.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the pulse main lobe width. \n
+		Returns the pulse mainlobe width. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: width: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PMLWidth:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/PmlWidth/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Nrmse/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Average.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.average.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,40 +28,40 @@
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Default) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:CURRent<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.psdu.plevel.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Maximum.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.maximum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.psdu.plevel.maximum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/Minimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("minimum", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MINimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.minimum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MINimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.minimum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MINimum<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.psdu.plevel.minimum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/StandardDev.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.psdu.plevel.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.psdu.plevel.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the PSDU pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the PSDU pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:PSDU:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/Plevel/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Psdu/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Rmarker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sevm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/PlPolarity/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sfd/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/Nrmse/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Shr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Average.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.average.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.average.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:AVERage{ppdu_cmd_val}?', suppressed)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Current.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,51 +26,51 @@
 
 	def repcap_ppdu_get(self) -> repcap.Ppdu:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
-		pulse and the reference pulse) . \n
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.current.fetch(ppdu = repcap.Ppdu.Default) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: peak: No help available"""
+			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent{ppdu_cmd_val}?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
-		pulse and the reference pulse) . \n
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.current.read(ppdu = repcap.Ppdu.Default) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: peak: No help available"""
+			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent{ppdu_cmd_val}?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Default) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent<PPDU> \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
-		pulse and the reference pulse) . \n
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.current.calculate(ppdu = repcap.Ppdu.Default) \n
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
+		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: peak: No help available"""
+			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:CURRent{ppdu_cmd_val}?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
 
 	def clone(self) -> 'CurrentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = CurrentCls(self._core, self._cmd_group.parent)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/Extreme.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("extreme", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:EXTReme{ppdu_cmd_val}?', suppressed)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/StandardDev.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.slPeak.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.slPeak.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the side lobe peak (largest magnitude of side lobe peaks of the normalized cross correlation between the measured
+		Returns the sidelobe peak (largest magnitude of sidelobe peaks of the normalized cross-correlation between the measured
 		pulse and the reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: peak: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SLPeak:SDEViation{ppdu_cmd_val}?', suppressed)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SlPeak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Average.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.average.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.average.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:AVERage{ppdu_cmd_val}?', suppressed)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Current.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from ......Internal.Core import Core
-from ......Internal.CommandsGroup import CommandsGroup
-from ......Internal import Conversions
-from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from ......Internal.Types import DataType
-from ......Internal.RepeatedCapability import RepeatedCapability
-from ...... import enums
-from ...... import repcap
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
+from .......Internal import Conversions
+from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from .......Internal.Types import DataType
+from .......Internal.RepeatedCapability import RepeatedCapability
+from ....... import enums
+from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class CurrentCls:
 	"""Current commands group definition. 3 total commands, 0 Subgroups, 3 group commands
 	Repeated Capability: Ppdu, default value after init: Ppdu.Nr1"""
 
@@ -26,51 +26,48 @@
 
 	def repcap_ppdu_get(self) -> repcap.Ppdu:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
-		reference pulse) . \n
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.nrmse.current.fetch(ppdu = repcap.Ppdu.Default) \n
+		Returns the NRMSE for STS, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: accuracy: No help available"""
+			:return: error: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent{ppdu_cmd_val}?', suppressed)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
-		reference pulse) . \n
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.nrmse.current.read(ppdu = repcap.Ppdu.Default) \n
+		Returns the NRMSE for STS, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: accuracy: No help available"""
+			:return: error: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent{ppdu_cmd_val}?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Default) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent<PPDU> \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
-		reference pulse) . \n
+		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent<PPDU> \n
+		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.sts.nrmse.current.calculate(ppdu = repcap.Ppdu.Default) \n
+		Returns the NRMSE for STS, according to FIRA specification. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: accuracy: No help available"""
+			:return: error: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:CURRent{ppdu_cmd_val}?', suppressed)
+		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
 
 	def clone(self) -> 'CurrentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = CurrentCls(self._core, self._cmd_group.parent)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/Extreme.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("extreme", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.extreme.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:EXTReme{ppdu_cmd_val}?', suppressed)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/StandardDev.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,42 +14,42 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.smAccuracy.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the symbol modulation accuracy (magnitude of the normalized cross correlation between the measured pulse and the
+		Returns the symbol modulation accuracy (magnitude of the normalized cross-correlation between the measured pulse and the
 		reference pulse) . \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: accuracy: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:SMACcuracy:SDEViation{ppdu_cmd_val}?', suppressed)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SmAccuracy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/SpJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Current.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from .......Internal.Core import Core
 from .......Internal.CommandsGroup import CommandsGroup
 from .......Internal import Conversions
 from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from .......Internal.Types import DataType
+from .......Internal.StructBase import StructBase
+from .......Internal.ArgStruct import ArgStruct
 from .......Internal.RepeatedCapability import RepeatedCapability
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class CurrentCls:
-	"""Current commands group definition. 3 total commands, 0 Subgroups, 3 group commands
+	"""Current commands group definition. 2 total commands, 0 Subgroups, 2 group commands
 	Repeated Capability: Ppdu, default value after init: Ppdu.Nr1"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("current", core, parent)
 		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_ppdu_get', 'repcap_ppdu_set', repcap.Ppdu.Nr1)
 
@@ -25,50 +27,49 @@
 		self._cmd_group.set_repcap_enum_value(ppdu)
 
 	def repcap_ppdu_get(self) -> repcap.Ppdu:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
-	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.nrmse.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the NRMSE for STS, according to FIRA specification. \n
-		Suppressed linked return values: reliability \n
-			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: error: No help available"""
-		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent{ppdu_cmd_val}?', suppressed)
-		return Conversions.str_to_float(response)
-
-	def read(self, ppdu=repcap.Ppdu.Default) -> float:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.nrmse.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the NRMSE for STS, according to FIRA specification. \n
-		Suppressed linked return values: reliability \n
+	# noinspection PyTypeChecker
+	class FetchStruct(StructBase):
+		"""Response structure. Fields: \n
+			- Reliabiltiy: int: No parameter help available
+			- Sync_Pulse_Loc_Pol: enums.Result: No parameter help available"""
+		__meta_args_list = [
+			ArgStruct.scalar_int('Reliabiltiy'),
+			ArgStruct.scalar_enum('Sync_Pulse_Loc_Pol', enums.Result)]
+
+		def __init__(self):
+			StructBase.__init__(self, self)
+			self.Reliabiltiy: int = None
+			self.Sync_Pulse_Loc_Pol: enums.Result = None
+
+	def fetch(self, ppdu=repcap.Ppdu.Default) -> FetchStruct:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent<PPDU> \n
+		Snippet: value: FetchStruct = driver.uwbMeas.multiEval.modulation.sync.plPolarity.current.fetch(ppdu = repcap.Ppdu.Default) \n
+		Returns the result of the check for correct pulse location and polarity, for SYNC. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: error: No help available"""
+			:return: structure: for return value, see the help for FetchStruct structure arguments."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
-		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent{ppdu_cmd_val}?', suppressed)
-		return Conversions.str_to_float(response)
+		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent{ppdu_cmd_val}?', self.__class__.FetchStruct())
 
 	# noinspection PyTypeChecker
-	def calculate(self, ppdu=repcap.Ppdu.Default) -> enums.ResultStatus2:
-		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent<PPDU> \n
-		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.sts.nrmse.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns the NRMSE for STS, according to FIRA specification. \n
+	def read(self, ppdu=repcap.Ppdu.Default) -> enums.Result:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.modulation.sync.plPolarity.current.read(ppdu = repcap.Ppdu.Default) \n
+		Returns the result of the check for correct pulse location and polarity, for SYNC. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: error: No help available"""
+			:return: sync_pulse_loc_pol: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:NRMSe:CURRent{ppdu_cmd_val}?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
 
 	def clone(self) -> 'CurrentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = CurrentCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Nrmse/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/PlPolarity/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Average.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.average.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:AVERage{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Current.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,40 +28,40 @@
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:CURRent<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Default) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:CURRent<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.sts.plevel.current.calculate(ppdu = repcap.Ppdu.Default) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.maximum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MAXimum<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.sts.plevel.maximum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MAXimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/Minimum.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("minimum", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MINimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.minimum.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MINimum<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.minimum.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MINimum<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.sts.plevel.minimum.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:MINimum{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/StandardDev.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,40 +14,40 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: float = driver.uwbMeas.multiEval.modulation.sts.plevel.standardDev.read(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_float(response)
 
 	# noinspection PyTypeChecker
 	def calculate(self, ppdu=repcap.Ppdu.Nr1) -> enums.ResultStatus2:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:SDEViation<PPDU> \n
 		Snippet: value: enums.ResultStatus2 = driver.uwbMeas.multiEval.modulation.sts.plevel.standardDev.calculate(ppdu = repcap.Ppdu.Nr1) \n
-		Returns the STS pulse level according to FIRA specification, relative to the SHR pulse level. \n
+		Returns the STS pulse level according to the FIRA specification, relative to the SHR pulse level. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: level: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_str_suppressed(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:MODulation:STS:PLEVel:SDEViation{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.ResultStatus2)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/Plevel/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sts/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Current.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from .......Internal.Core import Core
 from .......Internal.CommandsGroup import CommandsGroup
 from .......Internal import Conversions
 from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
 from .......Internal.Types import DataType
-from .......Internal.StructBase import StructBase
-from .......Internal.ArgStruct import ArgStruct
 from .......Internal.RepeatedCapability import RepeatedCapability
 from ....... import enums
 from ....... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class CurrentCls:
@@ -28,47 +26,37 @@
 
 	def repcap_ppdu_get(self) -> repcap.Ppdu:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	# noinspection PyTypeChecker
-	class FetchStruct(StructBase):
-		"""Response structure. Fields: \n
-			- Reliabiltiy: int: No parameter help available
-			- Sync_Pulse_Loc_Pol: enums.Result: No parameter help available"""
-		__meta_args_list = [
-			ArgStruct.scalar_int('Reliabiltiy'),
-			ArgStruct.scalar_enum('Sync_Pulse_Loc_Pol', enums.Result)]
-
-		def __init__(self):
-			StructBase.__init__(self, self)
-			self.Reliabiltiy: int = None
-			self.Sync_Pulse_Loc_Pol: enums.Result = None
-
-	def fetch(self, ppdu=repcap.Ppdu.Default) -> FetchStruct:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent<PPDU> \n
-		Snippet: value: FetchStruct = driver.uwbMeas.multiEval.modulation.sync.plPolarity.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the result of the check for correct pulse location and polarity, for SYNC. \n
+	def fetch(self, ppdu=repcap.Ppdu.Default) -> enums.Result:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.pmask.margin.prMonotonic.current.fetch(ppdu = repcap.Ppdu.Default) \n
+		Returns the result of the check for monotonic rise of the pulse. \n
+		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: structure: for return value, see the help for FetchStruct structure arguments."""
+			:return: pr_monotonic: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
-		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent{ppdu_cmd_val}?', self.__class__.FetchStruct())
+		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_scalar_enum(response, enums.Result)
 
 	# noinspection PyTypeChecker
 	def read(self, ppdu=repcap.Ppdu.Default) -> enums.Result:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent<PPDU> \n
-		Snippet: value: enums.Result = driver.uwbMeas.multiEval.modulation.sync.plPolarity.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the result of the check for correct pulse location and polarity, for SYNC. \n
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent<PPDU> \n
+		Snippet: value: enums.Result = driver.uwbMeas.multiEval.pmask.margin.prMonotonic.current.read(ppdu = repcap.Ppdu.Default) \n
+		Returns the result of the check for monotonic rise of the pulse. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: sync_pulse_loc_pol: No help available"""
+			:return: pr_monotonic: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:MODulation:SYNC:PLPolarity:CURRent{ppdu_cmd_val}?', suppressed)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent{ppdu_cmd_val}?', suppressed)
 		return Conversions.str_to_scalar_enum(response, enums.Result)
 
 	def clone(self) -> 'CurrentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = CurrentCls(self._core, self._cmd_group.parent)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/PlPolarity/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/Sync/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/Margin.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/Margin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/Area/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Lower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/Area/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Current.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from .......Internal.Core import Core
-from .......Internal.CommandsGroup import CommandsGroup
-from .......Internal import Conversions
-from .......Internal.ArgSingleSuppressed import ArgSingleSuppressed
-from .......Internal.Types import DataType
-from .......Internal.RepeatedCapability import RepeatedCapability
-from ....... import enums
-from ....... import repcap
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ......Internal.ArgSingleSuppressed import ArgSingleSuppressed
+from ......Internal.Types import DataType
+from ......Internal.RepeatedCapability import RepeatedCapability
+from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class CurrentCls:
 	"""Current commands group definition. 2 total commands, 0 Subgroups, 2 group commands
 	Repeated Capability: Ppdu, default value after init: Ppdu.Nr1"""
 
@@ -25,39 +24,37 @@
 		self._cmd_group.set_repcap_enum_value(ppdu)
 
 	def repcap_ppdu_get(self) -> repcap.Ppdu:
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
-	# noinspection PyTypeChecker
-	def fetch(self, ppdu=repcap.Ppdu.Default) -> enums.Result:
-		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent<PPDU> \n
-		Snippet: value: enums.Result = driver.uwbMeas.multiEval.pmask.margin.prMonotonic.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the result of the check for monotonic rise of the pulse. \n
+	def fetch(self, ppdu=repcap.Ppdu.Default) -> float:
+		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPDPeak:CURRent<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppdPeak.current.fetch(ppdu = repcap.Ppdu.Default) \n
+		Returns the peak power of the PPDU. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: pr_monotonic: No help available"""
+			:return: ppdu_peak_power: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent{ppdu_cmd_val}?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.Result)
+		response = self._core.io.query_str_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:PPDPeak:CURRent{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
 
-	# noinspection PyTypeChecker
-	def read(self, ppdu=repcap.Ppdu.Default) -> enums.Result:
-		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent<PPDU> \n
-		Snippet: value: enums.Result = driver.uwbMeas.multiEval.pmask.margin.prMonotonic.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the result of the check for monotonic rise of the pulse. \n
+	def read(self, ppdu=repcap.Ppdu.Default) -> float:
+		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPDPeak:CURRent<PPDU> \n
+		Snippet: value: float = driver.uwbMeas.multiEval.power.ppdPeak.current.read(ppdu = repcap.Ppdu.Default) \n
+		Returns the peak power of the PPDU. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: pr_monotonic: No help available"""
+			:return: ppdu_peak_power: No help available"""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
-		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:PMASk:MARGin:PRMonotonic:CURRent{ppdu_cmd_val}?', suppressed)
-		return Conversions.str_to_scalar_enum(response, enums.Result)
+		response = self._core.io.query_str_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:POWer:PPDPeak:CURRent{ppdu_cmd_val}?', suppressed)
+		return Conversions.str_to_float(response)
 
 	def clone(self) -> 'CurrentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = CurrentCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Extreme.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/Extreme.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/PrMonotonic/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Margin/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Otolerance.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Otolerance.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/Margin.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/Margin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/Area/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/Upper/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Pmask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Average.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,33 +18,39 @@
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
 			- Max_Spec_Power: float: No parameter help available
-			- Max_Spec_50_Power: float: No parameter help available"""
+			- Max_Spec_50_Power: float: No parameter help available
+			- Ppdu_Power: float: Mean power of the PPDU.
+			- Ppdu_Peak_Power: float: Peak power of the PPDU."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
 			ArgStruct.scalar_float('Max_Spec_Power'),
-			ArgStruct.scalar_float('Max_Spec_50_Power')]
+			ArgStruct.scalar_float('Max_Spec_50_Power'),
+			ArgStruct.scalar_float('Ppdu_Power'),
+			ArgStruct.scalar_float('Ppdu_Peak_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
 			self.Max_Spec_50_Power: float = None
+			self.Ppdu_Power: float = None
+			self.Ppdu_Peak_Power: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:AVERage<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.average.fetch(ppdu = repcap.Ppdu.Nr1) \n
 		Return the current, average, extreme and standard deviation single value power results. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Current.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,33 +32,39 @@
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
 			- Max_Spec_Power: float: No parameter help available
-			- Max_Spec_50_Power: float: No parameter help available"""
+			- Max_Spec_50_Power: float: No parameter help available
+			- Ppdu_Power: float: Mean power of the PPDU.
+			- Ppdu_Peak_Power: float: Peak power of the PPDU."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
 			ArgStruct.scalar_float('Max_Spec_Power'),
-			ArgStruct.scalar_float('Max_Spec_50_Power')]
+			ArgStruct.scalar_float('Max_Spec_50_Power'),
+			ArgStruct.scalar_float('Ppdu_Power'),
+			ArgStruct.scalar_float('Ppdu_Peak_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
 			self.Max_Spec_50_Power: float = None
+			self.Ppdu_Power: float = None
+			self.Ppdu_Peak_Power: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:CURRent<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.current.fetch(ppdu = repcap.Ppdu.Default) \n
 		Return the current, average, extreme and standard deviation single value power results. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/DpPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Dpower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Maximum.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,33 +18,39 @@
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
 			- Max_Spec_Power: float: No parameter help available
-			- Max_Spec_50_Power: float: No parameter help available"""
+			- Max_Spec_50_Power: float: No parameter help available
+			- Ppdu_Power: float: Mean power of the PPDU.
+			- Ppdu_Peak_Power: float: Peak power of the PPDU."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
 			ArgStruct.scalar_float('Max_Spec_Power'),
-			ArgStruct.scalar_float('Max_Spec_50_Power')]
+			ArgStruct.scalar_float('Max_Spec_50_Power'),
+			ArgStruct.scalar_float('Ppdu_Power'),
+			ArgStruct.scalar_float('Ppdu_Peak_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
 			self.Max_Spec_50_Power: float = None
+			self.Ppdu_Power: float = None
+			self.Ppdu_Peak_Power: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MAXimum<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.maximum.fetch(ppdu = repcap.Ppdu.Nr1) \n
 		Return the current, average, extreme and standard deviation single value power results. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Minimum.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,33 +18,39 @@
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
 			- Max_Spec_Power: float: No parameter help available
-			- Max_Spec_50_Power: float: No parameter help available"""
+			- Max_Spec_50_Power: float: No parameter help available
+			- Ppdu_Power: float: Mean power of the PPDU.
+			- Ppdu_Peak_Power: float: Peak power of the PPDU."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
 			ArgStruct.scalar_float('Max_Spec_Power'),
-			ArgStruct.scalar_float('Max_Spec_50_Power')]
+			ArgStruct.scalar_float('Max_Spec_50_Power'),
+			ArgStruct.scalar_float('Ppdu_Power'),
+			ArgStruct.scalar_float('Ppdu_Peak_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
 			self.Max_Spec_50_Power: float = None
+			self.Ppdu_Power: float = None
+			self.Ppdu_Peak_Power: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:MINimum<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.minimum.fetch(ppdu = repcap.Ppdu.Nr1) \n
 		Return the current, average, extreme and standard deviation single value power results. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/StandardDev.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/StandardDev.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,33 +18,39 @@
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Preamble_Power: float: No parameter help available
 			- Pre_Peak_Power: float: No parameter help available
 			- Data_Power: float: No parameter help available
 			- Data_Peak_Power: float: No parameter help available
 			- Max_Spec_Power: float: No parameter help available
-			- Max_Spec_50_Power: float: No parameter help available"""
+			- Max_Spec_50_Power: float: No parameter help available
+			- Ppdu_Power: float: Mean power of the PPDU.
+			- Ppdu_Peak_Power: float: Peak power of the PPDU."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Preamble_Power'),
 			ArgStruct.scalar_float('Pre_Peak_Power'),
 			ArgStruct.scalar_float('Data_Power'),
 			ArgStruct.scalar_float('Data_Peak_Power'),
 			ArgStruct.scalar_float('Max_Spec_Power'),
-			ArgStruct.scalar_float('Max_Spec_50_Power')]
+			ArgStruct.scalar_float('Max_Spec_50_Power'),
+			ArgStruct.scalar_float('Ppdu_Power'),
+			ArgStruct.scalar_float('Ppdu_Peak_Power')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Preamble_Power: float = None
 			self.Pre_Peak_Power: float = None
 			self.Data_Power: float = None
 			self.Data_Peak_Power: float = None
 			self.Max_Spec_Power: float = None
 			self.Max_Spec_50_Power: float = None
+			self.Ppdu_Power: float = None
+			self.Ppdu_Peak_Power: float = None
 
 	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:POWer:SDEViation<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.power.standardDev.fetch(ppdu = repcap.Ppdu.Nr1) \n
 		Return the current, average, extreme and standard deviation single value power results. \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class PowerCls:
-	"""Power commands group definition. 70 total commands, 11 Subgroups, 0 group commands"""
+	"""Power commands group definition. 90 total commands, 13 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("power", core, parent)
 
 	@property
 	def current(self):
@@ -94,14 +94,30 @@
 	def msfPower(self):
 		"""msfPower commands group. 5 Sub-classes, 0 commands."""
 		if not hasattr(self, '_msfPower'):
 			from .MsfPower import MsfPowerCls
 			self._msfPower = MsfPowerCls(self._core, self._cmd_group)
 		return self._msfPower
 
+	@property
+	def ppdu(self):
+		"""ppdu commands group. 5 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ppdu'):
+			from .Ppdu import PpduCls
+			self._ppdu = PpduCls(self._core, self._cmd_group)
+		return self._ppdu
+
+	@property
+	def ppdPeak(self):
+		"""ppdPeak commands group. 5 Sub-classes, 0 commands."""
+		if not hasattr(self, '_ppdPeak'):
+			from .PpdPeak import PpdPeakCls
+			self._ppdPeak = PpdPeakCls(self._core, self._cmd_group)
+		return self._ppdPeak
+
 	def clone(self) -> 'PowerCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = PowerCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Cindex.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Cindex.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/CsLength.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/CsLength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dlength.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dlength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dppdu.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Dppdu.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Drate.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Drate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/FcsCheck.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/FcsCheck.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/AsSymbols.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/AsSymbols.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Bitrate.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Bitrate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,33 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
-from ......Internal.RepeatedCapability import RepeatedCapability
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class BitrateCls:
-	"""Bitrate commands group definition. 2 total commands, 0 Subgroups, 2 group commands
-	Repeated Capability: Pddu, default value after init: Pddu.Nr1"""
+	"""Bitrate commands group definition. 2 total commands, 0 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("bitrate", core, parent)
-		self._cmd_group.rep_cap = RepeatedCapability(self._cmd_group.group_name, 'repcap_pddu_get', 'repcap_pddu_set', repcap.Pddu.Nr1)
 
-	def repcap_pddu_set(self, pddu: repcap.Pddu) -> None:
-		"""Repeated Capability default value numeric suffix.
-		This value is used, if you do not explicitely set it in the child set/get methods, or if you leave it to Pddu.Default
-		Default value after init: Pddu.Nr1"""
-		self._cmd_group.set_repcap_enum_value(pddu)
-
-	def repcap_pddu_get(self) -> repcap.Pddu:
-		"""Returns the current default repeated capability for the child set/get methods"""
-		# noinspection PyTypeChecker
-		return self._cmd_group.get_repcap_enum_value()
-
-	def fetch(self, pddu=repcap.Pddu.Default) -> float:
+	def fetch(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:BITRate<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.phr.bitrate.fetch(pddu = repcap.Pddu.Default) \n
+		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.phr.bitrate.fetch(ppdu = repcap.Ppdu.Nr1) \n
 		Returns the data rate of the PHR. \n
-			:param pddu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Bitrate')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: phr_bitrate: No help available"""
-		pddu_cmd_val = self._cmd_group.get_repcap_cmd_value(pddu, repcap.Pddu)
-		response = self._core.io.query_str(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:BITRate{pddu_cmd_val}?')
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		response = self._core.io.query_str(f'FETCh:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:BITRate{ppdu_cmd_val}?')
 		return Conversions.str_to_float(response)
 
-	def read(self, pddu=repcap.Pddu.Default) -> float:
+	def read(self, ppdu=repcap.Ppdu.Nr1) -> float:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:BITRate<PPDU> \n
-		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.phr.bitrate.read(pddu = repcap.Pddu.Default) \n
+		Snippet: value: float = driver.uwbMeas.multiEval.sinfo.phr.bitrate.read(ppdu = repcap.Ppdu.Nr1) \n
 		Returns the data rate of the PHR. \n
-			:param pddu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Bitrate')
+			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: phr_bitrate: No help available"""
-		pddu_cmd_val = self._cmd_group.get_repcap_cmd_value(pddu, repcap.Pddu)
-		response = self._core.io.query_str(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:BITRate{pddu_cmd_val}?')
+		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
+		response = self._core.io.query_str(f'READ:UWB:MEASurement<Instance>:MEValuation:SINFo:PHR:BITRate{ppdu_cmd_val}?')
 		return Conversions.str_to_float(response)
-
-	def clone(self) -> 'BitrateCls':
-		"""Clones the group by creating new object from it and its whole existing subgroups
-		Also copies all the existing default Repeated Capabilities setting,
-		which you can change independently without affecting the original group"""
-		new_group = BitrateCls(self._core, self._cmd_group.parent)
-		self._cmd_group.synchronize_repcaps(new_group)
-		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/PstGap.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/PstGap.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/RaBit.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/RaBit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/ReBit.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/ReBit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Sfd.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Sfd.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/SfdLength.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/SfdLength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/All.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Average.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self) -> List[float]:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.average.fetch() \n
-		Returns the y-values of the average normalized cross correlation trace. See also 'Normalized Cross Correlation square'. \n
+		Returns the y-values of the average normalized cross-correlation trace. See also 'Normalized Cross Correlation square'. \n
 		Suppressed linked return values: reliability \n
-			:return: correlation: Comma-separated list of cross correlation values."""
+			:return: correlation: Comma-separated list of cross-correlation values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage?', suppressed)
 		return response
 
 	def read(self) -> List[float]:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.average.read() \n
-		Returns the y-values of the average normalized cross correlation trace. See also 'Normalized Cross Correlation square'. \n
+		Returns the y-values of the average normalized cross-correlation trace. See also 'Normalized Cross Correlation square'. \n
 		Suppressed linked return values: reliability \n
-			:return: correlation: Comma-separated list of cross correlation values."""
+			:return: correlation: Comma-separated list of cross-correlation values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,30 @@
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> List[float]:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:CURRent<PPDU> \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the y-values of the current normalized cross correlation trace. See also 'Normalized Cross Correlation square'. \n
+		Returns the y-values of the current normalized cross-correlation trace. See also 'Normalized Cross Correlation square'. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: correlation: Comma-separated list of cross correlation values."""
+			:return: correlation: Comma-separated list of cross-correlation values."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:CURRent{ppdu_cmd_val}?', suppressed)
 		return response
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> List[float]:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:CURRent<PPDU> \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the y-values of the current normalized cross correlation trace. See also 'Normalized Cross Correlation square'. \n
+		Returns the y-values of the current normalized cross-correlation trace. See also 'Normalized Cross Correlation square'. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
-			:return: correlation: Comma-separated list of cross correlation values."""
+			:return: correlation: Comma-separated list of cross-correlation values."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:CURRent{ppdu_cmd_val}?', suppressed)
 		return response
 
 	def clone(self) -> 'CurrentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/Xvalues.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("xvalues", core, parent)
 
 	def fetch(self) -> List[float]:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.xvalues.fetch() \n
-		Returns the x-values of the normalized cross correlation trace. \n
+		Returns the x-values of the normalized cross-correlation trace. \n
 		Suppressed linked return values: reliability \n
 			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues?', suppressed)
 		return response
 
 	def read(self) -> List[float]:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.ncCorr.xvalues.read() \n
-		Returns the x-values of the normalized cross correlation trace. \n
+		Returns the x-values of the normalized cross-correlation trace. \n
 		Suppressed linked return values: reliability \n
 			:return: values: Comma-separated list of time values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:NCCorr:XVALues?', suppressed)
 		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/NcCorr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Pmask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Maximum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Minimum.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/PowerVsTime/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbwl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/Sbws/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/SpJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/StJitter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Average.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	def fetch(self) -> List[float]:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.average.fetch() \n
-		Returns the y-values of the average transmit spectrum trace. See also 'Transmit Spectrum Mask square'. \n
+		Returns the y-values of the average transmit spectrum trace. See also 'Narrowband results'. \n
 		Suppressed linked return values: reliability \n
 			:return: ratio: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage?', suppressed)
 		return response
 
 	def read(self) -> List[float]:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.average.read() \n
-		Returns the y-values of the average transmit spectrum trace. See also 'Transmit Spectrum Mask square'. \n
+		Returns the y-values of the average transmit spectrum trace. See also 'Narrowband results'. \n
 		Suppressed linked return values: reliability \n
 			:return: ratio: Comma-separated list of power values."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Current.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 		"""Returns the current default repeated capability for the child set/get methods"""
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def fetch(self, ppdu=repcap.Ppdu.Default) -> List[float]:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent<PPDU> \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.current.fetch(ppdu = repcap.Ppdu.Default) \n
-		Returns the y-values of the current transmit spectrum trace. See also 'Transmit Spectrum Mask square'. \n
+		Returns the y-values of the current transmit spectrum trace. See also 'Narrowband results'. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: ratio: Comma-separated list of power values."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent{ppdu_cmd_val}?', suppressed)
 		return response
 
 	def read(self, ppdu=repcap.Ppdu.Default) -> List[float]:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent<PPDU> \n
 		Snippet: value: List[float] = driver.uwbMeas.multiEval.trace.tsMask.current.read(ppdu = repcap.Ppdu.Default) \n
-		Returns the y-values of the current transmit spectrum trace. See also 'Transmit Spectrum Mask square'. \n
+		Returns the y-values of the current transmit spectrum trace. See also 'Narrowband results'. \n
 		Suppressed linked return values: reliability \n
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: ratio: Comma-separated list of power values."""
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:UWB:MEASurement<Instance>:MEValuation:TRACe:TSMask:CURRent{ppdu_cmd_val}?', suppressed)
 		return response
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Xvalues.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/Xvalues.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/TsMask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Average.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 			self.Margin_Avg_Neg_Y: enums.ResultStatus2 = None
 			self.Margin_Avg_Pos_Y: enums.ResultStatus2 = None
 
 	def calculate(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> CalculateStruct:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:AVERage<PPDU> \n
 		Snippet: value: CalculateStruct = driver.uwbMeas.multiEval.tsMask.margin.area.average.calculate(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
 		Returns the limit check results for the current and average traces, for the transmit spectrum mask area <no>. See also
-		'Transmit Spectrum Mask square'. \n
+		'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:AVERage{ppdu_cmd_val}?', self.__class__.CalculateStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 			self.Margin_Curr_Neg_Y: enums.ResultStatus2 = None
 			self.Margin_Curr_Pos_Y: enums.ResultStatus2 = None
 
 	def calculate(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Default) -> CalculateStruct:
 		"""SCPI: CALCulate:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:CURRent<PPDU> \n
 		Snippet: value: CalculateStruct = driver.uwbMeas.multiEval.tsMask.margin.area.current.calculate(area = repcap.Area.Default, ppdu = repcap.Ppdu.Default) \n
 		Returns the limit check results for the current and average traces, for the transmit spectrum mask area <no>. See also
-		'Transmit Spectrum Mask square'. \n
+		'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'CALCulate:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:CURRent{ppdu_cmd_val}?', self.__class__.CalculateStruct())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 			self.Margin_Aver_Neg_Y: float = None
 
 	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:AVERage<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.average.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with negative
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:AVERage<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.average.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with negative
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Current.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,28 +45,28 @@
 			self.Margin_Curr_Neg_Y: float = None
 
 	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Default) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:CURRent<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.current.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Default) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with negative
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Default) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:NEGativ:CURRent<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.negativ.current.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Default) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with negative
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:NEGativ:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 			self.Margin_Aver_Pos_Y: float = None
 
 	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:AVERage<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.average.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with positive
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Nr1) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:AVERage<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.average.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Nr1) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with positive
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:AVERage{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Current.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,28 @@
 			self.Margin_Curr_Pos_Y: float = None
 
 	def fetch(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Default) -> ResultData:
 		"""SCPI: FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:CURRent<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.current.fetch(area = repcap.Area.Default, ppdu = repcap.Ppdu.Default) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with positive
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'FETCh:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
 
 	def read(self, area=repcap.Area.Default, ppdu=repcap.Ppdu.Default) -> ResultData:
 		"""SCPI: READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA<nr>:POSitiv:CURRent<PPDU> \n
 		Snippet: value: ResultData = driver.uwbMeas.multiEval.tsMask.margin.area.positiv.current.read(area = repcap.Area.Default, ppdu = repcap.Ppdu.Default) \n
 		Returns the margin values between the result trace and the transmit spectrum mask for the area <no> with positive
 		frequency offset. A negative margin indicates that the trace is located above the limit line, i.e. the limit is exceeded.
-		The current and average values can be retrieved. See also 'Transmit Spectrum Mask square'. \n
+		The current and average values can be retrieved. See also 'Narrowband results'. \n
 			:param area: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Area')
 			:param ppdu: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Current')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		area_cmd_val = self._cmd_group.get_repcap_cmd_value(area, repcap.Area)
 		ppdu_cmd_val = self._cmd_group.get_repcap_cmd_value(ppdu, repcap.Ppdu)
 		return self._core.io.query_struct(f'READ:UWB:MEASurement<Instance>:MEValuation:TSMask:MARGin:AREA{area_cmd_val}:POSitiv:CURRent{ppdu_cmd_val}?', self.__class__.ResultData())
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Otolerance.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Otolerance.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class TsMaskCls:
-	"""TsMask commands group definition. 12 total commands, 2 Subgroups, 0 group commands"""
+	"""TsMask commands group definition. 17 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("tsMask", core, parent)
 
 	@property
 	def margin(self):
@@ -22,14 +22,22 @@
 	def otolerance(self):
 		"""otolerance commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_otolerance'):
 			from .Otolerance import OtoleranceCls
 			self._otolerance = OtoleranceCls(self._core, self._cmd_group)
 		return self._otolerance
 
+	@property
+	def tdbBandwidth(self):
+		"""tdbBandwidth commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_tdbBandwidth'):
+			from .TdbBandwidth import TdbBandwidthCls
+			self._tdbBandwidth = TdbBandwidthCls(self._core, self._cmd_group)
+		return self._tdbBandwidth
+
 	def clone(self) -> 'TsMaskCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = TsMaskCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MultiEvalCls:
-	"""MultiEval commands group definition. 465 total commands, 8 Subgroups, 3 group commands"""
+	"""MultiEval commands group definition. 494 total commands, 9 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("multiEval", core, parent)
 
 	@property
 	def state(self):
@@ -24,15 +24,15 @@
 		if not hasattr(self, '_ddecoding'):
 			from .Ddecoding import DdecodingCls
 			self._ddecoding = DdecodingCls(self._core, self._cmd_group)
 		return self._ddecoding
 
 	@property
 	def tsMask(self):
-		"""tsMask commands group. 2 Sub-classes, 0 commands."""
+		"""tsMask commands group. 3 Sub-classes, 0 commands."""
 		if not hasattr(self, '_tsMask'):
 			from .TsMask import TsMaskCls
 			self._tsMask = TsMaskCls(self._core, self._cmd_group)
 		return self._tsMask
 
 	@property
 	def modulation(self):
@@ -40,15 +40,15 @@
 		if not hasattr(self, '_modulation'):
 			from .Modulation import ModulationCls
 			self._modulation = ModulationCls(self._core, self._cmd_group)
 		return self._modulation
 
 	@property
 	def power(self):
-		"""power commands group. 11 Sub-classes, 0 commands."""
+		"""power commands group. 13 Sub-classes, 0 commands."""
 		if not hasattr(self, '_power'):
 			from .Power import PowerCls
 			self._power = PowerCls(self._core, self._cmd_group)
 		return self._power
 
 	@property
 	def sinfo(self):
@@ -63,50 +63,58 @@
 		"""pmask commands group. 4 Sub-classes, 0 commands."""
 		if not hasattr(self, '_pmask'):
 			from .Pmask import PmaskCls
 			self._pmask = PmaskCls(self._core, self._cmd_group)
 		return self._pmask
 
 	@property
+	def stsSequence(self):
+		"""stsSequence commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_stsSequence'):
+			from .StsSequence import StsSequenceCls
+			self._stsSequence = StsSequenceCls(self._core, self._cmd_group)
+		return self._stsSequence
+
+	@property
 	def trace(self):
 		"""trace commands group. 10 Sub-classes, 0 commands."""
 		if not hasattr(self, '_trace'):
 			from .Trace import TraceCls
 			self._trace = TraceCls(self._core, self._cmd_group)
 		return self._trace
 
 	def initiate(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:UWB:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.uwbMeas.multiEval.initiate() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
-			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
-			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
-			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
+			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
+			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
+			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'INITiate:UWB:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
 	def stop(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:UWB:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.uwbMeas.multiEval.stop() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
-			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
-			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
-			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
+			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
+			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
+			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'STOP:UWB:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
 	def abort(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:UWB:MEASurement<Instance>:MEValuation \n
 		Snippet: driver.uwbMeas.multiEval.abort() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
-			- INITiate... starts or restarts the measurement. The measurement enters the 'RUN' state.
-			- STOP... halts the measurement immediately. The measurement enters the 'RDY' state. Measurement results are kept. The resources remain allocated to the measurement.
-			- ABORt... halts the measurement immediately. The measurement enters the 'OFF' state. All measurement values are set to NAV. Allocated resources are released.
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
+			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
+			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
+			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'ABORt:UWB:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
 	def clone(self) -> 'MultiEvalCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Implementations/UwbMeas/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Implementations/UwbMeas/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class UwbMeasCls:
-	"""UwbMeas commands group definition. 465 total commands, 1 Subgroups, 0 group commands"""
+	"""UwbMeas commands group definition. 494 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("uwbMeas", core, parent)
 
 	@property
 	def multiEval(self):
-		"""multiEval commands group. 8 Sub-classes, 3 commands."""
+		"""multiEval commands group. 9 Sub-classes, 3 commands."""
 		if not hasattr(self, '_multiEval'):
 			from .MultiEval import MultiEvalCls
 			self._multiEval = MultiEvalCls(self._core, self._cmd_group)
 		return self._multiEval
 
 	def clone(self) -> 'UwbMeasCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingle.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgSingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleList.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgSingleList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStringComposer.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStringComposer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStruct.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStruct.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructList.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStructList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ArgStructStringParser.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/CommandsGroup.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/CommandsGroup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Conversions.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import math
 import struct
 import sys
 from enum import Enum
 from typing import List, Tuple
 from .ScpiEnums import ScpiEnum, enum_spec_prefixes, enum_spec_strings
+from .Properties import Properties
 from datetime import datetime
 
 from . import Utilities
 from .InstrumentErrors import RsInstrException
 
 
 class BinFloatFormat(Enum):
@@ -198,15 +199,20 @@
 
 
 number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
 number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
 number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
 number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
 number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
-number_si_suffix = {'pHz': 1E-12, 'MHz': 1E+6, 'kHz': 1E+3, 'GHz': 1E+9, 'mHz': 1E-3, 'uHz': 1E-6, 'µHz': 1E-6, 'THz': 1E+12, 'nHz': 1E-9, 'ns': 1E-9, 'fW': 1E-15, 'pW': 1E-12, 'nW': 1E-9, 'uW': 1E-6, 'µW': 1E-6, 'mW': 1E-3, 'kW': 1E3, 'MW': 1E6, 'GW': 1E9, 'MV': 1E+6, 'MA': 1E+6, 'ps': 1E-12, 'fs':1E-15, 'km': 1E+3, 'kV': 1E+3, 'kA': 1E+3, 'pF': 1E-2, 'Hz': 1.0, 'mm': 1E-3, 'mA': 1E-3, 'mF': 1E-3, 'mV': 1E-3, 'pV': 1E-12, 'nF': 1E-9, 'nA': 1E-9, 'nV': 1E-9, 'nm': 1E-9, 'pm': 1E-12, 'us': 1E-6, 'µs': 1E-6, 'uF': 1E-6, 'µF': 1E-6, 'ms': 1E-3, 'uA': 1E-6, 'µA': 1E-6, 'uV': 1E-6, 'µV': 1E-6, 'um': 1E-6, 'µm': 1E-6, 'pA': 1E-12, 'V': 1, 'W': 1, 'A': 1, 'F': 1, 's': 1, 'm': 1}
+number_si_suffix = {
+	'pHz': 1E-12, 'MHz': 1E+6, 'kHz': 1E+3, 'GHz': 1E+9, 'mHz': 1E-3, 'uHz': 1E-6, 'µHz': 1E-6, 'THz': 1E+12, 'nHz': 1E-9, 'ns': 1E-9, 'fW': 1E-15,
+	'pW': 1E-12, 'nW': 1E-9, 'uW': 1E-6, 'µW': 1E-6, 'mW': 1E-3, 'kW': 1E3, 'MW': 1E6, 'GW': 1E9, 'MV': 1E+6, 'MA': 1E+6, 'ps': 1E-12, 'fs': 1E-15,
+	'km': 1E+3, 'kV': 1E+3, 'kA': 1E+3, 'pF': 1E-2, 'Hz': 1.0, 'mm': 1E-3, 'mA': 1E-3, 'mF': 1E-3, 'mV': 1E-3, 'pV': 1E-12, 'nF': 1E-9, 'nA': 1E-9,
+	'nV': 1E-9, 'nm': 1E-9, 'pm': 1E-12, 'us': 1E-6, 'µs': 1E-6, 'uF': 1E-6, 'µF': 1E-6, 'ms': 1E-3, 'uA': 1E-6, 'µA': 1E-6, 'uV': 1E-6, 'µV': 1E-6,
+	'um': 1E-6, 'µm': 1E-6, 'pA': 1E-12, 'V': 1, 'W': 1, 'A': 1, 'F': 1, 's': 1, 'm': 1}
 int_neg_inf = -(sys.maxsize - 1)
 
 
 def strip_si_suffix(string: str) -> Tuple[bool, str, float]:
 	"""Tries to find defined suffixes in the text and returns the stripped text and the multiplier as double number.
 	If no known suffix is detected, the method returns false, strippedText=text, multiplier=1.0
 	Example: text='123 MHz' strippedText='123' multiplier=1E6"""
@@ -358,15 +364,15 @@
 	else:
 		raise RsInstrException(f"bool_to_str: unsupported variable type '{type(value)}', value '{value}'. Only boolean values are supported.")
 
 
 def str_enclose_by_quotes(string: str) -> str:
 	"""Returns string enclosed by single quotes."""
 	assert_string_data(string)
-	return "'" + string + "'"
+	return Properties.scpi_quotes + string + Properties.scpi_quotes
 
 
 def list_to_csv_str(value: List, delimiter: str = ',') -> str:
 	"""Converts list of elements to strings separated by commas.
 	Element types can differ on an individual basis.
 	Supported element types:
 	- int
@@ -476,15 +482,15 @@
 	"""Converts scalar value to string enclosed by single quotes.
 	Supported element types:
 	- int
 	- bool
 	- float
 	- string
 	- enum"""
-	return f"'{value_to_str(x)}'"
+	return Properties.scpi_quotes + value_to_str(x) + Properties.scpi_quotes
 
 
 def str_to_float_list(string: str) -> List[float]:
 	"""Converts string with comma-separated values to list of Floats."""
 	assert_string_data(string)
 	if not string:
 		return []
@@ -570,15 +576,15 @@
 	# noinspection PyTypeChecker
 	return Utilities.trim_str_response(string)
 
 
 def str_to_simple_scalar_enum(string: str, enum_type, case_sensitive: bool = True, ignore_underscores: bool = False) -> Enum or None:
 	"""Converts string to one enum element.
 	Does not handle special value or non-mandatory parts.
-	Function is used in core only for standard enum conversions, not for SCPI enum conversions."""
+	The function is used in core only for standard enum conversions, not for SCPI enum conversions."""
 	value = Utilities.trim_str_response(string)
 	enum_members = [x.name for x in enum_type]
 	enum_members_mod = [x.name for x in enum_type]
 	if not case_sensitive:
 		enum_members_mod = [x.upper() for x in enum_members]
 		value = value.upper()
 	if ignore_underscores:
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ConverterFromScpiString.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	For list argument types, you must use the method get_one_element_value in a loop for each element.
 	Provides methods:
 	- get_one_element_value(str): returns one scalar value converted from the SCPI string.
 	- get_list_value(str): return complete list value converted from the SCPI string.
 	- get_value(str): calls either get_one_element_value or get_list_value() depending on the data type. \n
 	The reason for the different methods is, that sometimes the list data are interleaved with other arguments.
 	In order to parse them properly, the ArgStructStringParser module must be able to set the argument value element-by-element.
-	On the other side, the driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
+	The driver methods might want to set the whole argument value, because the result scpi string is a single argument response."""
 
 	def __init__(self, data_type: DataType, enum_type: Enum = None):
 		self.scpi_enum = None
 		self.data_type = data_type
 		self.element_type = self.data_type.element_type
 
 		if self.element_type == DataType.RawString:
@@ -58,22 +58,21 @@
 			assert enum_type, f"For data type enum, you have to define the enum_type variable."
 			# noinspection PyTypeChecker
 			self.scpi_enum = ScpiEnum(enum_type)
 		else:
 			raise RsInstrException(f"Unsupported data type '{data_type}'")
 
 	def get_one_element_value(self, scpi_string: str):
-		"""Returns single element !!! of the argument value converted from the SCPI string (single element)"""
+		"""Returns single element (not an array!!!) of the argument value converted from the SCPI string (single element)"""
 		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
 		if self.element_type.is_scalar_enum:
 			return str_to_scalar_enum_helper(scpi_string, self.scpi_enum, False, exc_if_not_found=self.element_type == DataType.Enum)
 		return self.converter(scpi_string)
 
 	def get_value(self, scpi_string: str):
 		"""Returns complete value of the argument converted from the SCPI string (list or scalar)"""
 		if not self.data_type.is_list:
 			return self.get_one_element_value(scpi_string)
-
 		assert isinstance(scpi_string, str), f"Input parameter scpi_string must be string. Actual parameter: {type(scpi_string)}, value: {scpi_string}"
 		if self.element_type is DataType.Enum:
 			return str_to_list_enum_helper(scpi_string, self.scpi_enum, exc_if_not_found=self.element_type == DataType.Enum)
 		return self.list_converter(scpi_string)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ConverterToScpiString.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from enum import Enum
 
 from .Conversions import list_to_csv_quoted_str, value_to_quoted_str, list_to_csv_str, value_to_str, enum_list_to_str, enum_scalar_to_str, enum_ext_scalar_to_str, enum_ext_list_to_str
 from .Types import DataType
 from .InstrumentErrors import RsInstrException
 
 
-def value_to_scpi_string(data, data_type: DataType):
-	"""Method to be used in the driver implementation.
-	Convert data to SCPI string parameter: data -> str.
+def value_to_scpi_string(data, data_type: DataType) -> str:
+	"""Convert data to SCPI string parameter: data -> str.
 	Does not work with enum data types."""
 	if data_type.is_list:
 		assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
 	else:
 		assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
 	# Strings are enclosed by single quotes
 	if data_type == DataType.StringList:
@@ -71,18 +70,16 @@
 
 	def get_value(self, data) -> str:
 		"""Returns SCPI string converted from the argument data."""
 		if self.data_type.is_list:
 			assert isinstance(data, list), f"Expected command parameter list, actual data type: {type(data)}. Value: {data}"
 		else:
 			assert not isinstance(data, list), f"Expected command parameter scalar, actual data type: {type(data)}. Value: {data}"
-
 		if self.data_type == DataType.Enum:
 			return enum_scalar_to_str(data, self.enum_type)
 		if self.data_type == DataType.EnumExt:
 			return enum_ext_scalar_to_str(data, self.enum_type)
 		if self.data_type == DataType.EnumList:
 			return enum_list_to_str(data, self.enum_type)
 		if self.data_type == DataType.EnumExtList:
 			return enum_ext_list_to_str(data, self.enum_type)
-
 		return value_to_scpi_string(data, self.data_type)
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Core.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Core.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,44 @@
 from typing import Callable
 
 from . import InstrumentOptions as Options
 from .ArgSingle import ArgSingle
 from .ArgSingleList import ArgSingleList
 from .Conversions import BinFloatFormat, BinIntFormat
 from .Instrument import Instrument
-from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode
+from .InstrumentSettings import InstrViClearMode, InstrumentSettings, WaitForOpcMode, OpcSyncQueryMechanism
 from .ScpiLogger import LoggingMode
 from .InstrumentErrors import RsInstrException
+from .Properties import Properties
 
 
 class Core(object):
 	"""Main driver component. Provides: \n
 		- Main core constructor
 		- 'io' interface for all the write / query operations
 		- Command parameters string composer for single arguments...
 		- Link handlers adding / changing / deleting
 
 		Version history:
 
+		1.70.0 (27.02.2024)
+			- Added settings profile 'XK41' for R&S Software Defined Radios.
+			- Added settings 'FirstCmds' where you can send the defined commands right after the init. Send more commands in a row with ';;' separator.
+			- Added settings 'EachCmdPrefix' - this prefix is added to each command sent to the instrument. Supported values are also 'lf', 'cr', 'tab'
+
+		1.60.0 (31.01.2024)
+			- Added Properties script for global properties.
+			- Added Properties.scpi_quotes, string option settings token: 'ScpiQuotes'. Example: ScpiQuotes=double. Default: Single
+			- Fixed VisaPluginSocketIo read() method for cases where the session is lost. The method now generates exception in that case.
+			- Added settings 'OpcSyncQueryMechanism' with values: Standard, AlsoCheckMav, ClsOnlyCheckMavErrQueue, OnlyCheckMavErrQueue
+
+		1.54.0 (27.06.2023)
+			- Added new options profile for ATS chambers.
+			- Added settings boolean token EachCmdAsQuery. Example: EachCmdAsQuery=True. Default: False
+
 		1.53.0 (18.10.2022)
 			- Improved mode where the instrument works with a session from another object.
 			- Silently ignoring invalid *IDN? string.
 			- Added new options profile 'Minimal' for non-SCPI-99 instruments.
 
 		1.52.0 (28.09.2022)
 			- Fixed DisableOpcQuery=True settings effect.
@@ -171,15 +187,15 @@
 			reset: bool = False,
 			driver_options: str = None,
 			user_options: str = None,
 			direct_session: object = None):
 		"""Initializes new driver session. For cleaner code, use the class methods: \n
 		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
 
-		self.core_version = '1.53.0'
+		self.core_version = '1.55.0'
 		self.resource_name = resource_name
 
 		# Typical settings for the Core
 		self._instrumentSettings = InstrumentSettings(
 			InstrViClearMode.execute_on_all,  # Instrument viClear mode
 			False,  # Full model name. True: SMW200A, False: SMW
 			0,  # Delay by each write
@@ -189,15 +205,17 @@
 			30000,  # OPC timeout
 			10000,  # VISA timeout
 			60000,  # Self-test timeout
 			Options.ParseMode.Auto,  # *OPT? response parsing mode
 			BinFloatFormat.Single_4bytes,  # Format for parsing of binary float numbers
 			BinIntFormat.Integer32_4bytes,  # Format for parsing of binary integer numbers
 			False,  # OPC query after each setting
-			LoggingMode.Off  # Logging mode
+			LoggingMode.Off,
+			OpcSyncQueryMechanism.only_check_mav_err_queue
+			# Logging mode
 		)
 
 		self._instrumentSettings.apply_option_settings(driver_options)
 		self._instrumentSettings.apply_option_settings(user_options)
 
 		self.simulating = self._instrumentSettings.simulating
 		self.supported_idn_patterns = self._instrumentSettings.supported_idn_patterns
@@ -208,14 +226,15 @@
 		self.io = Instrument(self.resource_name, self.simulating, self._instrumentSettings, handle)
 		self.io.query_instr_status = True
 		# Update the resource name if it changed, for example because of the direct session
 		self.resource_name = self.io.resource_name
 		self.allow_reconnect = self.io.allow_reconnect
 
 		self._apply_settings_to_instrument(self._instrumentSettings)
+		self._apply_global_properties(self._instrumentSettings)
 		self.io.set_simulating_cmds()
 
 		if id_query:
 			self.io.fits_idn_pattern(self.supported_idn_patterns, self.supported_instr_models)
 
 		if reset:
 			self.io.reset()
@@ -271,14 +290,20 @@
 	def _apply_settings_to_instrument(self, settings: InstrumentSettings) -> None:
 		"""Applies settings relevant for the Instrument from the InstrumentSettings structure."""
 		if settings.instrument_status_check is not None:
 			self.io.query_instr_status = settings.instrument_status_check
 		if self.simulating and settings.instrument_simulation_idn_string is not None:
 			self.io.idn_string = settings.instrument_simulation_idn_string
 
+	@staticmethod
+	def _apply_global_properties(settings: InstrumentSettings) -> None:
+		"""Applies settings valid for the entire module. All are available in the module 'Properties'."""
+		if settings.scpi_quotes is not None:
+			Properties.scpi_quotes = settings.scpi_quotes
+
 	def compose_cmd_arg_param(
 			self, arg1: ArgSingle, arg2: ArgSingle = None, arg3: ArgSingle = None, arg4: ArgSingle = None, arg5: ArgSingle = None, arg6: ArgSingle = None) -> str:
 		"""Composes command parameter string based on the single argument definition."""
 		return self._args_single_list.compose_cmd_string(arg1, arg2, arg3, arg4, arg5, arg6)
 
 	def get_last_sent_cmd(self) -> str:
 		"""Returns the last commands sent to the instrument. Only works in simulation mode"""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/GlobalData.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/GlobalData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Instrument.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 		self._instr_options: InstrumentOptions = None  # Internal private property for the lazy property self.instr_options - see the getter for self.instr_options. Initialized by the first access
 		self.query_instr_status: bool = True
 		self.opc_query_after_write: bool = False
 		self.bin_float_numbers_format = self._settings.bin_float_numbers_format
 		self.bin_int_numbers_format = self._settings.bin_int_numbers_format
 		self.opc_query_after_write: bool = self._settings.opc_query_after_write
 		self.stb_in_error_check: bool = self._settings.stb_in_error_check
+		self.each_cmd_as_query: bool = self._settings.each_cmd_as_query
 
 		self.manufacturer: str = 'Rohde&Schwarz'
 		self.model: str = 'R&S Instrument'
 		self.serial_number: str = '100001'
 		self.firmware_version: str = '1.00'
 
 		direct_start_time = datetime.now()
@@ -85,21 +86,34 @@
 
 			self._set_session(VisaSession(resource_name, self._settings, direct_session))
 			self._init_logger(self._session.resource_name)
 			self._log_start_segment(direct_start_time)
 
 			self._lock = self._session.get_lock()
 			with self._lock:
-				self._session.clear_before_read()
-				self.idn_string = Utilities.trim_str_response(self._session.query_str(self._session.cmd_idn)).strip()
+				self.idn_string = ''
+				if len(self._session.cmd_idn) > 0:
+					self._session.clear_before_read()
+					resp = Utilities.trim_str_response(self._session.query_str(self._session.cmd_idn)).strip()
+					if settings.idn_custom_parse:
+						sr = settings.idn_custom_parse.split('->')
+						search = sr[0]
+						replace = sr[1]
+						resp = re.sub(search, replace, resp)
+					self.idn_string = resp
+				else:
+					self.idn_string = "Rohde&Schwarz,DefaultDevice,100001,1.00"
+
 				# NRP-Z session coercing
 				if self._session.is_rsnrp_session():
 					self._settings.instr_options_parse_mode = InstrumentOptions.ParseMode.Skip
 					self.stb_in_error_check = False
+
 				self.instr_options_parse_mode = self._settings.instr_options_parse_mode
+
 			self._log_info('Session init', f"Device{dir_str} '{self.resource_name}' IDN: {self.idn_string}")
 
 		except RsInstrException as e:
 			if not self.logger:
 				self._assure_logger_exists()
 				self._log_start_segment(direct_start_time)
 			self._log_error('Session init error', e.args[0], self._start_time, datetime.now())
@@ -232,14 +246,22 @@
 		"""Returns the current RLock object."""
 		return self._lock
 
 	def clear_lock(self):
 		"""Clears the existing thread lock, making the current session thread-independent from others that might share the current thread lock."""
 		self.assign_lock(threading.RLock())
 
+	def lock_resource(self, timeout: int, requested_key: str or bytes = None) -> bytes or None:
+		"""Locks the instrument to prevent it from communicating with other clients."""
+		return self._session.lock_resource(timeout, requested_key)
+
+	def unlock_resource(self) -> None:
+		"""Unlocks the instrument to other clients."""
+		self._session.unlock_resource()
+
 	def _log_start_segment(self, direct_start_time: datetime = None):
 		"""Sets start time for the log entry to be able to calculate the duration. You can enter a direct start time."""
 		self._last_error_log = None
 		if direct_start_time:
 			self._start_time = direct_start_time
 		else:
 			self._start_time = datetime.now()
@@ -376,14 +398,24 @@
 		self._session.visa_timeout = value
 
 	@property
 	def data_chunk_size(self) -> int:
 		"""Returns max chunk size of one data block."""
 		return self._session.data_chunk_size
 
+	@property
+	def opc_sync_query_mechanism(self) -> InstrumentSettings.OpcSyncQueryMechanism:
+		"""Returns the current setting of the OPC-Sync query mechanism."""
+		return self._session.opc_sync_query_mechanism
+
+	@opc_sync_query_mechanism.setter
+	def opc_sync_query_mechanism(self, mechanism: InstrumentSettings.OpcSyncQueryMechanism) -> None:
+		"""Sets the current setting of the OPC-Sync query mechanism."""
+		self._session.opc_sync_query_mechanism = mechanism
+
 	@data_chunk_size.setter
 	def data_chunk_size(self, chunk_size: int) -> None:
 		"""Sets the maximum size of one block transferred during write/read operations."""
 		self._session.data_chunk_size = int(chunk_size)
 
 	# noinspection PyMethodMayBeStatic
 	def _sim_cached_value_found(self, value) -> bool:
@@ -426,15 +458,16 @@
 		if items_count >= 4:
 			self.firmware_version = Utilities.trim_str_response(items[3].strip())
 
 	def fits_idn_pattern(self, patterns: List[str], supported_models: List[str]) -> None:
 		"""Throws exception if the current instrument model does not fit  any of the patterns.
 		The supported_models argument is only used for exception messages"""
 		matches = False
-		assert self._idn_string, f'*IDN? was not assigned yet.'
+		if not self._idn_string:
+			return
 		for x in patterns:
 			matches = re.search(x, self.idn_string, re.IGNORECASE)
 			if matches:
 				break
 		if not matches:
 			message = f"Instrument is not supported.\n*IDN? string: '{self.idn_string}'"
 			if len(supported_models) > 0:
@@ -618,14 +651,18 @@
 				self._log_end_segment()
 		finally:
 			if old_tout > 0:
 				self.visa_timeout = old_tout
 
 	def write(self, cmd: str, block_callback: bool = False, log_info: str = 'Write') -> None:
 		"""Writes string command to the instrument."""
+		if self.each_cmd_as_query:
+			self.query_str(cmd, block_callback, log_info)
+			return
+
 		with self._lock:
 			try:
 				self._log_start_segment()
 				cmd = self._replace_global_repcaps(cmd)
 				self._call_before_write_handler(cmd, block_callback)
 				self._session.write(cmd)
 				if self.opc_query_after_write:
@@ -640,14 +677,17 @@
 			finally:
 				self._log_end_segment()
 
 	def write_with_opc(self, cmd: str, timeout: int = None, block_callback: bool = False, log_info: str = 'Write string with OPC') -> None:
 		"""Writes a OPC-synced command.
 		Also performs error checking if the property self.query_instr_status is set to True.
 		If you do not provide timeout, the method uses current opc_timeout."""
+		if self.each_cmd_as_query:
+			self.query_str_with_opc(cmd, timeout, block_callback, log_info)
+			return
 		with self._lock:
 			try:
 				self._log_start_segment()
 				cmd = self._replace_global_repcaps(cmd)
 				self._call_before_write_handler(cmd, block_callback)
 				self._session.write_with_opc(cmd, timeout)
 				self._session.query_and_clear_esr()
@@ -707,15 +747,16 @@
 			try:
 				self._log_start_segment()
 				query = self._replace_global_repcaps(query)
 				self.start_send_read_event(query, True)
 				self._call_pre_query_handler(query, block_callback)
 				response = self._session.query_str_with_opc(query, timeout, log_info)
 				self.end_send_read_event()
-				self._session.query_and_clear_esr()
+				if self._session.clear_status_after_query_with_opc():
+					self._session.query_and_clear_esr()
 				self._log_info(log_info, f'{query} {response}')
 				self.check_status()
 			except RsInstrException as e:
 				self._log_exception(e, log_info)
 				raise
 			finally:
 				self._log_end_segment()
@@ -802,15 +843,16 @@
 
 					self._log_start_segment()
 					query = self._replace_global_repcaps(query)
 					self.start_send_read_event(query, True)
 					self._call_pre_query_handler(query, False)
 					self._session.query_bin_block_with_opc(query, stream, True, timeout)
 					self.end_send_read_event()
-					self._session.query_and_clear_esr()
+					if self._session.clear_status_after_query_with_opc():
+						self._session.query_and_clear_esr()
 					add_str = 'target file' if append is False else 'appended to target file'
 					self._log_info(log_info, f'Query {query} - written {size_to_kb_mb_string(stream.written_len, True)}, {add_str} {file_path}')
 					self.check_status()
 				except RsInstrException as e:
 					self._log_exception(e, log_info)
 					raise
 				finally:
@@ -1031,15 +1073,16 @@
 					return [0.1, 1.2, 2.3, 3.4, 4.5, 5.6, 6.7, 7.8, 8.9, 9.1, 10.2]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_floats(stream.content, self.bin_float_numbers_format)
 					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
 				else:
 					result = Conv.str_to_float_list(stream.content)
 					self._log_info_list(f'{log_info}, received ascii format list', result)
-				self._session.query_and_clear_esr()
+				if self._session.clear_status_after_query_with_opc():
+					self._session.query_and_clear_esr()
 				self.check_status()
 				return result
 			except RsInstrException as e:
 				self._log_exception(e, log_info)
 				raise
 			finally:
 				self._log_end_segment()
@@ -1114,15 +1157,16 @@
 					return [1, 2, 3, 5, 10, 15, 20, 30, 50, 100]
 				if stream.binary:
 					result = Conv.bytes_to_list_of_integers(stream.content, self.bin_int_numbers_format)
 					self._log_info_list(f'{log_info}, received binary format list {size_to_kb_mb_string(stream.written_len, True)} {stream.written_len // len(result)} bytes per number', result)
 				else:
 					result = Conv.str_to_int_list(stream.content)
 					self._log_info_list(f'{log_info}, received ascii format list', result)
-				self._session.query_and_clear_esr()
+				if self._session.clear_status_after_query_with_opc():
+					self._session.query_and_clear_esr()
 				self.check_status()
 				return result
 			except RsInstrException as e:
 				self._log_exception(e, log_info)
 				raise
 			finally:
 				self._log_end_segment()
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentErrors.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InstrumentErrors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentOptions.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InstrumentOptions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InstrumentSettings.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InstrumentSettings.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 	"""Mode that is used for OPC-sync commands/queries"""
 	stb_poll = 1
 	stb_poll_slow = 2
 	stb_poll_superslow = 3
 	opc_query = 4
 
 
+class OpcSyncQueryMechanism(Enum):
+	"""Mechanism to use when querying with OPC."""
+	standard = 0  # Sends the command with ;*OPC at the end, and waits for the ESB or ERRQ bits.
+	also_check_mav = 1  # Same as Standard, but for queries additionally ends the OPC-waiting queue on MAV bit set to 1.
+	cls_only_check_mav_err_queue = 2  # ClearBeforeRead, does not send the ;*OPC as the command suffix. In the wait loop, checks the MAV and ERRQ.
+	only_check_mav_err_queue = 3  # Same as above, but skips the ClearBeforeRead()
+
+
 class InstrumentSettings(object):
 	"""Defines settings of the instrument session."""
 
 	def __init__(
 			self,
 			viclear_exe_mode: InstrViClearMode,
 			idn_model_full_name: bool,
@@ -45,29 +53,32 @@
 			opc_timeout: int,
 			visa_timeout: int,
 			self_test_timeout: int,
 			instr_options_parse_mode: Opts.ParseMode,
 			bin_float_numbers_format: Conv.BinFloatFormat,
 			bin_int_numbers_format: Conv.BinIntFormat,
 			opc_query_after_write: bool,
-			logging_mode: LoggingMode):
+			logging_mode: LoggingMode,
+			opc_query_sync_mechanism: OpcSyncQueryMechanism):
 
 		self.viclear_exe_mode = viclear_exe_mode
 		self.idn_model_full_name = idn_model_full_name
 		self.write_delay = write_delay
 		self.read_delay = read_delay
 		self.io_segment_size = io_segment_size
 		self.opc_wait_mode = opc_wait_mode
 		self.opc_timeout = opc_timeout
 		self.visa_timeout = visa_timeout
 		self.selftest_timeout = self_test_timeout
 		self.instr_options_parse_mode = instr_options_parse_mode
 		self.bin_float_numbers_format = bin_float_numbers_format
 		self.bin_int_numbers_format = bin_int_numbers_format
 		self.opc_query_after_write = opc_query_after_write
+		self.opc_query_after_write = opc_query_after_write
+		self.opc_query_sync_mechanism = opc_query_sync_mechanism
 
 		self.logging_mode = logging_mode
 		self.logging_name = None
 		self.log_to_global_target = False
 		self.log_to_console = False
 		self.log_to_udp = False
 		self.log_udp_port = 49200
@@ -75,20 +86,25 @@
 		self.assure_write_with_tc = False
 		self.term_char = '\n'
 		self.encoding = 'charmap'
 		self.add_term_char_to_write_bin_block = False
 		self.open_timeout = 0
 		self.exclusive_lock = False
 		self.vxi_capable = True
+		self.scpi_quotes: str or None = None
 
 		self.cmd_idn = '*IDN?'
+		self.first_cmds = ''
+		self.idn_custom_parse = ''
+		self.each_cmd_prefix = ''
 		self.cmd_reset = '*RST'
 		self.skip_status_system_setting = False
 		self.skip_clear_status = False
 		self.stb_in_error_check = True
+		self.each_cmd_as_query = False
 		self.instr_status_check = False
 		self.disable_opc_query = False
 
 		self.visa_select = None
 		self._last_settings = None
 
 		# Instrument object settings
@@ -172,14 +188,15 @@
 		if value:
 			self.write_delay = Conv.str_to_int(value)
 
 		value = self._get_driversetup_item('ReadDelay')
 		if value is not None:
 			self.read_delay = Conv.str_to_int(value)
 
+		# OpcWaitMode
 		value = self._get_driversetup_item('OpcWaitMode')
 		if value:
 			value = value.upper()
 			if value == 'STBPOLLING':
 				self.opc_wait_mode = WaitForOpcMode.stb_poll
 			elif value == 'STBPOLLINGSLOW':
 				self.opc_wait_mode = WaitForOpcMode.stb_poll_slow
@@ -204,28 +221,39 @@
 		if value:
 			self.exclusive_lock = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('VxiCapable')
 		if value:
 			self.vxi_capable = Conv.str_to_bool(value)
 
+		# ScpiQuotes
+		value = self._get_driversetup_item('ScpiQuotes')
+		if value:
+			if value.lower() == 'single':
+				self.scpi_quotes = "'"
+			elif value.lower() == 'double':
+				self.scpi_quotes = '"'
+			else:
+				self.scpi_quotes = value
+
 		# Obsolete, use the AssureWriteWithTermChar
 		value = self._get_driversetup_item('AssureWriteWithLf')
 		if not value:
 			value = self._get_driversetup_item('AssureWriteWithTermChar')
 		if value:
 			self.assure_write_with_tc = Conv.str_to_bool(value)
 
 		# Obsolete, use the DataChunkSize
 		value = self._get_driversetup_item('IoSegmentSize')
 		if not value:
 			value = self._get_driversetup_item('DataChunkSize')
 		if value:
 			self.io_segment_size = Conv.str_to_int(value)
 
+		# TerminationCharacter
 		value = self._get_driversetup_item('TerminationCharacter')
 		if value:
 			val_lc = value.lower()
 			if value == '\\r' or val_lc == 'cr':
 				self.term_char = '\r'
 			elif value == '\\n' or val_lc == 'lf':
 				self.term_char = '\n'
@@ -246,38 +274,57 @@
 		if value:
 			self.opc_timeout = Conv.str_to_int(value)
 
 		value = self._get_driversetup_item('VisaTimeout')
 		if value:
 			self.visa_timeout = Conv.str_to_int(value)
 
+		# ViClearExeMode
 		value = self._get_driversetup_item('ViClearExeMode')
 		if value:
 			enum_value = Conv.str_to_simple_scalar_enum(value, InstrViClearMode, case_sensitive=False, ignore_underscores=True)
 			if enum_value is None:
 				try:
 					enum_value = InstrViClearMode(Conv.str_to_int(value))
 				except ValueError:
 					raise ValueError(
 						f"Unknown value in InitWithOptions string DriverSetup key 'ViClearExeMode'. Value '{value}' is not recognized. "
 						f"Valid values: ExecuteOnAll, Disabled, IgnoreError or integer bit-wise value.")
 			self.viclear_exe_mode = enum_value
 
+		# OpcSyncQueryMechanism
+		value = self._get_driversetup_item('OpcSyncQueryMechanism')
+		if value:
+			enum_value = Conv.str_to_simple_scalar_enum(value, OpcSyncQueryMechanism, case_sensitive=False, ignore_underscores=True)
+			if enum_value is None:
+				try:
+					enum_value = OpcSyncQueryMechanism(Conv.str_to_int(value))
+				except ValueError:
+					raise ValueError(
+						f"Unknown value in InitWithOptions string DriverSetup key 'OpcSyncQueryMechanism'. Value '{value}' is not recognized. "
+						f"Valid values: Standard, AlsoCheckMav, ClsOnlyCheckMavErrQueue, OnlyCheckMavErrQueue.")
+			self.opc_query_sync_mechanism = enum_value
+
 		value = self._get_driversetup_item('OpcQueryAfterWrite')
 		if value:
 			self.opc_query_after_write = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('StbInErrorCheck')
 		if value:
 			self.stb_in_error_check = Conv.str_to_bool(value)
 
+		value = self._get_driversetup_item('EachCmdAsQuery')
+		if value:
+			self.each_cmd_as_query = Conv.str_to_bool(value)
+
 		value = self._get_driversetup_item('DisableOpcQuery')
 		if value:
 			self.disable_opc_query = Conv.str_to_bool(value)
 
+		# LoggingMode
 		value = self._get_driversetup_item('LoggingMode')
 		if value:
 			enum_value = Conv.str_to_simple_scalar_enum(value, LoggingMode, case_sensitive=False)
 			if not enum_value:
 				raise ValueError(
 					f"Unknown value in InitWithOptions string 'options', key 'LoggingMode'. Value '{value}' is not recognized. "
 					f"Valid values: {', '.join([x.name for x in LoggingMode])}")
@@ -303,28 +350,29 @@
 		value = self._get_driversetup_item('LoggingUdpPort')
 		if value:
 			self.log_udp_port = Conv.str_to_int(value)
 
 		# Others
 		value = self._get_driversetup_item('CmdIdn')
 		if value:
-			self.cmd_idn = value
+			self.cmd_idn = '' if value.lower() == '<none>' else value
 
 		value = self._get_driversetup_item('CmdReset')
 		if value:
 			self.cmd_reset = value
 
 		value = self._get_driversetup_item('SkipStatusSystemSettings')
 		if value:
 			self.skip_status_system_setting = Conv.str_to_bool(value)
 
 		value = self._get_driversetup_item('SkipClearStatus')
 		if value:
 			self.skip_clear_status = Conv.str_to_bool(value)
 
+		# QueryOpt
 		value = self._get_driversetup_item('QueryOpt')
 		if value:
 			enum_value = Conv.str_to_simple_scalar_enum(value, Opts.ParseMode, case_sensitive=False)
 			if not enum_value:
 				raise ValueError(
 					f"Unknown value in InitWithOptions string 'options', key 'QueryOpt'. Value '{value}' is not recognized. "
 					f"Valid values: {', '.join([x.name for x in Opts.ParseMode])}")
@@ -349,15 +397,15 @@
 		if value:
 			self.supported_instr_models = [*map(trim_str_response, value.split('/'))]
 
 		value = self._get_driversetup_item('SupportedIdnPatterns')
 		if value:
 			self.supported_idn_patterns = [*map(trim_str_response, value.split('/'))]
 
-		# Profile has the ultimate priority.
+		# Profiles
 		value = self._get_driversetup_item('Profile')
 		if value:
 			val_low = value.lower()
 
 			if val_low == 'hm8123':
 				self.term_char = '\r'
 				self.assure_write_with_tc = True
@@ -373,18 +421,64 @@
 				self.term_char = '\r'
 				self.assure_write_with_tc = True
 				self.skip_status_system_setting = True
 				self.skip_clear_status = True
 				self.disable_opc_query = True
 				self.instrument_status_check = False
 				self.stb_in_error_check = False
+				self.each_cmd_as_query = True
 
 			elif val_low == 'minimal':
 				self.assure_write_with_tc = True
 				self.skip_status_system_setting = True
 				self.skip_clear_status = True
 				self.disable_opc_query = True
 				self.instrument_status_check = False
 				self.stb_in_error_check = False
 
+			elif val_low == 'ats':
+				self.term_char = '\0'
+				self.assure_write_with_tc = True
+				self.skip_status_system_setting = True
+				self.skip_clear_status = True
+				self.disable_opc_query = True
+				self.instrument_status_check = False
+				self.stb_in_error_check = False
+				self.each_cmd_as_query = True
+
+			elif val_low == 'xk41':
+				self.assure_write_with_tc = True
+				self.skip_status_system_setting = True
+				self.skip_clear_status = True
+				self.disable_opc_query = True
+				self.instrument_status_check = False
+				self.stb_in_error_check = False
+				self.each_cmd_prefix = '\n'
+				self.first_cmds = '<q>M:REMOTE SENTER1'
+				self.cmd_idn = 'M:GR GVER'
+				self.idn_custom_parse = 'gVER"([^"]+)"->Rohde&Schwarz,M3SR,100000,\\1'
+				self.term_char = '\r'
+				self.each_cmd_as_query = True
+
 			else:
-				raise ValueError(f"Unknown value in InitWithOptions string 'options', key 'Profile', value '{value}'. Valid values: HM8123, CMQ")
+				raise ValueError(f"Unknown value in InitWithOptions string 'options', key 'Profile', value '{value}'. Valid values (case-insensitive): HM8123, CMQ, Minimal, XK41, ATS")
+
+			# Following values can still be overwritten on top of the profiles
+			value = self._get_driversetup_item('FirstCmds')
+			if value:
+				self.first_cmds = value
+
+			value = self._get_driversetup_item('IdnCustomParse')
+			if value:
+				self.idn_custom_parse = value
+
+			value = self._get_driversetup_item('EachCmdPrefix')
+			if value:
+				val_lc = value.lower()
+				if value == '\\r' or val_lc == 'cr':
+					self.each_cmd_prefix = '\r'
+				elif value == '\\n' or val_lc == 'lf':
+					self.each_cmd_prefix = '\n'
+				elif value == '\\t' or val_lc == 'tab':
+					self.each_cmd_prefix = '\t'
+				else:
+					self.each_cmd_prefix = value
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/InternalLinker.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/InternalLinker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/RepeatedCapability.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/RepeatedCapability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ScpiEnums.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ScpiEnums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/ScpiLogger.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/ScpiLogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
 
     def __init__(self, resource_name: str, encoding: str = 'charmap'):
         if resource_name is None:
             raise RsInstrException('resource_name cannot be None')
         self._orig_resource_name = resource_name
         self._global_mode: bool = False
         self._default_mode: LoggingMode = LoggingMode.Off
+        self._last_logging_mode: LoggingMode = LoggingMode.On
         self._mode: LoggingMode = self._default_mode
         self._log_target_local = None
         self._cached = CachedEntries()
         self._timestamp_reference_time_local: datetime or None = None
         self._format_string: str = ''
         self._line_divider: str = '\n'
         self._target_auto_flushing = True
@@ -336,33 +337,55 @@
     def target_auto_flushing(self, value: bool) -> None:
         """Sets auto-flushing for the logging target. If set to True (default value), after each entry the stream is flushed,
         This makes sure, that even if your e.g. file stream is not closed at the end, it contains all the entries."""
         self._target_auto_flushing = value
 
     @property
     def mode(self) -> LoggingMode:
-        """Sets / returns the Logging mode.
+        """Sets the logging ON or OFF. Additionally, you can set the logging ON only for errors.
+        Possible values:
 
-        :Data Type: LoggingMode"""
+        * LoggingMode.Off  - logging is switched OFF
+        * LoggingMode.On  - logging is switched ON
+        * LoggingMode.Errors  - logging is switched ON, but only for error entries
+        * LoggingMode.Default  - sets the logging to default - the value you have set with logger.default_mode
+
+        """
         return self._mode
 
+    Off = 0  # Don't write messages to log
+    On = 1  # Write message to log
+    Errors = 2  # Only log errors. This is like 'Off', with the exception, that VisaIOErrors are logged.
+    Default = 3  # Default mode
+
     @mode.setter
     def mode(self, value: LoggingMode) -> None:
         """Sets / returns the Logging mode."""
         if self._segment:
             raise RsInstrException(f"Can not change the logging mode when a log segment is active. End the segment with ScpiLogger.end_current_segment(). Device name: '{self.device_name}'")
         value = self._resolve_log_mode(value)
         if self.mode != LoggingMode.Off:
             # logging is ON. Check the internal log entries and flush them to the target
             self._flush_cached_entries()
         self._mode = value
         if self._mode == LoggingMode.Off and self.get_logging_target():
             # Logging was switched off, flush the entries on the target
             self.flush()
 
+    def start(self) -> None:
+        """Starts the logging with the last defined LoggingMode. Default is LoggingMode.On"""
+        self.mode = self._last_logging_mode
+
+    def stop(self) -> None:
+        """Stops the logging. This is the same as: mode = LoggingMode.Off"""
+        if self.mode is not LoggingMode.Off:
+            self._last_logging_mode = self.mode
+
+        self.mode = LoggingMode.Off
+
     @property
     def log_status_check_ok(self) -> bool:
         """Sets / returns the current status of status checking OK.
         If True (default), the log contains logging of the status checking 'Status check: OK'.
         If False, the 'Status check: OK' is skipped - the log is more compact.
         Errors will still be logged."""
         return self._log_status_check_ok
@@ -458,15 +481,15 @@
             return self._default_mode
         else:
             return value
 
     @property
     def default_mode(self) -> LoggingMode:
         """Sets / returns the default logging mode.
-        You can recall the default mode by calling the logger.mode = LoggingMode.Default
+        You can recall the default mode by calling the logger.mode = LoggingMode.Default.
 
         :Data Type: LoggingMode
         """
         return self._default_mode
 
     @default_mode.setter
     def default_mode(self, value: LoggingMode) -> None:
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamReader.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/StreamReader.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StreamWriter.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/StreamWriter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/StructBase.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/StructBase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Types.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Types.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/Utilities.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/Utilities.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/VisaPluginSocketIo.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,16 @@
 
 		try:
 			while True:
 				to_read_len = chunk_size - read_len
 				if to_read_len <= 0:
 					break
 				data = session.recv(to_read_len)
+				if not data:
+					raise pyvisa.VisaIOError(pyvisa.constants.VI_ERROR_CONN_LOST)
 				chunk += data
 				read_len += len(data)
 
 				if self._socket_io.read_termination is not None:
 					# Read termination character is ON, look for it and stop the reading if found
 					term_char = self._socket_io.read_termination.encode()
 					if term_char in data:
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSession.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/VisaSession.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from typing import List, Tuple, Callable, AnyStr
 import os.path
 import re
 import threading
 
 # noinspection PyPackageRequirements
 import pyvisa
+from pyvisa.errors import StatusCode
 
 from .VisaPluginSocketIo import ResourceManager, SocketIo
 from . import InstrumentSettings, InstrumentErrors, Conversions as Conv
-from .InstrumentSettings import WaitForOpcMode, InstrViClearMode as ViClearMode
+from .InstrumentSettings import WaitForOpcMode, OpcSyncQueryMechanism, InstrViClearMode as ViClearMode
 from .StreamReader import StreamReader
 from .StreamWriter import StreamWriter
 from .Utilities import size_to_kb_mb_string, calculate_chunks_count
 import platform
 import struct
 
 
@@ -39,14 +40,16 @@
 	bin_known_len = 3
 	bin_unknown_len = 4
 
 
 class StatusByte(Flag):
 	"""Status Byte flags."""
 	NONE = 0x00
+	custom_bit_0 = 0x01
+	custom_bit_1 = 0x02
 	error_queue_not_empty = 0x04
 	questionable_status_reg = 0x08
 	message_available = 0x10
 	event_status_byte = 0x20
 	request_service = 0x40
 	operation_status_reg = 0x80
 
@@ -72,14 +75,16 @@
 		self.visa_library_name = None
 		self.resource_name = resource_name  # might be changed later if direct_session is used
 		self.encoding = settings.encoding  # default encoder between bytes and string
 		self.cmd_idn = settings.cmd_idn
 		self.skip_status_system_setting = settings.skip_status_system_setting
 		self.skip_clear_status = settings.skip_clear_status
 		self.stb_in_error_check = settings.stb_in_error_check
+		self.opc_sync_query_mechanism = settings.opc_query_sync_mechanism
+		self.each_cmd_prefix = settings.each_cmd_prefix
 
 		# Implemented for interface compatibility with VisaSessionSim
 		self.cached_to_stream = False
 
 		# Event handlers
 		# noinspection PyTypeChecker
 		self.on_read_chunk_handler: Callable = None
@@ -187,14 +192,27 @@
 		# Must call the VISA viClear() before any communication with the instrument
 		self.clear()
 
 		# Further steps are for NRP-Z session not valid
 		if self.is_rsnrp_session():
 			return
 
+		# First commands, can be more than one, separated by ';;'
+		if settings.first_cmds:
+			cmds = settings.first_cmds.split(';;')
+			for cmd in cmds:
+				if cmd.startswith('<w>'):
+					self.write(cmd[3:])
+				elif cmd.startswith('<q>'):
+					_ = self._query_str_no_events(cmd[3:])
+				elif '?' in cmd:
+					_ = self._query_str_no_events(cmd)
+				else:
+					self.write(cmd)
+
 		# Clear instrument status
 		if self.skip_clear_status is False:
 			self.write('*CLS')
 			if self.vxi_capable:
 				stb = self._read_stb()
 				if stb & StatusByte.message_available:
 					self._flush_junk_data()
@@ -292,14 +310,26 @@
 		setattr(self._session, 'session_thread_rlock', lock)
 		self._lock = lock
 
 	def get_lock(self) -> threading.RLock:
 		"""Returns the current RLock object."""
 		return self._lock
 
+	def lock_resource(self, timeout: int, requested_key: str or bytes = None) -> bytes or None:
+		"""Locks the instrument to prevent it from communicating with other clients."""
+		if requested_key is None:
+			self._session.lock_excl(timeout)
+			return None
+		else:
+			return self._session.lock(timeout, requested_key)
+
+	def unlock_resource(self) -> None:
+		"""Unlocks the instrument to other clients."""
+		self._session.unlock()
+
 	@property
 	def visa_timeout(self) -> int:
 		"""See the visa_timeout.setter."""
 		return int(self._session.timeout)
 
 	@visa_timeout.setter
 	def visa_timeout(self, value: int) -> None:
@@ -314,15 +344,15 @@
 	@data_chunk_size.setter
 	def data_chunk_size(self, chunk_size: int) -> None:
 		"""Sets the maximum size of one block transferred during write/read operations."""
 		self._data_chunk_size = int(chunk_size)
 		self._session.chunk_size = int(chunk_size)
 
 	def _resolve_opc_timeout(self, timeout: int) -> int:
-		"""Resolves entered timeout value - if the input value is less than 1, it is replaces with opc_timeout."""
+		"""Resolves entered timeout value - if the input value is less than 1, it is replaced with opc_timeout."""
 		if timeout is None or timeout < 1:
 			return self.opc_timeout
 		else:
 			return timeout
 
 	def _set_regs_ese_sre(self, mode: WaitForOpcMode) -> WaitForOpcMode:
 		"""Based on the WaitForOpcMode, it sets the ESE and SRE register masks.
@@ -350,41 +380,60 @@
 			current_value = int(self._query_str_no_events('*SRE?'))
 			mask = current_value | mask.value
 		# Also affect the _opc_wait_mode:
 		# If the mask has event_status_byte == false, and the _opc_wait_mode is service_request, set it to stb_poll
 		# If the mask has event_status_byte == true, do not change anything
 		self.write(f'*SRE {mask.value}')
 
-	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int, end_mask: StatusByte) -> StatusByte:
+	def _write_and_poll_stb_vxi(self, command: str, is_query: bool, timeout: int) -> StatusByte:
 		"""Reads Status Byte Register and ends if the ESB bit (5) is set to 1.
 		Also works with the SOCKET and SERIAL interface by sending *STB? query.
 		In that case however, command cannot be a query.
 		Returns the last read Status Byte value."""
 		timeout_secs = timeout / 1000
-		self.clear_before_read()
+		end_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
 		if command.endswith(self._term_char):
 			command = command.rstrip(self._term_char)
-		self.write(command + ';*OPC')
-		# Use catch to return the VISA Timeout back
+
+		if is_query is True:
+			if self.opc_sync_query_mechanism == OpcSyncQueryMechanism.standard or self.opc_sync_query_mechanism == OpcSyncQueryMechanism.also_check_mav:
+				self.clear_before_read()
+				self.write(command + ';*OPC')
+				if self.opc_sync_query_mechanism == OpcSyncQueryMechanism.also_check_mav:
+					end_mask |= StatusByte.message_available
+
+			elif self.opc_sync_query_mechanism == OpcSyncQueryMechanism.only_check_mav_err_queue:
+				self.write(command)
+				end_mask = StatusByte.error_queue_not_empty | StatusByte.message_available
+
+			elif self.opc_sync_query_mechanism == OpcSyncQueryMechanism.cls_only_check_mav_err_queue:
+				self.clear_before_read()
+				self.write(command)
+				end_mask = StatusByte.error_queue_not_empty | StatusByte.message_available
+		else:
+			self.clear_before_read()
+			self.write(command + ';*OPC')
+
 		start = time.time()
 		# STB polling loop
 		while True:
 			stb = self._read_stb()
 			elapsed = self._polling_delay(start)
 			if elapsed > timeout_secs:
 				self._narrow_down_opc_tout_error(command, is_query, timeout)
 			if end_mask & stb:
 				break
 		return stb
 
-	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int, end_mask: StatusByte) -> StatusByte:
+	def _write_and_poll_stb_non_vxi(self, command: str, timeout: int) -> StatusByte:
 		"""Queries Status Byte Register (*STB?) and ends if the ESB bit (5) is set to 1.
 			The command must not be a query. Also works with the SOCKET and SERIAL interface.
 			Returns the last read Status Byte value."""
 		timeout_secs = timeout / 1000
+		end_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
 		self.clear_before_read()
 		if command.endswith(self._term_char):
 			command = command.rstrip(self._term_char)
 		self.write(command + ';*OPC')
 		start = time.time()
 		# STB polling loop
 		while True:
@@ -644,16 +693,17 @@
 		- sending the *IDN? query"""
 		if self._session is None:
 			return False
 		# noinspection PyBroadException
 		try:
 			old_tout = self.visa_timeout
 			self.visa_timeout = 2000
-			self.write(self.cmd_idn)
-			_ = self._read_str_no_events()
+			if len(self.cmd_idn) > 0:
+				self.write(self.cmd_idn)
+				_ = self._read_str_no_events()
 			self.visa_timeout = old_tout
 			return True
 		except Exception:
 			return False
 
 	def _write_and_wait_for_opc(self, command: str, is_query: bool, timeout: int) -> StatusByte:
 		"""Internal method to synchronise a command with OPC timeout.
@@ -669,21 +719,18 @@
 
 		if self._opc_wait_mode == WaitForOpcMode.opc_query:
 			if is_query:
 				raise RsInstrException('Sending a query with OpcQuery synchronization is not possible')
 			stb = self._write_and_query_opc(command, timeout)
 		else:
 			# STB polling
-			end_stb_mask = StatusByte.error_queue_not_empty | StatusByte.event_status_byte
-			if is_query:
-				end_stb_mask |= StatusByte.message_available
 			if self.vxi_capable:
-				stb = self._write_and_poll_stb_vxi(command, is_query, timeout, end_stb_mask)
+				stb = self._write_and_poll_stb_vxi(command, is_query, timeout)
 			else:
-				stb = self._write_and_poll_stb_non_vxi(command, timeout, end_stb_mask)
+				stb = self._write_and_poll_stb_non_vxi(command, timeout)
 
 		return stb
 
 	def _write_and_query_opc(self, cmd: str, timeout: int) -> StatusByte:
 		"""Internal method to write a command followed by query_opc().
 		Used for opc-synchronization if the mode is set to WaitForOpcMode.opc_query or the session is not-vxi.
 		Timeout value 0 means the OPC timeout is used."""
@@ -697,36 +744,48 @@
 			self.write(cmd)
 			self.query_opc()
 		finally:
 			if old_tout != timeout:
 				self.visa_timeout = old_tout
 		return self._query_stb()
 
+	def clear_status_after_query_with_opc(self) -> bool:
+		"""Returns true, if the opc-sync queries require status clearing afterward."""
+		if self.vxi_capable is False or self._opc_wait_mode is WaitForOpcMode.opc_query:
+			return False
+		if self.opc_sync_query_mechanism == InstrumentSettings.OpcSyncQueryMechanism.standard:
+			return True
+		if self.opc_sync_query_mechanism == InstrumentSettings.OpcSyncQueryMechanism.also_check_mav:
+			return True
+		return False
+
 	def write(self, cmd: str) -> None:
 		"""Writes command to the instrument."""
 		if self.write_delay > 0:
 			time.sleep(self.write_delay / 1000)
 		add_tc = False
 		if self._assure_write_with_tc and not cmd.endswith(self._term_char):
 			add_tc = True
+		if self.each_cmd_prefix:
+			cmd = self.each_cmd_prefix + cmd
 		cmd_bytes = cmd.encode(self.encoding)
 		if add_tc:
 			cmd_bytes += self._term_char.encode(self.encoding)
 		self._session.write_raw(cmd_bytes)
 
 	def _read_unknown_len(self, stream: StreamWriter, allow_chunk_events: bool, prepend_data: AnyStr = None) -> None:
 		"""Reads data of unknown length to the provided WriteStream.
 		The read is performed in an incremental chunk steps to optimize memory use (for NRP-Z session it is set to fixed self._data_chunk_size):
 			- The first read is performed with the fixed size of 1024 bytes
 			- The 2nd one reads 64 kBytes
 			- The 3rd one reads 128 kBytes
 			- The 4th one reads 256 kBytes and so on, with the max cap of self._data_chunk_size
 		:param stream: [StreamWriter] target for the read data
 		:param allow_chunk_events: [bool] if True, the method can send the chunk_events. If False, sending events is blocked.
-		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first chunk read
+		:param prepend_data: Optional[bytes or string] You can prepend this data to the beginning. It will be considered part of the first read chunk
 		:return: read data [bytes or string], depending on the parameter binary."""
 		with self._session.ignore_warning(pyvisa.constants.StatusCode.success_max_count_read):
 			if prepend_data and isinstance(prepend_data, str):
 				prepend_data = prepend_data.encode(self.encoding)
 			chunk_ix = 0
 			eot = False
 			while not eot:
@@ -774,20 +833,23 @@
 		"""Queries the instrument and reads the response as string.
 		The length of the string is not limited. The response is then trimmed for trailing LF.
 		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
 		response = ''
 		self.write(query)
 		try:
 			response = self._read_str_no_events()
-		except pyvisa.VisaIOError:
+		except pyvisa.VisaIOError as e:
 			context = f"Query '{query.rstrip(self._term_char)}'"
-			if allow_tout_error_narrow_down:
-				self._narrow_down_io_tout_error(context + ' - ')
+			if e.error_code == StatusCode.error_timeout:
+				if allow_tout_error_narrow_down:
+					self._narrow_down_io_tout_error(context + ' - ')
+				else:
+					raise InstrumentErrors.TimeoutException(context)
 			else:
-				raise InstrumentErrors.TimeoutException(context)
+				raise InstrumentErrors.RsInstrException(context)
 		return response
 
 	def _query_str_no_events_timed(self, query: str, timeout: int, suppress_read_tout: bool = False) -> str:
 		"""Queries the instrument and reads the response as string.
 		The entered timeout sets the VISA timeout just for this call. You can suppress the timeout error.
 		The length of the string is not limited. The response is then trimmed for trailing LF.
 		Sending of any read events is blocked. Use this method for all the service VisaSession queries."""
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/Internal/VisaSessionSim.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/Internal/VisaSessionSim.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,18 @@
 		"""Clears IO buffers and the ESR register before reading/writing responses synchronized with *OPC."""
 		return
 
 	def clear(self) -> None:
 		"""Perform VISA viClear conditionally based on the instrument settings."""
 		return
 
+	def clear_status_after_query_with_opc(self) -> bool:
+		"""Returns true, if the opc-sync queries require status clearing afterward."""
+		return False
+
 	def write(self, cmd: str) -> None:
 		"""Writes command to the instrument."""
 		self._last_cmd = cmd
 		self._update_cmd_vals_cache(cmd)
 		return
 
 	def query_str(self, query: str) -> str:
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/RsCMPX_UwbMeas.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/RsCMPX_UwbMeas.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from datetime import datetime, timedelta
 from . import repcap
 from .Internal.RepeatedCapability import RepeatedCapability
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class RsCMPX_UwbMeas:
-	"""520 total commands, 5 Subgroups, 0 group commands"""
-	_driver_options = "SupportedInstrModels = CMP/CMX/CMW, SupportedIdnPatterns = CMP/CMX/CMW, SimulationIdnString = 'Rohde&Schwarz,CMP,100001,4.0.80.0016'"
+	"""554 total commands, 5 Subgroups, 0 group commands"""
+	_driver_options = "SupportedInstrModels = CMP/CMX, SupportedIdnPatterns = CMP/CMX, SimulationIdnString = 'Rohde&Schwarz,CMP200,100001,5.0.20.0022'"
 	_global_logging_relative_timestamp: ClassVar[datetime] = None
 	_global_logging_target_stream: ClassVar = None
 
 	def __init__(self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsCMPX_UwbMeas session. \n
 		Parameter options tokens examples:
 			- ``Simulate=True`` - starts the session in simulation mode. Default: ``False``
@@ -31,27 +31,28 @@
 			- ``TerminationCharacter = "\\r"`` - Sets the termination character for reading. Default: ``\\n`` (LineFeed or LF)
 			- ``DataChunkSize = 10E3`` - Maximum size of one write/read segment. If transferred data is bigger, it is split to more segments. Default: ``1E6`` bytes
 			- ``OpcTimeout = 10000`` - same as driver.utilities.opc_timeout = 10000. Default: ``30000ms``
 			- ``VisaTimeout = 5000`` - same as driver.utilities.visa_timeout = 5000. Default: ``10000ms``
 			- ``ViClearExeMode = Disabled`` - viClear() execution mode. Default: ``execute_on_all``
 			- ``OpcQueryAfterWrite = True`` - same as driver.utilities.opc_query_after_write = True. Default: ``False``
 			- ``StbInErrorCheck = False`` - if true, the driver checks errors with *STB? If false, it uses SYST:ERR?. Default: ``True``
+			- ``ScpiQuotes = double'. - for SCPI commands, you can define how strings are quoted. With single or double quotes. Possible values: single | double | {char}. Default: ``single``
 			- ``LoggingMode = On`` - Sets the logging status right from the start. Default: ``Off``
 			- ``LoggingName = 'MyDevice'`` - Sets the name to represent the session in the log entries. Default: ``'resource_name'``
 			- ``LogToGlobalTarget = True`` - Sets the logging target to the class-property previously set with RsCMPX_UwbMeas.set_global_logging_target() Default: ``False``
 			- ``LoggingToConsole = True`` - Immediately starts logging to the console. Default: False
 			- ``LoggingToUdp = True`` - Immediately starts logging to the UDP port. Default: False
 			- ``LoggingUdpPort = 49200`` - UDP port to log to. Default: 49200
 		:param resource_name: VISA resource name, e.g. 'TCPIP::192.168.2.1::INSTR'
 		:param id_query: if True, the instrument's model name is verified against the models supported by the driver and eventually throws an exception.
 		:param reset: Resets the instrument (sends *RST command) and clears its status sybsystem.
 		:param options: string tokens alternating the driver settings.
 		:param direct_session: Another driver object or pyVisa object to reuse the session instead of opening a new session."""
 		self._core = Core(resource_name, id_query, reset, RsCMPX_UwbMeas._driver_options, options, direct_session)
-		self._core.driver_version = '4.0.80.0016'
+		self._core.driver_version = '5.0.20.0022'
 		self._options = options
 		self._add_all_global_repcaps()
 		self._custom_properties_init()
 		self.utilities.default_instrument_setup()
 		# noinspection PyTypeChecker
 		self._cmd_group = CommandsGroup("ROOT", self._core, None)
 
@@ -123,25 +124,25 @@
 		self._core.io.reset_time_statistics()
 
 	@staticmethod
 	def assert_minimum_version(min_version: str) -> None:
 		"""Asserts that the driver version fulfills the minimum required version you have entered.
 		This way you make sure your installed driver is of the entered version or newer."""
 		min_version_list = min_version.split('.')
-		curr_version_list = '4.0.80.0016'.split('.')
+		curr_version_list = '5.0.20.0022'.split('.')
 		count_min = len(min_version_list)
 		count_curr = len(curr_version_list)
 		count = count_min if count_min < count_curr else count_curr
 		for i in range(count):
 			minimum = int(min_version_list[i])
 			curr = int(curr_version_list[i])
 			if curr > minimum:
 				break
 			if curr < minimum:
-				raise RsInstrException(f"Assertion for minimum RsCMPX_UwbMeas version failed. Current version: '4.0.80.0016', minimum required version: '{min_version}'")
+				raise RsInstrException(f"Assertion for minimum RsCMPX_UwbMeas version failed. Current version: '5.0.20.0022', minimum required version: '{min_version}'")
 
 	@staticmethod
 	def list_resources(expression: str = '?*::INSTR', visa_select: str = None) -> List[str]:
 		"""Finds all the resources defined by the expression
 			- '?*' - matches all the available instruments
 			- 'USB::?*' - matches all the USB instruments
 			- 'TCPIP::192?*' - matches all the LAN instruments with the IP address starting with 192
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/__init__.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """RsCMPX_UwbMeas instrument driver
-	:version: 4.0.80.16
-	:copyright: 2021 by Rohde & Schwarz GMBH & Co. KG
+	:version: 5.0.20.22
+	:copyright: 2023 by Rohde & Schwarz GMBH & Co. KG
 	:license: MIT, see LICENSE for more details.
 """
 
-__version__ = '4.0.80.16'
+__version__ = '5.0.20.22'
 
 # Main class
 from RsCMPX_UwbMeas.RsCMPX_UwbMeas import RsCMPX_UwbMeas
 
 # Bin data format
 from RsCMPX_UwbMeas.Internal.Conversions import BinIntFormat, BinFloatFormat
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/enums.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,21 +174,23 @@
 	"""2 Members, MS1 ... PPDU"""
 	MS1 = 0
 	PPDU = 1
 
 
 # noinspection SpellCheckingInspection
 class PhrDataRate(Enum):
-	"""6 Members, DRHP ... SYNC"""
+	"""8 Members, DRHP ... SYNC"""
 	DRHP = 0
 	DRLP = 1
 	DRMD = 2
-	RHMH = 3
-	RHML = 4
-	SYNC = 5
+	IGN = 3
+	RHMH = 4
+	RHML = 5
+	RSF = 6
+	SYNC = 7
 
 
 # noinspection SpellCheckingInspection
 class PpduMode(Enum):
 	"""2 Members, MPPDu ... SPPDu"""
 	MPPDu = 0
 	SPPDu = 1
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas/repcap.py` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas/repcap.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 	Default = DefaultRepCap
 	Nr1 = 1
 	Nr2 = 2
 	Nr3 = 3
 
 
 # noinspection SpellCheckingInspection
-class Pddu(Enum):
-	"""Repeated capability Pddu"""
+class Ppdu(Enum):
+	"""Repeated capability Ppdu"""
 	Empty = EmptyRepCap
 	Default = DefaultRepCap
 	Nr1 = 1
 	Nr2 = 2
 	Nr3 = 3
 	Nr4 = 4
 	Nr5 = 5
@@ -142,16 +142,16 @@
 	Nr97 = 97
 	Nr98 = 98
 	Nr99 = 99
 	Nr100 = 100
 
 
 # noinspection SpellCheckingInspection
-class Ppdu(Enum):
-	"""Repeated capability Ppdu"""
+class Record(Enum):
+	"""Repeated capability Record"""
 	Empty = EmptyRepCap
 	Default = DefaultRepCap
 	Nr1 = 1
 	Nr2 = 2
 	Nr3 = 3
 	Nr4 = 4
 	Nr5 = 5
@@ -166,87 +166,7 @@
 	Nr14 = 14
 	Nr15 = 15
 	Nr16 = 16
 	Nr17 = 17
 	Nr18 = 18
 	Nr19 = 19
 	Nr20 = 20
-	Nr21 = 21
-	Nr22 = 22
-	Nr23 = 23
-	Nr24 = 24
-	Nr25 = 25
-	Nr26 = 26
-	Nr27 = 27
-	Nr28 = 28
-	Nr29 = 29
-	Nr30 = 30
-	Nr31 = 31
-	Nr32 = 32
-	Nr33 = 33
-	Nr34 = 34
-	Nr35 = 35
-	Nr36 = 36
-	Nr37 = 37
-	Nr38 = 38
-	Nr39 = 39
-	Nr40 = 40
-	Nr41 = 41
-	Nr42 = 42
-	Nr43 = 43
-	Nr44 = 44
-	Nr45 = 45
-	Nr46 = 46
-	Nr47 = 47
-	Nr48 = 48
-	Nr49 = 49
-	Nr50 = 50
-	Nr51 = 51
-	Nr52 = 52
-	Nr53 = 53
-	Nr54 = 54
-	Nr55 = 55
-	Nr56 = 56
-	Nr57 = 57
-	Nr58 = 58
-	Nr59 = 59
-	Nr60 = 60
-	Nr61 = 61
-	Nr62 = 62
-	Nr63 = 63
-	Nr64 = 64
-	Nr65 = 65
-	Nr66 = 66
-	Nr67 = 67
-	Nr68 = 68
-	Nr69 = 69
-	Nr70 = 70
-	Nr71 = 71
-	Nr72 = 72
-	Nr73 = 73
-	Nr74 = 74
-	Nr75 = 75
-	Nr76 = 76
-	Nr77 = 77
-	Nr78 = 78
-	Nr79 = 79
-	Nr80 = 80
-	Nr81 = 81
-	Nr82 = 82
-	Nr83 = 83
-	Nr84 = 84
-	Nr85 = 85
-	Nr86 = 86
-	Nr87 = 87
-	Nr88 = 88
-	Nr89 = 89
-	Nr90 = 90
-	Nr91 = 91
-	Nr92 = 92
-	Nr93 = 93
-	Nr94 = 94
-	Nr95 = 95
-	Nr96 = 96
-	Nr97 = 97
-	Nr98 = 98
-	Nr99 = 99
-	Nr100 = 100
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/PKG-INFO` & `RsCMPX_UwbMeas-5.0.20/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: RsCMPX-UwbMeas
-Version: 4.0.80
-Summary: CMP/CMX Ultra Wideband Measurement Remote-control module
+Name: RsCMPX_UwbMeas
+Version: 5.0.20
+Summary: CMP200 Ultra Wideband Measurement Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_UwbMeas
         ==================================
         
@@ -20,43 +20,50 @@
         
         .. image:: https://img.shields.io/pypi/pyversions/pybadges.svg
            :target: https://img.shields.io/pypi/pyversions/pybadges.svg
         
         .. image:: https://img.shields.io/pypi/dm/RsCMPX_UwbMeas.svg
            :target: https://pypi.python.org/pypi/RsCMPX_UwbMeas/
         
-        Rohde & Schwarz CMP/CMX Ultra Wideband Measurement RsCMPX_UwbMeas instrument driver.
+        Rohde & Schwarz CMP200 Ultra Wideband Measurement RsCMPX_UwbMeas instrument driver.
         
         Basic Hello-World code:
         
         .. code-block:: python
         
             from RsCMPX_UwbMeas import *
         
-            instr = RsCMPX_UwbMeas('TCPIP::192.168.56.101::5025::SOCKET', reset=True)
+            instr = RsCMPX_UwbMeas('TCPIP::192.168.2.101::hislip0')
             idn = instr.query('*IDN?')
             print('Hello, I am: ' + idn)
         
-        Check out the full documentation on `ReadTheDocs <https://RsCMPX_UwbMeas.readthedocs.io/>`_.
+        Supported instruments: CMP200
         
-        Supported instruments: CMX500, CMP200
+        The package is hosted here: https://pypi.org/project/RsCMPX-UwbMeas/
         
-        The package is hosted here: https://pypi.org/project/RsCMPX_UwbMeas/
-        
-        Documentation: https://RsCMPX_UwbMeas.readthedocs.io/
+        Documentation: https://RsCMPX-UwbMeas.readthedocs.io/
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
-        Version history:
+        Version history
         ----------------
         
-        	Latest release notes summary: Update of RsCMPX_UwbMeas to FW 4.0.80 from the complete FW package 7.10.0
+        	Latest release notes summary: Update for FW 5.0.20
+        
+        	Version 5.0.20
+        		- Update for FW 5.0.20
+        
+        	Version 4.0.171
+        		- Fixed documentation
+        
+        	Version 4.0.170
+        		- Update for FW 4.0.170
         
-        	Version 4.0.80.16
+        	Version 4.0.80
         		- Update of RsCMPX_UwbMeas to FW 4.0.80 from the complete FW package 7.10.0
         
         	Version 4.0.70
         		- Update of RsCMPX_UwbMeas to FW 4.0.70
         		
         	Version 4.0.12
         		- Update of RsCMPX_UwbMeas to FW 4.0.12
@@ -73,9 +80,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
```

### Comparing `RsCMPX_UwbMeas-4.0.80/RsCMPX_UwbMeas.egg-info/SOURCES.txt` & `RsCMPX_UwbMeas-5.0.20/RsCMPX_UwbMeas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,24 @@
 RsCMPX_UwbMeas/CustomFiles/reliability.py
 RsCMPX_UwbMeas/CustomFiles/utilities.py
 RsCMPX_UwbMeas/Implementations/__init__.py
 RsCMPX_UwbMeas/Implementations/Catalog/UwbMeas.py
 RsCMPX_UwbMeas/Implementations/Catalog/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/__init__.py
-RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/MprFrequency.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PhrRate.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PpLength.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Ppdu.py
-RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PrfMode.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/PsFormat.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Result.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Spectrum.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StSegments.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StsLength.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/CcError.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Foffset.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Plevel.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/PmlWidth.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/SlPeak.py
@@ -36,23 +41,30 @@
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Phr/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/Nrmse.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Psdu/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/Nrmse.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Shr/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/Nrmse.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Modulation/Limit/Sts/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr/Bitrate.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Phr/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Area.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/Area.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Lower/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/Area.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Pmask/Limit/Upper/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu/Bitrate.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/Psdu/__init__.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StsGap/Chip.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/StsGap/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/Area.py
+RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/TdbBandwidth.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/MultiEval/TsMask/Limit/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/__init__.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/Range.py
 RsCMPX_UwbMeas/Implementations/Configure/UwbMeas/RfSettings/Frequency/__init__.py
 RsCMPX_UwbMeas/Implementations/Route/__init__.py
 RsCMPX_UwbMeas/Implementations/Route/UwbMeas/RfSettings.py
 RsCMPX_UwbMeas/Implementations/Route/UwbMeas/__init__.py
@@ -252,14 +264,26 @@
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/MsfPower/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Average.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Current.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Maximum.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/Minimum.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/StandardDev.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpPower/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/PpdPeak/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Average.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Current.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Maximum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/Minimum.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/StandardDev.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppdu/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Average.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Current.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Maximum.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/Minimum.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/StandardDev.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Power/Ppower/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/AsSymbols.py
@@ -280,14 +304,17 @@
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/Crc.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Phr/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Crc.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/Length.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Sinfo/Psdu/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/All.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/State/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/StsSequence/Clength.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/StsSequence/Content.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/StsSequence/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Average.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Current.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/Xvalues.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CpJitter/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Average.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/Trace/CtJitter/Current.py
@@ -332,14 +359,18 @@
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Average.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/Current.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Negativ/__init__.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Average.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/Current.py
 RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/Margin/Area/Positiv/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/PsPower.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/__init__.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/Frequency/Fhfl.py
+RsCMPX_UwbMeas/Implementations/UwbMeas/MultiEval/TsMask/TdbBandwidth/Frequency/__init__.py
 RsCMPX_UwbMeas/Internal/ArgLinkedEventArgs.py
 RsCMPX_UwbMeas/Internal/ArgSingle.py
 RsCMPX_UwbMeas/Internal/ArgSingleList.py
 RsCMPX_UwbMeas/Internal/ArgSingleSuppressed.py
 RsCMPX_UwbMeas/Internal/ArgStringComposer.py
 RsCMPX_UwbMeas/Internal/ArgStruct.py
 RsCMPX_UwbMeas/Internal/ArgStructList.py
@@ -352,14 +383,15 @@
 RsCMPX_UwbMeas/Internal/GlobalData.py
 RsCMPX_UwbMeas/Internal/Instrument.py
 RsCMPX_UwbMeas/Internal/InstrumentErrors.py
 RsCMPX_UwbMeas/Internal/InstrumentOptions.py
 RsCMPX_UwbMeas/Internal/InstrumentSettings.py
 RsCMPX_UwbMeas/Internal/InternalLinker.py
 RsCMPX_UwbMeas/Internal/IoTransferEventArgs.py
+RsCMPX_UwbMeas/Internal/Properties.py
 RsCMPX_UwbMeas/Internal/RepeatedCapability.py
 RsCMPX_UwbMeas/Internal/ScpiEnums.py
 RsCMPX_UwbMeas/Internal/ScpiLogger.py
 RsCMPX_UwbMeas/Internal/StreamReader.py
 RsCMPX_UwbMeas/Internal/StreamWriter.py
 RsCMPX_UwbMeas/Internal/StructBase.py
 RsCMPX_UwbMeas/Internal/Types.py
```

### Comparing `RsCMPX_UwbMeas-4.0.80/setup.py` & `RsCMPX_UwbMeas-5.0.20/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 # The text of the README file
 README = (HERE / "README.rst").read_text()
 
 # This call to setup() does all the work
 setup(
     name="RsCMPX_UwbMeas",
-    version="4.0.80",
-    description="CMP/CMX Ultra Wideband Measurement Remote-control module",
+    version="5.0.20",
+    description="CMP200 Ultra Wideband Measurement Remote-control module",
     long_description=README,
     long_description_content_type="text/x-rst",
     author="Rohde & Schwarz GmbH & Co. KG",
     copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2022",
     license="MIT",
     classifiers=['License :: OSI Approved :: MIT License',
                  'Intended Audience :: Developers',
@@ -24,13 +24,14 @@
                  'Operating System :: MacOS :: MacOS X',
                  'Programming Language :: Python',
                  'Programming Language :: Python :: 3',
                  'Programming Language :: Python :: 3.6',
                  'Programming Language :: Python :: 3.7',
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
-                 'Programming Language :: Python :: 3.10'
+                 'Programming Language :: Python :: 3.10',
+                 'Programming Language :: Python :: 3.11'
                 ],
     packages=(find_packages(include=['RsCMPX_UwbMeas', 'RsCMPX_UwbMeas.*'])),
     install_requires=['PyVisa>=1.11.3'],
     python_requires='>=3.6'
 )
```

