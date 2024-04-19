# Comparing `tmp/RsCMPX_WcdmaMeas-4.0.186.tar.gz` & `tmp/RsCMPX_WcdmaMeas-5.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_WcdmaMeas-4.0.186.tar", last modified: Mon Sep  4 10:02:14 2023, max compression
+gzip compressed data, was "dist\RsCMPX_WcdmaMeas-5.0.40.tar", last modified: Fri Apr 19 09:04:19 2024, max compression
```

## Comparing `RsCMPX_WcdmaMeas-4.0.186.tar` & `RsCMPX_WcdmaMeas-5.0.40.tar`

### file list

```diff
@@ -1,955 +1,956 @@
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.709409 RsCMPX_WcdmaMeas-4.0.186/
--rw-rw-rw-   0        0        0     2791 2023-09-04 10:02:14.707457 RsCMPX_WcdmaMeas-4.0.186/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/README.rst
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.696870 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.722247 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/
--rw-rw-rw-   0        0        0       90 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3725 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4916 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    21869 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.725174 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.727126 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.732983 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.737862 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/
--rw-rw-rw-   0        0        0     2243 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/Band.py
--rw-rw-rw-   0        0        0     1861 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.740790 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.746646 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/
--rw-rw-rw-   0        0        0     1984 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/Scode.py
--rw-rw-rw-   0        0        0     1873 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/__init__.py
--rw-rw-rw-   0        0        0     1022 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.772023 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/
--rw-rw-rw-   0        0        0     1769 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Amode.py
--rw-rw-rw-   0        0        0     1578 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/CdThreshold.py
--rw-rw-rw-   0        0        0     1569 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Dmode.py
--rw-rw-rw-   0        0        0     1680 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/DsFactor.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.788616 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.794472 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/
--rw-rw-rw-   0        0        0     3273 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/Relative.py
--rw-rw-rw-   0        0        0     2423 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.799352 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/
--rw-rw-rw-   0        0        0     3389 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Absolute.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.805207 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/
--rw-rw-rw-   0        0        0     3292 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/Absolute.py
--rw-rw-rw-   0        0        0     1056 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/__init__.py
--rw-rw-rw-   0        0        0     3862 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/__init__.py
--rw-rw-rw-   0        0        0     2340 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/EvMagnitude.py
--rw-rw-rw-   0        0        0     2242 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Merror.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.813016 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/
--rw-rw-rw-   0        0        0     3477 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/EpStep.py
--rw-rw-rw-   0        0        0     3831 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/Hsdpcch.py
--rw-rw-rw-   0        0        0     1282 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Perror.py
--rw-rw-rw-   0        0        0     2510 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Phd.py
--rw-rw-rw-   0        0        0     3282 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/PhsDpcch.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.814967 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.817896 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.831560 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/
--rw-rw-rw-   0        0        0     3776 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpcch.py
--rw-rw-rw-   0        0        0     3776 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpdch.py
--rw-rw-rw-   0        0        0     3791 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpcch.py
--rw-rw-rw-   0        0        0     5737 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpdch.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.837416 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/
--rw-rw-rw-   0        0        0     2399 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/Config.py
--rw-rw-rw-   0        0        0     5173 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/__init__.py
--rw-rw-rw-   0        0        0    16214 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/__init__.py
--rw-rw-rw-   0        0        0     6072 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.844248 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.867672 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/
--rw-rw-rw-   0        0        0     4601 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/CdPower.py
--rw-rw-rw-   0        0        0     2189 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Cidx.py
--rw-rw-rw-   0        0        0     4631 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Modulation.py
--rw-rw-rw-   0        0        0     2185 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Phd.py
--rw-rw-rw-   0        0        0     5835 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Setup.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.874504 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/
--rw-rw-rw-   0        0        0     2181 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py
--rw-rw-rw-   0        0        0     1069 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py
--rw-rw-rw-   0        0        0     4176 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum.py
--rw-rw-rw-   0        0        0     2218 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/UePower.py
--rw-rw-rw-   0        0        0     3577 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py
--rw-rw-rw-   0        0        0     1542 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/SingleCmw.py
--rw-rw-rw-   0        0        0     8211 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Mperiod.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.879385 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/
--rw-rw-rw-   0        0        0     6121 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/Chip.py
--rw-rw-rw-   0        0        0    34819 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/__init__.py
--rw-rw-rw-   0        0        0     1754 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Rotation.py
--rw-rw-rw-   0        0        0     3853 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Scount.py
--rw-rw-rw-   0        0        0     1904 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Sscalar.py
--rw-rw-rw-   0        0        0    13688 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     2957 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OlpControl.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.885242 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/
--rw-rw-rw-   0        0        0     3032 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/Limit.py
--rw-rw-rw-   0        0        0     2658 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.887192 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.896952 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/
--rw-rw-rw-   0        0        0     2308 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/EvMagnitude.py
--rw-rw-rw-   0        0        0     2210 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Merror.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.904761 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.910617 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/
--rw-rw-rw-   0        0        0     3054 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/UserDefined.py
--rw-rw-rw-   0        0        0     6039 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/__init__.py
--rw-rw-rw-   0        0        0     2633 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/OlPower.py
--rw-rw-rw-   0        0        0     2683 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/Pstep.py
--rw-rw-rw-   0        0        0     2626 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/__init__.py
--rw-rw-rw-   0        0        0     2432 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Perror.py
--rw-rw-rw-   0        0        0     4812 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.916473 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/
--rw-rw-rw-   0        0        0     6536 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/Chip.py
--rw-rw-rw-   0        0        0    15082 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/__init__.py
--rw-rw-rw-   0        0        0     7868 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.921352 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.926233 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/
--rw-rw-rw-   0        0        0     2081 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/Frequency.py
--rw-rw-rw-   0        0        0     1905 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/__init__.py
--rw-rw-rw-   0        0        0     1497 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Dcarrier.py
--rw-rw-rw-   0        0        0     5041 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.939897 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.944777 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/
--rw-rw-rw-   0        0        0     2151 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/Mlength.py
--rw-rw-rw-   0        0        0     1024 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Dhib.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.952585 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/
--rw-rw-rw-   0        0        0     2326 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsef.py
--rw-rw-rw-   0        0        0     2530 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsgh.py
--rw-rw-rw-   0        0        0     3705 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.959417 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/
--rw-rw-rw-   0        0        0     2977 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ctfc.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.973081 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/
--rw-rw-rw-   0        0        0     2887 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/EpStep.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.977962 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/
--rw-rw-rw-   0        0        0     3128 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/UserDefined.py
--rw-rw-rw-   0        0        0     6166 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/__init__.py
--rw-rw-rw-   0        0        0     2421 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MinPower.py
--rw-rw-rw-   0        0        0     3861 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/PsGroup.py
--rw-rw-rw-   0        0        0     3101 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/Pstep.py
--rw-rw-rw-   0        0        0     2024 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/__init__.py
--rw-rw-rw-   0        0        0     2816 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Mpedch.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.985770 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/
--rw-rw-rw-   0        0        0     3147 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pa.py
--rw-rw-rw-   0        0        0     2615 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pb.py
--rw-rw-rw-   0        0        0     1190 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/__init__.py
--rw-rw-rw-   0        0        0     2569 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/__init__.py
--rw-rw-rw-   0        0        0     1338 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Monitor.py
--rw-rw-rw-   0        0        0     2175 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Mpedch.py
--rw-rw-rw-   0        0        0     2319 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ulcm.py
--rw-rw-rw-   0        0        0     9620 2023-09-04 10:02:04.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.988697 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.001386 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/
--rw-rw-rw-   0        0        0     3194 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpcch.py
--rw-rw-rw-   0        0        0     3194 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpdch.py
--rw-rw-rw-   0        0        0     3214 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpcch.py
--rw-rw-rw-   0        0        0     5161 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpdch.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.006265 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/
--rw-rw-rw-   0        0        0     2256 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/Config.py
--rw-rw-rw-   0        0        0     4561 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/__init__.py
--rw-rw-rw-   0        0        0     2817 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/__init__.py
--rw-rw-rw-   0        0        0     2133 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.009195 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.014075 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/
--rw-rw-rw-   0        0        0     1982 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/Scode.py
--rw-rw-rw-   0        0        0     1873 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/__init__.py
--rw-rw-rw-   0        0        0     5764 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/__init__.py
--rw-rw-rw-   0        0        0     3261 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.017002 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.018954 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.026762 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/
--rw-rw-rw-   0        0        0      892 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/MaProtocol.py
--rw-rw-rw-   0        0        0     2309 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/Salone.py
--rw-rw-rw-   0        0        0     2627 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/__init__.py
--rw-rw-rw-   0        0        0     1039 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.029690 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.031643 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.040427 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/
--rw-rw-rw-   0        0        0     1049 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     2365 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/ListPy.py
--rw-rw-rw-   0        0        0     9370 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.046282 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/
--rw-rw-rw-   0        0        0      893 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/Catalog.py
--rw-rw-rw-   0        0        0     6133 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.053115 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/
--rw-rw-rw-   0        0        0      881 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/Catalog.py
--rw-rw-rw-   0        0        0     5969 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.058973 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/
--rw-rw-rw-   0        0        0     1029 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/Catalog.py
--rw-rw-rw-   0        0        0     7544 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.064828 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/
--rw-rw-rw-   0        0        0     1021 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/Catalog.py
--rw-rw-rw-   0        0        0     8858 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/__init__.py
--rw-rw-rw-   0        0        0     2006 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.066779 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.071658 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/
--rw-rw-rw-   0        0        0     1831 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Ber.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.074587 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.088252 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/
--rw-rw-rw-   0        0        0     3681 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Average.py
--rw-rw-rw-   0        0        0     3681 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Current.py
--rw-rw-rw-   0        0        0     3681 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Maximum.py
--rw-rw-rw-   0        0        0     3713 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/StandardDev.py
--rw-rw-rw-   0        0        0     1803 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.105820 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/
--rw-rw-rw-   0        0        0     3699 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Average.py
--rw-rw-rw-   0        0        0     3699 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Current.py
--rw-rw-rw-   0        0        0     3699 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Maximum.py
--rw-rw-rw-   0        0        0     3699 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Minimum.py
--rw-rw-rw-   0        0        0     3731 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/StandardDev.py
--rw-rw-rw-   0        0        0     2048 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.121436 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/
--rw-rw-rw-   0        0        0     8301 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Average.py
--rw-rw-rw-   0        0        0     8248 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Current.py
--rw-rw-rw-   0        0        0     8301 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Maximum.py
--rw-rw-rw-   0        0        0     8343 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/StandardDev.py
--rw-rw-rw-   0        0        0     1819 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.139980 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/
--rw-rw-rw-   0        0        0     6589 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Average.py
--rw-rw-rw-   0        0        0     6589 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Current.py
--rw-rw-rw-   0        0        0     6589 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Maximum.py
--rw-rw-rw-   0        0        0     4326 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/OcInfo.py
--rw-rw-rw-   0        0        0     3480 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Sf.py
--rw-rw-rw-   0        0        0     6631 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/StandardDev.py
--rw-rw-rw-   0        0        0     2249 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.141932 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.144860 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.158525 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/
--rw-rw-rw-   0        0        0     3526 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Average.py
--rw-rw-rw-   0        0        0     3526 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Current.py
--rw-rw-rw-   0        0        0     3526 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Maximum.py
--rw-rw-rw-   0        0        0     3558 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1797 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.172189 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/
--rw-rw-rw-   0        0        0     3526 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Average.py
--rw-rw-rw-   0        0        0     3526 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Current.py
--rw-rw-rw-   0        0        0     3526 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Maximum.py
--rw-rw-rw-   0        0        0     3558 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/StandardDev.py
--rw-rw-rw-   0        0        0     1797 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.184877 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Average.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Current.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Maximum.py
--rw-rw-rw-   0        0        0     3576 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1802 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.197564 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/
--rw-rw-rw-   0        0        0     4160 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Average.py
--rw-rw-rw-   0        0        0     4160 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Current.py
--rw-rw-rw-   0        0        0     4160 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Maximum.py
--rw-rw-rw-   0        0        0     4192 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/StandardDev.py
--rw-rw-rw-   0        0        0     2708 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.211229 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Average.py
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Current.py
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Maximum.py
--rw-rw-rw-   0        0        0     3584 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1807 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/__init__.py
--rw-rw-rw-   0        0        0     1970 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.214158 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.230749 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Average.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Current.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Maximum.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Minimum.py
--rw-rw-rw-   0        0        0     3576 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/StandardDev.py
--rw-rw-rw-   0        0        0     2042 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.246365 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Average.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Current.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Maximum.py
--rw-rw-rw-   0        0        0     3544 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Minimum.py
--rw-rw-rw-   0        0        0     3576 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/StandardDev.py
--rw-rw-rw-   0        0        0     2042 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.265886 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/
--rw-rw-rw-   0        0        0     3562 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Average.py
--rw-rw-rw-   0        0        0     3562 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Current.py
--rw-rw-rw-   0        0        0     3562 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Maximum.py
--rw-rw-rw-   0        0        0     3562 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Minimum.py
--rw-rw-rw-   0        0        0     3594 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/StandardDev.py
--rw-rw-rw-   0        0        0     2047 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.283453 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/
--rw-rw-rw-   0        0        0     4178 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Average.py
--rw-rw-rw-   0        0        0     4178 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Current.py
--rw-rw-rw-   0        0        0     4178 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Maximum.py
--rw-rw-rw-   0        0        0     4178 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Minimum.py
--rw-rw-rw-   0        0        0     4210 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/StandardDev.py
--rw-rw-rw-   0        0        0     2953 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.301022 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/
--rw-rw-rw-   0        0        0     3570 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Average.py
--rw-rw-rw-   0        0        0     3570 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Current.py
--rw-rw-rw-   0        0        0     3570 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Maximum.py
--rw-rw-rw-   0        0        0     3570 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Minimum.py
--rw-rw-rw-   0        0        0     3602 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/StandardDev.py
--rw-rw-rw-   0        0        0     2052 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/__init__.py
--rw-rw-rw-   0        0        0     1970 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.302975 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.321519 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/
--rw-rw-rw-   0        0        0     3512 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Average.py
--rw-rw-rw-   0        0        0     3512 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Current.py
--rw-rw-rw-   0        0        0     3512 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Maximum.py
--rw-rw-rw-   0        0        0     2050 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Sdeviaton.py
--rw-rw-rw-   0        0        0     2064 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/StandardDev.py
--rw-rw-rw-   0        0        0     2052 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.338111 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/
--rw-rw-rw-   0        0        0     3504 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Average.py
--rw-rw-rw-   0        0        0     3504 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Current.py
--rw-rw-rw-   0        0        0     3504 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Maximum.py
--rw-rw-rw-   0        0        0     2046 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Sdeviaton.py
--rw-rw-rw-   0        0        0     2060 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/StandardDev.py
--rw-rw-rw-   0        0        0     2047 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/__init__.py
--rw-rw-rw-   0        0        0     1250 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.351776 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/
--rw-rw-rw-   0        0        0     3535 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Average.py
--rw-rw-rw-   0        0        0     3535 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Current.py
--rw-rw-rw-   0        0        0     3535 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Maximum.py
--rw-rw-rw-   0        0        0     3567 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/StandardDev.py
--rw-rw-rw-   0        0        0     1815 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.354702 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.368368 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/
--rw-rw-rw-   0        0        0     3554 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Average.py
--rw-rw-rw-   0        0        0     3554 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Current.py
--rw-rw-rw-   0        0        0     3554 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Maximum.py
--rw-rw-rw-   0        0        0     3586 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/StandardDev.py
--rw-rw-rw-   0        0        0     1792 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.383984 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/
--rw-rw-rw-   0        0        0     3546 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Average.py
--rw-rw-rw-   0        0        0     3546 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Current.py
--rw-rw-rw-   0        0        0     3546 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Maximum.py
--rw-rw-rw-   0        0        0     3578 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/StandardDev.py
--rw-rw-rw-   0        0        0     1787 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.387888 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.403503 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/
--rw-rw-rw-   0        0        0     3530 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Average.py
--rw-rw-rw-   0        0        0     3530 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Current.py
--rw-rw-rw-   0        0        0     3530 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Maximum.py
--rw-rw-rw-   0        0        0     3562 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/StandardDev.py
--rw-rw-rw-   0        0        0     1792 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.420096 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/
--rw-rw-rw-   0        0        0     3522 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Average.py
--rw-rw-rw-   0        0        0     2047 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Current.py
--rw-rw-rw-   0        0        0     3522 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Maximum.py
--rw-rw-rw-   0        0        0     3554 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/StandardDev.py
--rw-rw-rw-   0        0        0     1787 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/__init__.py
--rw-rw-rw-   0        0        0     1225 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.437665 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/
--rw-rw-rw-   0        0        0     3819 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Average.py
--rw-rw-rw-   0        0        0     3819 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Current.py
--rw-rw-rw-   0        0        0     3819 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Maximum.py
--rw-rw-rw-   0        0        0     3819 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Minimum.py
--rw-rw-rw-   0        0        0     3851 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/StandardDev.py
--rw-rw-rw-   0        0        0     2045 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.440592 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.453281 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Average.py
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Current.py
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Maximum.py
--rw-rw-rw-   0        0        0     3584 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1797 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.467921 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Average.py
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Current.py
--rw-rw-rw-   0        0        0     3552 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Maximum.py
--rw-rw-rw-   0        0        0     3584 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/StandardDev.py
--rw-rw-rw-   0        0        0     1797 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.481584 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/
--rw-rw-rw-   0        0        0     3570 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Average.py
--rw-rw-rw-   0        0        0     3570 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Current.py
--rw-rw-rw-   0        0        0     3570 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Maximum.py
--rw-rw-rw-   0        0        0     3602 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1802 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.497200 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/
--rw-rw-rw-   0        0        0     4186 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Average.py
--rw-rw-rw-   0        0        0     4186 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Current.py
--rw-rw-rw-   0        0        0     4186 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Maximum.py
--rw-rw-rw-   0        0        0     4218 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/StandardDev.py
--rw-rw-rw-   0        0        0     2708 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.510864 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/
--rw-rw-rw-   0        0        0     3578 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Average.py
--rw-rw-rw-   0        0        0     3578 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Current.py
--rw-rw-rw-   0        0        0     3578 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Maximum.py
--rw-rw-rw-   0        0        0     3610 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1807 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.525506 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/
--rw-rw-rw-   0        0        0     3086 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpcch.py
--rw-rw-rw-   0        0        0     3086 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpdch.py
--rw-rw-rw-   0        0        0     3123 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpcch.py
--rw-rw-rw-   0        0        0     5026 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpdch.py
--rw-rw-rw-   0        0        0     3134 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Hsdpcch.py
--rw-rw-rw-   0        0        0     1947 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/__init__.py
--rw-rw-rw-   0        0        0     2179 2023-09-04 10:02:06.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.543074 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/
--rw-rw-rw-   0        0        0     3455 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Average.py
--rw-rw-rw-   0        0        0     3455 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Current.py
--rw-rw-rw-   0        0        0     3455 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Maximum.py
--rw-rw-rw-   0        0        0     3455 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Minimum.py
--rw-rw-rw-   0        0        0     3487 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/StandardDev.py
--rw-rw-rw-   0        0        0     2050 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/__init__.py
--rw-rw-rw-   0        0        0     3015 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/__init__.py
--rw-rw-rw-   0        0        0     2879 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.548931 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.562594 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/
--rw-rw-rw-   0        0        0     3445 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Average.py
--rw-rw-rw-   0        0        0     3445 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Current.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.576257 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Average.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Current.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Maximum.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1795 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.589923 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Average.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Current.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Maximum.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/StandardDev.py
--rw-rw-rw-   0        0        0     1795 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.603586 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/
--rw-rw-rw-   0        0        0     1243 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Average.py
--rw-rw-rw-   0        0        0     1243 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Current.py
--rw-rw-rw-   0        0        0     1243 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Maximum.py
--rw-rw-rw-   0        0        0     1265 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1800 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.619202 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/
--rw-rw-rw-   0        0        0     1594 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Average.py
--rw-rw-rw-   0        0        0     1594 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Current.py
--rw-rw-rw-   0        0        0     1594 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Maximum.py
--rw-rw-rw-   0        0        0     1616 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/StandardDev.py
--rw-rw-rw-   0        0        0     2704 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.631890 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Average.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Current.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Maximum.py
--rw-rw-rw-   0        0        0     1270 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/StandardDev.py
--rw-rw-rw-   0        0        0     1805 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/__init__.py
--rw-rw-rw-   0        0        0     3445 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Maximum.py
--rw-rw-rw-   0        0        0     3467 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/StandardDev.py
--rw-rw-rw-   0        0        0     2976 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.647507 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/
--rw-rw-rw-   0        0        0     3445 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Average.py
--rw-rw-rw-   0        0        0     3445 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Current.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.665075 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Average.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Current.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Maximum.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Minimum.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/StandardDev.py
--rw-rw-rw-   0        0        0     2039 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.683619 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Average.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Current.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Maximum.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Minimum.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/StandardDev.py
--rw-rw-rw-   0        0        0     2039 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.699236 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/
--rw-rw-rw-   0        0        0     1243 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Average.py
--rw-rw-rw-   0        0        0     1243 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Current.py
--rw-rw-rw-   0        0        0     1243 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Maximum.py
--rw-rw-rw-   0        0        0     1243 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Minimum.py
--rw-rw-rw-   0        0        0     1265 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/StandardDev.py
--rw-rw-rw-   0        0        0     2044 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.714852 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/
--rw-rw-rw-   0        0        0     1594 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Average.py
--rw-rw-rw-   0        0        0     1594 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Current.py
--rw-rw-rw-   0        0        0     1594 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Maximum.py
--rw-rw-rw-   0        0        0     1594 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Minimum.py
--rw-rw-rw-   0        0        0     1616 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/StandardDev.py
--rw-rw-rw-   0        0        0     2948 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.731443 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Average.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Current.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Maximum.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Minimum.py
--rw-rw-rw-   0        0        0     1270 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/StandardDev.py
--rw-rw-rw-   0        0        0     2049 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/__init__.py
--rw-rw-rw-   0        0        0     3445 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Maximum.py
--rw-rw-rw-   0        0        0     3445 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Minimum.py
--rw-rw-rw-   0        0        0     3467 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/StandardDev.py
--rw-rw-rw-   0        0        0     3221 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.743156 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/
--rw-rw-rw-   0        0        0     3986 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Average.py
--rw-rw-rw-   0        0        0     3986 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Current.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.746084 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.758772 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/
--rw-rw-rw-   0        0        0     1251 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Average.py
--rw-rw-rw-   0        0        0     1251 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Current.py
--rw-rw-rw-   0        0        0     1251 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Maximum.py
--rw-rw-rw-   0        0        0     1273 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/StandardDev.py
--rw-rw-rw-   0        0        0     1792 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.773412 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/
--rw-rw-rw-   0        0        0     1246 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Average.py
--rw-rw-rw-   0        0        0     1246 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Current.py
--rw-rw-rw-   0        0        0     1246 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Maximum.py
--rw-rw-rw-   0        0        0     1268 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/StandardDev.py
--rw-rw-rw-   0        0        0     1787 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/__init__.py
--rw-rw-rw-   0        0        0     1209 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.789028 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Average.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Current.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Maximum.py
--rw-rw-rw-   0        0        0     1270 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/StandardDev.py
--rw-rw-rw-   0        0        0     1815 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.801717 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/
--rw-rw-rw-   0        0        0     1246 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Average.py
--rw-rw-rw-   0        0        0     1246 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Current.py
--rw-rw-rw-   0        0        0     1246 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Maximum.py
--rw-rw-rw-   0        0        0     1268 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/StandardDev.py
--rw-rw-rw-   0        0        0     1825 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.815381 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/
--rw-rw-rw-   0        0        0     1238 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Average.py
--rw-rw-rw-   0        0        0     1238 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Current.py
--rw-rw-rw-   0        0        0     1238 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Maximum.py
--rw-rw-rw-   0        0        0     1260 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/StandardDev.py
--rw-rw-rw-   0        0        0     1810 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/__init__.py
--rw-rw-rw-   0        0        0     3986 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Maximum.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.818309 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.831973 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Average.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Current.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Maximum.py
--rw-rw-rw-   0        0        0     1281 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/StandardDev.py
--rw-rw-rw-   0        0        0     1792 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.844662 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/
--rw-rw-rw-   0        0        0     1254 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Average.py
--rw-rw-rw-   0        0        0     1254 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Current.py
--rw-rw-rw-   0        0        0     1254 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Maximum.py
--rw-rw-rw-   0        0        0     1276 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/StandardDev.py
--rw-rw-rw-   0        0        0     1787 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/__init__.py
--rw-rw-rw-   0        0        0     1224 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.847590 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.860278 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/
--rw-rw-rw-   0        0        0     1257 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Average.py
--rw-rw-rw-   0        0        0     1257 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Current.py
--rw-rw-rw-   0        0        0     1257 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Maximum.py
--rw-rw-rw-   0        0        0     1279 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/StandardDev.py
--rw-rw-rw-   0        0        0     1792 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.880774 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/
--rw-rw-rw-   0        0        0     1252 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Average.py
--rw-rw-rw-   0        0        0     1252 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Current.py
--rw-rw-rw-   0        0        0     1252 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Maximum.py
--rw-rw-rw-   0        0        0     1274 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/StandardDev.py
--rw-rw-rw-   0        0        0     1787 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/__init__.py
--rw-rw-rw-   0        0        0     1224 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/__init__.py
--rw-rw-rw-   0        0        0     4008 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/StandardDev.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.896390 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/
--rw-rw-rw-   0        0        0     1247 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Average.py
--rw-rw-rw-   0        0        0     1247 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Current.py
--rw-rw-rw-   0        0        0     1247 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Maximum.py
--rw-rw-rw-   0        0        0     1269 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/StandardDev.py
--rw-rw-rw-   0        0        0     1805 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.910054 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Average.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Current.py
--rw-rw-rw-   0        0        0     1237 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Maximum.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/StandardDev.py
--rw-rw-rw-   0        0        0     1805 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/__init__.py
--rw-rw-rw-   0        0        0     3780 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.917862 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.926646 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/
--rw-rw-rw-   0        0        0     1252 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Current.py
--rw-rw-rw-   0        0        0     1252 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Maximum.py
--rw-rw-rw-   0        0        0     1270 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/__init__.py
--rw-rw-rw-   0        0        0     2670 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Current.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.933478 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/
--rw-rw-rw-   0        0        0     1216 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Current.py
--rw-rw-rw-   0        0        0     1216 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Maximum.py
--rw-rw-rw-   0        0        0     1275 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/__init__.py
--rw-rw-rw-   0        0        0     2670 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Maximum.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.942263 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/
--rw-rw-rw-   0        0        0     1438 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Current.py
--rw-rw-rw-   0        0        0     1438 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Maximum.py
--rw-rw-rw-   0        0        0     1275 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/__init__.py
--rw-rw-rw-   0        0        0     1944 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.948119 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/
--rw-rw-rw-   0        0        0     1764 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/Current.py
--rw-rw-rw-   0        0        0     1019 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.950071 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.962759 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/
--rw-rw-rw-   0        0        0     3150 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Average.py
--rw-rw-rw-   0        0        0     3150 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Current.py
--rw-rw-rw-   0        0        0     3150 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Maximum.py
--rw-rw-rw-   0        0        0     3172 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/StandardDev.py
--rw-rw-rw-   0        0        0     1805 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.979351 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/
--rw-rw-rw-   0        0        0     3149 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Average.py
--rw-rw-rw-   0        0        0     3149 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Current.py
--rw-rw-rw-   0        0        0     3149 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Maximum.py
--rw-rw-rw-   0        0        0     3149 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Minimum.py
--rw-rw-rw-   0        0        0     3171 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/StandardDev.py
--rw-rw-rw-   0        0        0     2049 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:13.993991 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/
--rw-rw-rw-   0        0        0     3572 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Average.py
--rw-rw-rw-   0        0        0     3572 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Current.py
--rw-rw-rw-   0        0        0     3572 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Maximum.py
--rw-rw-rw-   0        0        0     3594 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py
--rw-rw-rw-   0        0        0     1820 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.001799 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/
--rw-rw-rw-   0        0        0     2583 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Current.py
--rw-rw-rw-   0        0        0     2583 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Maximum.py
--rw-rw-rw-   0        0        0     1270 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.007656 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/
--rw-rw-rw-   0        0        0     2738 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/Current.py
--rw-rw-rw-   0        0        0     1021 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.018392 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/
--rw-rw-rw-   0        0        0     5447 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Average.py
--rw-rw-rw-   0        0        0     5447 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Current.py
--rw-rw-rw-   0        0        0     5447 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Maximum.py
--rw-rw-rw-   0        0        0     1534 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.024248 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/
--rw-rw-rw-   0        0        0     2529 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/Current.py
--rw-rw-rw-   0        0        0     1041 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/__init__.py
--rw-rw-rw-   0        0        0     3330 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.034983 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.037912 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.048649 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/
--rw-rw-rw-   0        0        0     2207 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Average.py
--rw-rw-rw-   0        0        0     2207 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Current.py
--rw-rw-rw-   0        0        0     2207 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Maximum.py
--rw-rw-rw-   0        0        0     2329 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.060360 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/
--rw-rw-rw-   0        0        0     2198 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Average.py
--rw-rw-rw-   0        0        0     2198 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Current.py
--rw-rw-rw-   0        0        0     2198 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Maximum.py
--rw-rw-rw-   0        0        0     2316 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/__init__.py
--rw-rw-rw-   0        0        0     1174 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/__init__.py
--rw-rw-rw-   0        0        0     6071 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Average.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.072073 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Average.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Current.py
--rw-rw-rw-   0        0        0     1248 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Maximum.py
--rw-rw-rw-   0        0        0     1524 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/__init__.py
--rw-rw-rw-   0        0        0     6071 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Current.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.075976 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.088665 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.101353 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.115017 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.124776 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.135514 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.146250 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.156985 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.168697 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Average.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Current.py
--rw-rw-rw-   0        0        0     1406 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Maximum.py
--rw-rw-rw-   0        0        0     1506 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.179434 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/
--rw-rw-rw-   0        0        0     1369 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Average.py
--rw-rw-rw-   0        0        0     1369 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Current.py
--rw-rw-rw-   0        0        0     1369 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Maximum.py
--rw-rw-rw-   0        0        0     1511 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.189195 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/
--rw-rw-rw-   0        0        0     1369 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Average.py
--rw-rw-rw-   0        0        0     1369 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Current.py
--rw-rw-rw-   0        0        0     1369 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Maximum.py
--rw-rw-rw-   0        0        0     1511 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/__init__.py
--rw-rw-rw-   0        0        0     2845 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/__init__.py
--rw-rw-rw-   0        0        0     6071 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Maximum.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.198954 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/
--rw-rw-rw-   0        0        0     1209 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Average.py
--rw-rw-rw-   0        0        0     1209 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Current.py
--rw-rw-rw-   0        0        0     1209 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Maximum.py
--rw-rw-rw-   0        0        0     1509 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.208715 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/
--rw-rw-rw-   0        0        0     1216 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Average.py
--rw-rw-rw-   0        0        0     1216 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Current.py
--rw-rw-rw-   0        0        0     1216 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Maximum.py
--rw-rw-rw-   0        0        0     1529 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/__init__.py
--rw-rw-rw-   0        0        0     2674 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/__init__.py
--rw-rw-rw-   0        0        0     1682 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Sreliability.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.214571 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/
--rw-rw-rw-   0        0        0     1552 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/Current.py
--rw-rw-rw-   0        0        0     1039 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/__init__.py
--rw-rw-rw-   0        0        0     3004 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.223354 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/
--rw-rw-rw-   0        0        0     6152 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/PhDhsDpcch.py
--rw-rw-rw-   0        0        0     5014 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/Uephd.py
--rw-rw-rw-   0        0        0     1304 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.230186 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/
--rw-rw-rw-   0        0        0     2444 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Current.py
--rw-rw-rw-   0        0        0     2444 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Maximum.py
--rw-rw-rw-   0        0        0     1266 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.239946 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/
--rw-rw-rw-   0        0        0    12874 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Average.py
--rw-rw-rw-   0        0        0    12874 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Current.py
--rw-rw-rw-   0        0        0    12874 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Maximum.py
--rw-rw-rw-   0        0        0     1530 2023-09-04 10:02:07.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.244827 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/
--rw-rw-rw-   0        0        0     2111 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/All.py
--rw-rw-rw-   0        0        0     2752 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.247754 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.249707 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.252636 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.257514 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/
--rw-rw-rw-   0        0        0     2043 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/Current.py
--rw-rw-rw-   0        0        0     1023 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/__init__.py
--rw-rw-rw-   0        0        0     1881 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.259467 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.264348 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/
--rw-rw-rw-   0        0        0     2228 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/Current.py
--rw-rw-rw-   0        0        0     1041 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.270204 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/
--rw-rw-rw-   0        0        0     2228 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/Current.py
--rw-rw-rw-   0        0        0     1041 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/__init__.py
--rw-rw-rw-   0        0        0     1298 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.273131 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.278987 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/
--rw-rw-rw-   0        0        0     2228 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/Current.py
--rw-rw-rw-   0        0        0     1041 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.285820 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/
--rw-rw-rw-   0        0        0     2228 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/Current.py
--rw-rw-rw-   0        0        0     1041 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/__init__.py
--rw-rw-rw-   0        0        0     1298 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.288747 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.300459 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/
--rw-rw-rw-   0        0        0     3170 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Average.py
--rw-rw-rw-   0        0        0     3170 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Current.py
--rw-rw-rw-   0        0        0     3170 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Maximum.py
--rw-rw-rw-   0        0        0     1529 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.312172 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/
--rw-rw-rw-   0        0        0     3178 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Average.py
--rw-rw-rw-   0        0        0     3178 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Current.py
--rw-rw-rw-   0        0        0     3178 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Maximum.py
--rw-rw-rw-   0        0        0     1534 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.323883 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/
--rw-rw-rw-   0        0        0     2980 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Average.py
--rw-rw-rw-   0        0        0     2980 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Current.py
--rw-rw-rw-   0        0        0     2980 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Maximum.py
--rw-rw-rw-   0        0        0     1529 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.334619 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/
--rw-rw-rw-   0        0        0     3574 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Average.py
--rw-rw-rw-   0        0        0     3574 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Current.py
--rw-rw-rw-   0        0        0     3574 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Maximum.py
--rw-rw-rw-   0        0        0     1524 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.346332 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/
--rw-rw-rw-   0        0        0     3582 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Average.py
--rw-rw-rw-   0        0        0     3582 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Current.py
--rw-rw-rw-   0        0        0     3582 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Maximum.py
--rw-rw-rw-   0        0        0     1529 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/__init__.py
--rw-rw-rw-   0        0        0     2006 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.349260 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.359996 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/
--rw-rw-rw-   0        0        0     2224 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Average.py
--rw-rw-rw-   0        0        0     2224 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Current.py
--rw-rw-rw-   0        0        0     2224 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Maximum.py
--rw-rw-rw-   0        0        0     1514 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.364876 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/
--rw-rw-rw-   0        0        0     2413 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/Current.py
--rw-rw-rw-   0        0        0     1014 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.367804 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.378540 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/
--rw-rw-rw-   0        0        0     2222 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Average.py
--rw-rw-rw-   0        0        0     2222 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Current.py
--rw-rw-rw-   0        0        0     2222 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Maximum.py
--rw-rw-rw-   0        0        0     1514 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/__init__.py
--rw-rw-rw-   0        0        0     1010 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.381468 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.392204 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/
--rw-rw-rw-   0        0        0     2226 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Average.py
--rw-rw-rw-   0        0        0     2226 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Current.py
--rw-rw-rw-   0        0        0     2226 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Maximum.py
--rw-rw-rw-   0        0        0     1514 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/__init__.py
--rw-rw-rw-   0        0        0     1010 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.397085 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/
--rw-rw-rw-   0        0        0     3212 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/Current.py
--rw-rw-rw-   0        0        0     1019 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/__init__.py
--rw-rw-rw-   0        0        0     2956 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/__init__.py
--rw-rw-rw-   0        0        0     5393 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.400014 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.402941 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.407821 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/
--rw-rw-rw-   0        0        0     4305 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/Rup.py
--rw-rw-rw-   0        0        0     1012 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/__init__.py
--rw-rw-rw-   0        0        0     1932 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.412701 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/
--rw-rw-rw-   0        0        0     1802 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/All.py
--rw-rw-rw-   0        0        0     2366 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/__init__.py
--rw-rw-rw-   0        0        0     5273 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.414653 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.419533 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/
--rw-rw-rw-   0        0        0     1790 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/All.py
--rw-rw-rw-   0        0        0     2354 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/__init__.py
--rw-rw-rw-   0        0        0     7073 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.424413 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/
--rw-rw-rw-   0        0        0     2340 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/OffPower.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.429294 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/
--rw-rw-rw-   0        0        0     6681 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/Current.py
--rw-rw-rw-   0        0        0     1903 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.435149 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/
--rw-rw-rw-   0        0        0     2095 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/All.py
--rw-rw-rw-   0        0        0     2736 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.437101 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.440029 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.445886 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/
--rw-rw-rw-   0        0        0     1920 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/Current.py
--rw-rw-rw-   0        0        0     1026 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.451741 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/
--rw-rw-rw-   0        0        0     2012 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/Current.py
--rw-rw-rw-   0        0        0     1026 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.456621 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/
--rw-rw-rw-   0        0        0     2010 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/Current.py
--rw-rw-rw-   0        0        0     1021 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/__init__.py
--rw-rw-rw-   0        0        0     1467 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.462477 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/
--rw-rw-rw-   0        0        0     1956 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/Current.py
--rw-rw-rw-   0        0        0     1049 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.466381 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/
--rw-rw-rw-   0        0        0     2405 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/Current.py
--rw-rw-rw-   0        0        0     1014 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.469310 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.474190 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/
--rw-rw-rw-   0        0        0     1888 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/Current.py
--rw-rw-rw-   0        0        0     1026 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.479069 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/
--rw-rw-rw-   0        0        0     2030 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/Current.py
--rw-rw-rw-   0        0        0     1026 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.484926 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/
--rw-rw-rw-   0        0        0     2028 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/Current.py
--rw-rw-rw-   0        0        0     1021 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/__init__.py
--rw-rw-rw-   0        0        0     1442 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.487854 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.494686 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/
--rw-rw-rw-   0        0        0     1884 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/Current.py
--rw-rw-rw-   0        0        0     1026 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.501518 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/
--rw-rw-rw-   0        0        0     2014 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/Current.py
--rw-rw-rw-   0        0        0     1026 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.508350 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/
--rw-rw-rw-   0        0        0     2012 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/Current.py
--rw-rw-rw-   0        0        0     1021 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/__init__.py
--rw-rw-rw-   0        0        0     1442 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.514206 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/
--rw-rw-rw-   0        0        0     2016 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/Current.py
--rw-rw-rw-   0        0        0     1034 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.519086 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.523967 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/
--rw-rw-rw-   0        0        0     2032 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/Current.py
--rw-rw-rw-   0        0        0     1026 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Current.py
--rw-rw-rw-   0        0        0     1259 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/__init__.py
--rw-rw-rw-   0        0        0     2476 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/__init__.py
--rw-rw-rw-   0        0        0     4396 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.526895 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.528847 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.542510 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/
--rw-rw-rw-   0        0        0    12080 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Average.py
--rw-rw-rw-   0        0        0    12080 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Maximum.py
--rw-rw-rw-   0        0        0    12080 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Minimum.py
--rw-rw-rw-   0        0        0     5524 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Statistics.py
--rw-rw-rw-   0        0        0     1791 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.545438 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.551295 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/
--rw-rw-rw-   0        0        0     5298 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/Current.py
--rw-rw-rw-   0        0        0     1036 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.556175 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/
--rw-rw-rw-   0        0        0     4350 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/Current.py
--rw-rw-rw-   0        0        0     1041 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.570814 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/
--rw-rw-rw-   0        0        0     5818 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Average.py
--rw-rw-rw-   0        0        0     5818 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Maximum.py
--rw-rw-rw-   0        0        0     5818 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Minimum.py
--rw-rw-rw-   0        0        0     3434 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Statistics.py
--rw-rw-rw-   0        0        0     1796 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/__init__.py
--rw-rw-rw-   0        0        0     2350 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.587408 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/
--rw-rw-rw-   0        0        0     3984 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Average.py
--rw-rw-rw-   0        0        0     3984 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Maximum.py
--rw-rw-rw-   0        0        0     2529 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimum.py
--rw-rw-rw-   0        0        0     1951 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimumc.py
--rw-rw-rw-   0        0        0     1910 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Statistics.py
--rw-rw-rw-   0        0        0     2031 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.593265 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/
--rw-rw-rw-   0        0        0     2089 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/All.py
--rw-rw-rw-   0        0        0     2730 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.596192 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.599119 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.603999 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/
--rw-rw-rw-   0        0        0     2078 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/Current.py
--rw-rw-rw-   0        0        0     1041 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.617664 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/
--rw-rw-rw-   0        0        0     2208 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Average.py
--rw-rw-rw-   0        0        0     2208 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Maximum.py
--rw-rw-rw-   0        0        0     2208 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Minimum.py
--rw-rw-rw-   0        0        0     2095 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Statistics.py
--rw-rw-rw-   0        0        0     1795 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/__init__.py
--rw-rw-rw-   0        0        0     1256 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/__init__.py
--rw-rw-rw-   0        0        0     4328 2023-09-04 10:02:08.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/__init__.py
--rw-rw-rw-   0        0        0     2005 2023-09-04 10:02:05.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:14.704530 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/
--rw-rw-rw-   0        0        0      586 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4165 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1116 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1145 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9097 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5751 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3439 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2546 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5238 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    25317 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3775 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4768 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    12939 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Core.py
--rw-rw-rw-   0        0        0     1386 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/GlobalData.py
--rw-rw-rw-   0        0        0    59853 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Instrument.py
--rw-rw-rw-   0        0        0     4785 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2225 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0    13241 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3518 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4390 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0     4289 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4745 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ScpiEnums.py
--rw-rw-rw-   0        0        0    35058 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ScpiLogger.py
--rw-rw-rw-   0        0        0     5098 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     5856 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1114 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/StructBase.py
--rw-rw-rw-   0        0        0     3608 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Types.py
--rw-rw-rw-   0        0        0     5498 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Utilities.py
--rw-rw-rw-   0        0        0     5632 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    50075 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     7361 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0       29 2023-07-13 05:46:50.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/__init__.py
--rw-rw-rw-   0        0        0    12666 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/RsCMPX_WcdmaMeas.py
--rw-rw-rw-   0        0        0      954 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/__init__.py
--rw-rw-rw-   0        0        0     8737 2023-09-04 10:02:03.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/enums.py
--rw-rw-rw-   0        0        0     5117 2023-09-04 10:01:59.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/repcap.py
-drwxrwxrwx   0        0        0        0 2023-09-04 10:02:12.711510 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/
--rw-rw-rw-   0        0        0     2791 2023-09-04 10:02:12.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    59677 2023-09-04 10:02:12.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-04 10:02:12.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-09-04 10:02:12.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-09-04 10:02:12.000000 RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-04 10:02:14.710385 RsCMPX_WcdmaMeas-4.0.186/setup.cfg
--rw-rw-rw-   0        0        0     1491 2023-09-04 10:02:09.000000 RsCMPX_WcdmaMeas-4.0.186/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:19.088828 RsCMPX_WcdmaMeas-5.0.40/
+-rw-rw-rw-   0        0        0     2860 2024-04-19 09:04:19.087831 RsCMPX_WcdmaMeas-5.0.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-04-19 09:04:14.000000 RsCMPX_WcdmaMeas-5.0.40/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.187912 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.212845 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/
+-rw-rw-rw-   0        0        0       90 2024-04-19 09:04:14.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3725 2024-04-19 09:04:14.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4916 2024-04-19 09:04:14.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    21869 2024-04-19 09:04:14.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.214840 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.216835 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.222818 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.226808 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/
+-rw-rw-rw-   0        0        0     2243 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/Band.py
+-rw-rw-rw-   0        0        0     1861 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.228802 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.232791 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/
+-rw-rw-rw-   0        0        0     1984 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/Scode.py
+-rw-rw-rw-   0        0        0     1873 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/__init__.py
+-rw-rw-rw-   0        0        0     1022 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.256728 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/
+-rw-rw-rw-   0        0        0     1769 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Amode.py
+-rw-rw-rw-   0        0        0     1578 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/CdThreshold.py
+-rw-rw-rw-   0        0        0     1569 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Dmode.py
+-rw-rw-rw-   0        0        0     1680 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/DsFactor.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.270691 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.275676 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/
+-rw-rw-rw-   0        0        0     3273 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/Relative.py
+-rw-rw-rw-   0        0        0     2429 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.280664 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/
+-rw-rw-rw-   0        0        0     3401 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Absolute.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.284653 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/
+-rw-rw-rw-   0        0        0     3292 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/Absolute.py
+-rw-rw-rw-   0        0        0     1056 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/__init__.py
+-rw-rw-rw-   0        0        0     3862 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/__init__.py
+-rw-rw-rw-   0        0        0     2340 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/EvMagnitude.py
+-rw-rw-rw-   0        0        0     2242 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Merror.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.291634 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/
+-rw-rw-rw-   0        0        0     3477 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/EpStep.py
+-rw-rw-rw-   0        0        0     3833 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/Hsdpcch.py
+-rw-rw-rw-   0        0        0     1282 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/__init__.py
+-rw-rw-rw-   0        0        0     2448 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Perror.py
+-rw-rw-rw-   0        0        0     2512 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Phd.py
+-rw-rw-rw-   0        0        0     3284 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/PhsDpcch.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.293628 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.296620 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.309586 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/
+-rw-rw-rw-   0        0        0     3776 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpcch.py
+-rw-rw-rw-   0        0        0     3776 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpdch.py
+-rw-rw-rw-   0        0        0     3791 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpcch.py
+-rw-rw-rw-   0        0        0     5737 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpdch.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.314573 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/
+-rw-rw-rw-   0        0        0     2399 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/Config.py
+-rw-rw-rw-   0        0        0     5173 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/__init__.py
+-rw-rw-rw-   0        0        0    16214 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/__init__.py
+-rw-rw-rw-   0        0        0     1033 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/__init__.py
+-rw-rw-rw-   0        0        0     4264 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/__init__.py
+-rw-rw-rw-   0        0        0     6072 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.319560 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.338509 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/
+-rw-rw-rw-   0        0        0     4607 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/CdPower.py
+-rw-rw-rw-   0        0        0     2197 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Cidx.py
+-rw-rw-rw-   0        0        0     4638 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Modulation.py
+-rw-rw-rw-   0        0        0     2185 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Phd.py
+-rw-rw-rw-   0        0        0     5861 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.343495 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/
+-rw-rw-rw-   0        0        0     2181 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py
+-rw-rw-rw-   0        0        0     1069 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py
+-rw-rw-rw-   0        0        0     4184 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum.py
+-rw-rw-rw-   0        0        0     2218 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/UePower.py
+-rw-rw-rw-   0        0        0     3577 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/SingleCmw.py
+-rw-rw-rw-   0        0        0     8211 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     1909 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Mperiod.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.347484 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/
+-rw-rw-rw-   0        0        0     6139 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/Chip.py
+-rw-rw-rw-   0        0        0    34910 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/__init__.py
+-rw-rw-rw-   0        0        0     1770 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Rotation.py
+-rw-rw-rw-   0        0        0     3853 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Scount.py
+-rw-rw-rw-   0        0        0     1896 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Sscalar.py
+-rw-rw-rw-   0        0        0    13666 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     2957 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OlpControl.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.351474 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/
+-rw-rw-rw-   0        0        0     3032 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/Limit.py
+-rw-rw-rw-   0        0        0     2658 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.354467 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.367431 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/
+-rw-rw-rw-   0        0        0     2308 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/EvMagnitude.py
+-rw-rw-rw-   0        0        0     2210 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Merror.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.377405 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.381394 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/
+-rw-rw-rw-   0        0        0     3054 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/UserDefined.py
+-rw-rw-rw-   0        0        0     6041 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/__init__.py
+-rw-rw-rw-   0        0        0     2637 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/OlPower.py
+-rw-rw-rw-   0        0        0     2689 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/Pstep.py
+-rw-rw-rw-   0        0        0     2632 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/__init__.py
+-rw-rw-rw-   0        0        0     2430 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Perror.py
+-rw-rw-rw-   0        0        0     4812 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.387380 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/
+-rw-rw-rw-   0        0        0     6560 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/Chip.py
+-rw-rw-rw-   0        0        0    15039 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/__init__.py
+-rw-rw-rw-   0        0        0     7860 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.392365 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.397351 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/
+-rw-rw-rw-   0        0        0     2081 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/Frequency.py
+-rw-rw-rw-   0        0        0     1905 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/__init__.py
+-rw-rw-rw-   0        0        0     1497 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Dcarrier.py
+-rw-rw-rw-   0        0        0     5093 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.414306 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.419293 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/
+-rw-rw-rw-   0        0        0     2154 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/Mlength.py
+-rw-rw-rw-   0        0        0     1024 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/__init__.py
+-rw-rw-rw-   0        0        0     3293 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Dhib.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.428269 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/
+-rw-rw-rw-   0        0        0     2326 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsef.py
+-rw-rw-rw-   0        0        0     2530 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsgh.py
+-rw-rw-rw-   0        0        0     3705 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.436248 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/
+-rw-rw-rw-   0        0        0     2991 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ctfc.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.448215 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/
+-rw-rw-rw-   0        0        0     2887 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/EpStep.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.454199 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/
+-rw-rw-rw-   0        0        0     3128 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/UserDefined.py
+-rw-rw-rw-   0        0        0     6166 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/__init__.py
+-rw-rw-rw-   0        0        0     2429 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MinPower.py
+-rw-rw-rw-   0        0        0     3885 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/PsGroup.py
+-rw-rw-rw-   0        0        0     3115 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/Pstep.py
+-rw-rw-rw-   0        0        0     2024 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/__init__.py
+-rw-rw-rw-   0        0        0     2824 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Mpedch.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.461181 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/
+-rw-rw-rw-   0        0        0     3147 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pa.py
+-rw-rw-rw-   0        0        0     2615 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pb.py
+-rw-rw-rw-   0        0        0     1190 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/__init__.py
+-rw-rw-rw-   0        0        0     2569 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/__init__.py
+-rw-rw-rw-   0        0        0     1338 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Monitor.py
+-rw-rw-rw-   0        0        0     2175 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Mpedch.py
+-rw-rw-rw-   0        0        0     2319 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ulcm.py
+-rw-rw-rw-   0        0        0     9612 2024-04-19 09:04:08.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.463175 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.475144 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/
+-rw-rw-rw-   0        0        0     3194 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpcch.py
+-rw-rw-rw-   0        0        0     3194 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpdch.py
+-rw-rw-rw-   0        0        0     3214 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpcch.py
+-rw-rw-rw-   0        0        0     5161 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpdch.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.479132 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/
+-rw-rw-rw-   0        0        0     2256 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/Config.py
+-rw-rw-rw-   0        0        0     4561 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/__init__.py
+-rw-rw-rw-   0        0        0     2817 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/__init__.py
+-rw-rw-rw-   0        0        0     2133 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.481128 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.487112 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/
+-rw-rw-rw-   0        0        0     1982 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/Scode.py
+-rw-rw-rw-   0        0        0     1873 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/__init__.py
+-rw-rw-rw-   0        0        0     5764 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/__init__.py
+-rw-rw-rw-   0        0        0     3261 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.489106 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.492099 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.499080 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/
+-rw-rw-rw-   0        0        0      894 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/MaProtocol.py
+-rw-rw-rw-   0        0        0     2309 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/Salone.py
+-rw-rw-rw-   0        0        0     2629 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.502071 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.504067 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.511048 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/
+-rw-rw-rw-   0        0        0     1049 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     2365 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/ListPy.py
+-rw-rw-rw-   0        0        0     9372 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.516035 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/
+-rw-rw-rw-   0        0        0      893 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/Catalog.py
+-rw-rw-rw-   0        0        0     6135 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.521022 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/
+-rw-rw-rw-   0        0        0      881 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/Catalog.py
+-rw-rw-rw-   0        0        0     5971 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.525009 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/
+-rw-rw-rw-   0        0        0     1029 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     7538 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.530995 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/
+-rw-rw-rw-   0        0        0     1021 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/Catalog.py
+-rw-rw-rw-   0        0        0     8860 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/__init__.py
+-rw-rw-rw-   0        0        0     2006 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.533987 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.537975 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/
+-rw-rw-rw-   0        0        0     1831 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Ber.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.541966 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.554931 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/
+-rw-rw-rw-   0        0        0     3681 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Average.py
+-rw-rw-rw-   0        0        0     3681 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Current.py
+-rw-rw-rw-   0        0        0     3681 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Maximum.py
+-rw-rw-rw-   0        0        0     3713 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/StandardDev.py
+-rw-rw-rw-   0        0        0     1803 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.569895 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/
+-rw-rw-rw-   0        0        0     3699 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Average.py
+-rw-rw-rw-   0        0        0     3699 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Current.py
+-rw-rw-rw-   0        0        0     3699 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Maximum.py
+-rw-rw-rw-   0        0        0     3699 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Minimum.py
+-rw-rw-rw-   0        0        0     3731 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2048 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.583853 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/
+-rw-rw-rw-   0        0        0     8319 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Average.py
+-rw-rw-rw-   0        0        0     8266 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Current.py
+-rw-rw-rw-   0        0        0     8319 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Maximum.py
+-rw-rw-rw-   0        0        0     8361 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/StandardDev.py
+-rw-rw-rw-   0        0        0     1819 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.602803 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/
+-rw-rw-rw-   0        0        0     6589 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Average.py
+-rw-rw-rw-   0        0        0     6589 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Current.py
+-rw-rw-rw-   0        0        0     6589 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Maximum.py
+-rw-rw-rw-   0        0        0     4337 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/OcInfo.py
+-rw-rw-rw-   0        0        0     3480 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Sf.py
+-rw-rw-rw-   0        0        0     6631 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/StandardDev.py
+-rw-rw-rw-   0        0        0     2249 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.605795 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.610782 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.625741 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/
+-rw-rw-rw-   0        0        0     3528 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Average.py
+-rw-rw-rw-   0        0        0     3528 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Current.py
+-rw-rw-rw-   0        0        0     3528 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3560 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1797 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.644690 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/
+-rw-rw-rw-   0        0        0     3528 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Average.py
+-rw-rw-rw-   0        0        0     3528 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Current.py
+-rw-rw-rw-   0        0        0     3528 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Maximum.py
+-rw-rw-rw-   0        0        0     3560 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     1797 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.657655 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/
+-rw-rw-rw-   0        0        0     3546 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Average.py
+-rw-rw-rw-   0        0        0     3546 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Current.py
+-rw-rw-rw-   0        0        0     3546 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3578 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1802 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.671618 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/
+-rw-rw-rw-   0        0        0     4160 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Average.py
+-rw-rw-rw-   0        0        0     4160 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Current.py
+-rw-rw-rw-   0        0        0     4160 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Maximum.py
+-rw-rw-rw-   0        0        0     4192 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     2708 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.684583 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Average.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Current.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3586 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1807 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/__init__.py
+-rw-rw-rw-   0        0        0     1970 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.688574 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.706525 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Average.py
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Current.py
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Minimum.py
+-rw-rw-rw-   0        0        0     3576 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     2042 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.723479 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Average.py
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Current.py
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Maximum.py
+-rw-rw-rw-   0        0        0     3544 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Minimum.py
+-rw-rw-rw-   0        0        0     3576 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     2042 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.741431 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/
+-rw-rw-rw-   0        0        0     3564 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Average.py
+-rw-rw-rw-   0        0        0     3564 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Current.py
+-rw-rw-rw-   0        0        0     3564 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3564 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Minimum.py
+-rw-rw-rw-   0        0        0     3596 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     2047 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.757388 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/
+-rw-rw-rw-   0        0        0     4178 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Average.py
+-rw-rw-rw-   0        0        0     4178 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Current.py
+-rw-rw-rw-   0        0        0     4178 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Maximum.py
+-rw-rw-rw-   0        0        0     4178 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Minimum.py
+-rw-rw-rw-   0        0        0     4210 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     2953 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.775340 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Average.py
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Current.py
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Minimum.py
+-rw-rw-rw-   0        0        0     3604 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     2052 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/__init__.py
+-rw-rw-rw-   0        0        0     1970 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.778332 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.794291 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/
+-rw-rw-rw-   0        0        0     3512 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Average.py
+-rw-rw-rw-   0        0        0     3512 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Current.py
+-rw-rw-rw-   0        0        0     3512 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     2050 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Sdeviaton.py
+-rw-rw-rw-   0        0        0     2064 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/StandardDev.py
+-rw-rw-rw-   0        0        0     2052 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.819223 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/
+-rw-rw-rw-   0        0        0     3504 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Average.py
+-rw-rw-rw-   0        0        0     3504 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Current.py
+-rw-rw-rw-   0        0        0     3504 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     2046 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Sdeviaton.py
+-rw-rw-rw-   0        0        0     2060 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/StandardDev.py
+-rw-rw-rw-   0        0        0     2047 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1250 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.834183 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/
+-rw-rw-rw-   0        0        0     3535 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Average.py
+-rw-rw-rw-   0        0        0     3535 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Current.py
+-rw-rw-rw-   0        0        0     3535 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Maximum.py
+-rw-rw-rw-   0        0        0     3567 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/StandardDev.py
+-rw-rw-rw-   0        0        0     1815 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.837176 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.851138 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Average.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Current.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     3586 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/StandardDev.py
+-rw-rw-rw-   0        0        0     1792 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.865100 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/
+-rw-rw-rw-   0        0        0     3546 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Average.py
+-rw-rw-rw-   0        0        0     3546 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Current.py
+-rw-rw-rw-   0        0        0     3546 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     3578 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/StandardDev.py
+-rw-rw-rw-   0        0        0     1787 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1225 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.867096 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.882056 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/
+-rw-rw-rw-   0        0        0     3530 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Average.py
+-rw-rw-rw-   0        0        0     3530 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Current.py
+-rw-rw-rw-   0        0        0     3530 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     3562 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/StandardDev.py
+-rw-rw-rw-   0        0        0     1792 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.895022 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/
+-rw-rw-rw-   0        0        0     3522 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Average.py
+-rw-rw-rw-   0        0        0     2047 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Current.py
+-rw-rw-rw-   0        0        0     3522 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/StandardDev.py
+-rw-rw-rw-   0        0        0     1787 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1225 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.908984 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/
+-rw-rw-rw-   0        0        0     3819 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Average.py
+-rw-rw-rw-   0        0        0     3819 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Current.py
+-rw-rw-rw-   0        0        0     3819 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Maximum.py
+-rw-rw-rw-   0        0        0     3819 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Minimum.py
+-rw-rw-rw-   0        0        0     3851 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/StandardDev.py
+-rw-rw-rw-   0        0        0     2045 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.910978 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.922946 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Average.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Current.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3586 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1797 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.936909 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Average.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Current.py
+-rw-rw-rw-   0        0        0     3554 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Maximum.py
+-rw-rw-rw-   0        0        0     3586 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     1797 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.948876 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Average.py
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Current.py
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3604 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1802 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.960844 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/
+-rw-rw-rw-   0        0        0     4186 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Average.py
+-rw-rw-rw-   0        0        0     4186 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Current.py
+-rw-rw-rw-   0        0        0     4186 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Maximum.py
+-rw-rw-rw-   0        0        0     4218 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     2708 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.971816 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/
+-rw-rw-rw-   0        0        0     3580 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Average.py
+-rw-rw-rw-   0        0        0     3580 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Current.py
+-rw-rw-rw-   0        0        0     3580 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Maximum.py
+-rw-rw-rw-   0        0        0     3612 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1807 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.987773 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/
+-rw-rw-rw-   0        0        0     3088 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpcch.py
+-rw-rw-rw-   0        0        0     3088 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpdch.py
+-rw-rw-rw-   0        0        0     3125 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpcch.py
+-rw-rw-rw-   0        0        0     5026 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpdch.py
+-rw-rw-rw-   0        0        0     3136 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Hsdpcch.py
+-rw-rw-rw-   0        0        0     1947 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/__init__.py
+-rw-rw-rw-   0        0        0     2179 2024-04-19 09:04:10.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.004728 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/
+-rw-rw-rw-   0        0        0     3455 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Average.py
+-rw-rw-rw-   0        0        0     3455 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Current.py
+-rw-rw-rw-   0        0        0     3455 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Maximum.py
+-rw-rw-rw-   0        0        0     3455 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Minimum.py
+-rw-rw-rw-   0        0        0     3487 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/StandardDev.py
+-rw-rw-rw-   0        0        0     2050 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/__init__.py
+-rw-rw-rw-   0        0        0     3015 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/__init__.py
+-rw-rw-rw-   0        0        0     2879 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.010712 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.025671 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/
+-rw-rw-rw-   0        0        0     3445 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Average.py
+-rw-rw-rw-   0        0        0     3445 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.036643 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Average.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Current.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Maximum.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1795 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.050605 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Average.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Current.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Maximum.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     1795 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.063570 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/
+-rw-rw-rw-   0        0        0     1243 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Average.py
+-rw-rw-rw-   0        0        0     1243 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Current.py
+-rw-rw-rw-   0        0        0     1243 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Maximum.py
+-rw-rw-rw-   0        0        0     1265 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1800 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.075538 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/
+-rw-rw-rw-   0        0        0     1594 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Average.py
+-rw-rw-rw-   0        0        0     1594 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Current.py
+-rw-rw-rw-   0        0        0     1594 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Maximum.py
+-rw-rw-rw-   0        0        0     1616 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     2704 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.088503 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Average.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Current.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Maximum.py
+-rw-rw-rw-   0        0        0     1270 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     1805 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/__init__.py
+-rw-rw-rw-   0        0        0     3445 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Maximum.py
+-rw-rw-rw-   0        0        0     3467 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/StandardDev.py
+-rw-rw-rw-   0        0        0     2976 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.103464 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/
+-rw-rw-rw-   0        0        0     3445 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Average.py
+-rw-rw-rw-   0        0        0     3445 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.119422 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Average.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Current.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Maximum.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Minimum.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     2039 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.137373 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Average.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Current.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Maximum.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Minimum.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     2039 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.150338 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/
+-rw-rw-rw-   0        0        0     1243 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Average.py
+-rw-rw-rw-   0        0        0     1243 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Current.py
+-rw-rw-rw-   0        0        0     1243 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Maximum.py
+-rw-rw-rw-   0        0        0     1243 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Minimum.py
+-rw-rw-rw-   0        0        0     1265 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     2044 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.165298 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/
+-rw-rw-rw-   0        0        0     1594 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Average.py
+-rw-rw-rw-   0        0        0     1594 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Current.py
+-rw-rw-rw-   0        0        0     1594 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Maximum.py
+-rw-rw-rw-   0        0        0     1594 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Minimum.py
+-rw-rw-rw-   0        0        0     1616 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/StandardDev.py
+-rw-rw-rw-   0        0        0     2948 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.180259 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Average.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Current.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Maximum.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Minimum.py
+-rw-rw-rw-   0        0        0     1270 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/StandardDev.py
+-rw-rw-rw-   0        0        0     2049 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/__init__.py
+-rw-rw-rw-   0        0        0     3445 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Maximum.py
+-rw-rw-rw-   0        0        0     3445 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Minimum.py
+-rw-rw-rw-   0        0        0     3467 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/StandardDev.py
+-rw-rw-rw-   0        0        0     3221 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.193223 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/
+-rw-rw-rw-   0        0        0     3986 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Average.py
+-rw-rw-rw-   0        0        0     3986 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.196216 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.207187 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/
+-rw-rw-rw-   0        0        0     1251 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Average.py
+-rw-rw-rw-   0        0        0     1251 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Current.py
+-rw-rw-rw-   0        0        0     1251 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     1273 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/StandardDev.py
+-rw-rw-rw-   0        0        0     1792 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.221149 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/
+-rw-rw-rw-   0        0        0     1246 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Average.py
+-rw-rw-rw-   0        0        0     1246 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Current.py
+-rw-rw-rw-   0        0        0     1246 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     1268 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/StandardDev.py
+-rw-rw-rw-   0        0        0     1787 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1209 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.235112 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Average.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Current.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Maximum.py
+-rw-rw-rw-   0        0        0     1270 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/StandardDev.py
+-rw-rw-rw-   0        0        0     1815 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.250071 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/
+-rw-rw-rw-   0        0        0     1246 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Average.py
+-rw-rw-rw-   0        0        0     1246 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Current.py
+-rw-rw-rw-   0        0        0     1246 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Maximum.py
+-rw-rw-rw-   0        0        0     1268 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/StandardDev.py
+-rw-rw-rw-   0        0        0     1825 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.264034 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/
+-rw-rw-rw-   0        0        0     1238 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Average.py
+-rw-rw-rw-   0        0        0     1238 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Current.py
+-rw-rw-rw-   0        0        0     1238 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Maximum.py
+-rw-rw-rw-   0        0        0     1260 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/StandardDev.py
+-rw-rw-rw-   0        0        0     1810 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/__init__.py
+-rw-rw-rw-   0        0        0     3986 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Maximum.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.267027 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.277997 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Average.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Current.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     1281 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/StandardDev.py
+-rw-rw-rw-   0        0        0     1792 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.289965 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/
+-rw-rw-rw-   0        0        0     1254 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Average.py
+-rw-rw-rw-   0        0        0     1254 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Current.py
+-rw-rw-rw-   0        0        0     1254 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     1276 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/StandardDev.py
+-rw-rw-rw-   0        0        0     1787 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.292957 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.306919 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/
+-rw-rw-rw-   0        0        0     1257 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Average.py
+-rw-rw-rw-   0        0        0     1257 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Current.py
+-rw-rw-rw-   0        0        0     1257 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     1279 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/StandardDev.py
+-rw-rw-rw-   0        0        0     1792 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.319884 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/
+-rw-rw-rw-   0        0        0     1252 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Average.py
+-rw-rw-rw-   0        0        0     1252 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Current.py
+-rw-rw-rw-   0        0        0     1252 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     1274 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/StandardDev.py
+-rw-rw-rw-   0        0        0     1787 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1224 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/__init__.py
+-rw-rw-rw-   0        0        0     4008 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/StandardDev.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.331852 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/
+-rw-rw-rw-   0        0        0     1247 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Average.py
+-rw-rw-rw-   0        0        0     1247 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Current.py
+-rw-rw-rw-   0        0        0     1247 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Maximum.py
+-rw-rw-rw-   0        0        0     1269 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/StandardDev.py
+-rw-rw-rw-   0        0        0     1805 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.343820 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Average.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Current.py
+-rw-rw-rw-   0        0        0     1237 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Maximum.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/StandardDev.py
+-rw-rw-rw-   0        0        0     1805 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/__init__.py
+-rw-rw-rw-   0        0        0     3780 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.349804 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.357784 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/
+-rw-rw-rw-   0        0        0     1252 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Current.py
+-rw-rw-rw-   0        0        0     1252 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Maximum.py
+-rw-rw-rw-   0        0        0     1270 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/__init__.py
+-rw-rw-rw-   0        0        0     2671 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.365761 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/
+-rw-rw-rw-   0        0        0     1216 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Current.py
+-rw-rw-rw-   0        0        0     1216 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Maximum.py
+-rw-rw-rw-   0        0        0     1275 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/__init__.py
+-rw-rw-rw-   0        0        0     2671 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Maximum.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.373742 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/
+-rw-rw-rw-   0        0        0     1438 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Current.py
+-rw-rw-rw-   0        0        0     1438 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Maximum.py
+-rw-rw-rw-   0        0        0     1275 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/__init__.py
+-rw-rw-rw-   0        0        0     1944 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.378729 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/
+-rw-rw-rw-   0        0        0     1764 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/Current.py
+-rw-rw-rw-   0        0        0     1019 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.381719 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.393687 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/
+-rw-rw-rw-   0        0        0     3150 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Average.py
+-rw-rw-rw-   0        0        0     3150 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Current.py
+-rw-rw-rw-   0        0        0     3150 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Maximum.py
+-rw-rw-rw-   0        0        0     3172 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/StandardDev.py
+-rw-rw-rw-   0        0        0     1805 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.410643 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/
+-rw-rw-rw-   0        0        0     3149 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Average.py
+-rw-rw-rw-   0        0        0     3149 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Current.py
+-rw-rw-rw-   0        0        0     3149 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Maximum.py
+-rw-rw-rw-   0        0        0     3149 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Minimum.py
+-rw-rw-rw-   0        0        0     3171 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/StandardDev.py
+-rw-rw-rw-   0        0        0     2049 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.423607 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Average.py
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Current.py
+-rw-rw-rw-   0        0        0     3572 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Maximum.py
+-rw-rw-rw-   0        0        0     3594 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py
+-rw-rw-rw-   0        0        0     1820 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.433581 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/
+-rw-rw-rw-   0        0        0     2583 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Current.py
+-rw-rw-rw-   0        0        0     2583 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Maximum.py
+-rw-rw-rw-   0        0        0     1270 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.439565 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/
+-rw-rw-rw-   0        0        0     2738 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/Current.py
+-rw-rw-rw-   0        0        0     1021 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.450536 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/
+-rw-rw-rw-   0        0        0     5458 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Average.py
+-rw-rw-rw-   0        0        0     5458 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Current.py
+-rw-rw-rw-   0        0        0     5458 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Maximum.py
+-rw-rw-rw-   0        0        0     1534 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.455522 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/
+-rw-rw-rw-   0        0        0     2529 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/__init__.py
+-rw-rw-rw-   0        0        0     3330 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.464498 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.466492 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.475469 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/
+-rw-rw-rw-   0        0        0     2218 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Average.py
+-rw-rw-rw-   0        0        0     2218 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Current.py
+-rw-rw-rw-   0        0        0     2218 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Maximum.py
+-rw-rw-rw-   0        0        0     2329 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.485442 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/
+-rw-rw-rw-   0        0        0     2209 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Average.py
+-rw-rw-rw-   0        0        0     2209 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Current.py
+-rw-rw-rw-   0        0        0     2209 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Maximum.py
+-rw-rw-rw-   0        0        0     2316 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/__init__.py
+-rw-rw-rw-   0        0        0     1174 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/__init__.py
+-rw-rw-rw-   0        0        0     6082 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Average.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.496412 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Average.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Current.py
+-rw-rw-rw-   0        0        0     1248 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Maximum.py
+-rw-rw-rw-   0        0        0     1524 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/__init__.py
+-rw-rw-rw-   0        0        0     6082 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.499404 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.510375 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.519352 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.530322 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.540295 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.551266 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.562237 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.572210 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.581185 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Average.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Current.py
+-rw-rw-rw-   0        0        0     1406 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Maximum.py
+-rw-rw-rw-   0        0        0     1506 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.590162 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/
+-rw-rw-rw-   0        0        0     1369 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Average.py
+-rw-rw-rw-   0        0        0     1369 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Current.py
+-rw-rw-rw-   0        0        0     1369 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Maximum.py
+-rw-rw-rw-   0        0        0     1511 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.599137 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/
+-rw-rw-rw-   0        0        0     1369 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Average.py
+-rw-rw-rw-   0        0        0     1369 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Current.py
+-rw-rw-rw-   0        0        0     1369 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Maximum.py
+-rw-rw-rw-   0        0        0     1511 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/__init__.py
+-rw-rw-rw-   0        0        0     2845 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/__init__.py
+-rw-rw-rw-   0        0        0     6082 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Maximum.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.610109 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/
+-rw-rw-rw-   0        0        0     1209 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Average.py
+-rw-rw-rw-   0        0        0     1209 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Current.py
+-rw-rw-rw-   0        0        0     1209 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Maximum.py
+-rw-rw-rw-   0        0        0     1509 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.621081 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/
+-rw-rw-rw-   0        0        0     1216 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Average.py
+-rw-rw-rw-   0        0        0     1216 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Current.py
+-rw-rw-rw-   0        0        0     1216 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Maximum.py
+-rw-rw-rw-   0        0        0     1529 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/__init__.py
+-rw-rw-rw-   0        0        0     2674 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/__init__.py
+-rw-rw-rw-   0        0        0     1682 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Sreliability.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.628062 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/
+-rw-rw-rw-   0        0        0     1552 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/Current.py
+-rw-rw-rw-   0        0        0     1039 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.639032 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/
+-rw-rw-rw-   0        0        0     6152 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/PhDhsDpcch.py
+-rw-rw-rw-   0        0        0     5038 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/Uephd.py
+-rw-rw-rw-   0        0        0     1304 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.647011 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/
+-rw-rw-rw-   0        0        0     2446 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Current.py
+-rw-rw-rw-   0        0        0     2446 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Maximum.py
+-rw-rw-rw-   0        0        0     1266 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.657981 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/
+-rw-rw-rw-   0        0        0    12896 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Average.py
+-rw-rw-rw-   0        0        0    12896 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Current.py
+-rw-rw-rw-   0        0        0    12896 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Maximum.py
+-rw-rw-rw-   0        0        0     1530 2024-04-19 09:04:11.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.662967 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/
+-rw-rw-rw-   0        0        0     2111 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/All.py
+-rw-rw-rw-   0        0        0     2752 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.665959 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.668953 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.670946 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.676930 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/
+-rw-rw-rw-   0        0        0     2043 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/Current.py
+-rw-rw-rw-   0        0        0     1023 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1004 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/__init__.py
+-rw-rw-rw-   0        0        0     1881 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.679922 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.685906 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/
+-rw-rw-rw-   0        0        0     2228 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.690892 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/
+-rw-rw-rw-   0        0        0     2228 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/__init__.py
+-rw-rw-rw-   0        0        0     1298 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.693884 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.699868 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/
+-rw-rw-rw-   0        0        0     2228 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.704856 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/
+-rw-rw-rw-   0        0        0     2228 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/__init__.py
+-rw-rw-rw-   0        0        0     1298 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.706850 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.714828 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/
+-rw-rw-rw-   0        0        0     3170 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Average.py
+-rw-rw-rw-   0        0        0     3170 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Current.py
+-rw-rw-rw-   0        0        0     3170 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Maximum.py
+-rw-rw-rw-   0        0        0     1529 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.724802 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/
+-rw-rw-rw-   0        0        0     3178 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Average.py
+-rw-rw-rw-   0        0        0     3178 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Current.py
+-rw-rw-rw-   0        0        0     3178 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Maximum.py
+-rw-rw-rw-   0        0        0     1534 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.735772 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/
+-rw-rw-rw-   0        0        0     2980 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Average.py
+-rw-rw-rw-   0        0        0     2980 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Current.py
+-rw-rw-rw-   0        0        0     2980 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Maximum.py
+-rw-rw-rw-   0        0        0     1529 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.745746 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/
+-rw-rw-rw-   0        0        0     3574 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Average.py
+-rw-rw-rw-   0        0        0     3574 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Current.py
+-rw-rw-rw-   0        0        0     3574 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Maximum.py
+-rw-rw-rw-   0        0        0     1524 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.754722 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/
+-rw-rw-rw-   0        0        0     3582 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Average.py
+-rw-rw-rw-   0        0        0     3582 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Current.py
+-rw-rw-rw-   0        0        0     3582 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Maximum.py
+-rw-rw-rw-   0        0        0     1529 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/__init__.py
+-rw-rw-rw-   0        0        0     2006 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.756717 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.766690 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/
+-rw-rw-rw-   0        0        0     2224 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Average.py
+-rw-rw-rw-   0        0        0     2224 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Current.py
+-rw-rw-rw-   0        0        0     2224 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Maximum.py
+-rw-rw-rw-   0        0        0     1514 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/__init__.py
+-rw-rw-rw-   0        0        0     1035 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.770679 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/
+-rw-rw-rw-   0        0        0     2413 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/Current.py
+-rw-rw-rw-   0        0        0     1014 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.772674 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.782648 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/
+-rw-rw-rw-   0        0        0     2222 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Average.py
+-rw-rw-rw-   0        0        0     2222 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Current.py
+-rw-rw-rw-   0        0        0     2222 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Maximum.py
+-rw-rw-rw-   0        0        0     1514 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/__init__.py
+-rw-rw-rw-   0        0        0     1010 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.784642 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.794614 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/
+-rw-rw-rw-   0        0        0     2226 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Average.py
+-rw-rw-rw-   0        0        0     2226 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Current.py
+-rw-rw-rw-   0        0        0     2226 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Maximum.py
+-rw-rw-rw-   0        0        0     1514 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/__init__.py
+-rw-rw-rw-   0        0        0     1010 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.799601 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/
+-rw-rw-rw-   0        0        0     3212 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/Current.py
+-rw-rw-rw-   0        0        0     1019 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/__init__.py
+-rw-rw-rw-   0        0        0     2956 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/__init__.py
+-rw-rw-rw-   0        0        0     5390 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.801596 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.804588 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.809576 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/
+-rw-rw-rw-   0        0        0     4305 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/Rup.py
+-rw-rw-rw-   0        0        0     1012 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/__init__.py
+-rw-rw-rw-   0        0        0     1932 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.814562 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/
+-rw-rw-rw-   0        0        0     1802 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/All.py
+-rw-rw-rw-   0        0        0     2366 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/__init__.py
+-rw-rw-rw-   0        0        0     5273 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.816556 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.821545 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/
+-rw-rw-rw-   0        0        0     1790 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/All.py
+-rw-rw-rw-   0        0        0     2354 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/__init__.py
+-rw-rw-rw-   0        0        0     7073 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.826529 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/
+-rw-rw-rw-   0        0        0     2340 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/OffPower.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.831517 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/
+-rw-rw-rw-   0        0        0     6691 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/Current.py
+-rw-rw-rw-   0        0        0     1903 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.839496 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/
+-rw-rw-rw-   0        0        0     2095 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/All.py
+-rw-rw-rw-   0        0        0     2736 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.842487 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.845479 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.850466 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/
+-rw-rw-rw-   0        0        0     1920 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/Current.py
+-rw-rw-rw-   0        0        0     1026 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.855453 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/
+-rw-rw-rw-   0        0        0     2012 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/Current.py
+-rw-rw-rw-   0        0        0     1026 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.860439 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/
+-rw-rw-rw-   0        0        0     2010 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/Current.py
+-rw-rw-rw-   0        0        0     1021 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1467 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.865425 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/
+-rw-rw-rw-   0        0        0     1954 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/Current.py
+-rw-rw-rw-   0        0        0     1049 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.870413 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/
+-rw-rw-rw-   0        0        0     2405 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/Current.py
+-rw-rw-rw-   0        0        0     1014 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.872408 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.878393 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/
+-rw-rw-rw-   0        0        0     1888 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/Current.py
+-rw-rw-rw-   0        0        0     1026 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.882381 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/
+-rw-rw-rw-   0        0        0     2030 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/Current.py
+-rw-rw-rw-   0        0        0     1026 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.888365 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/
+-rw-rw-rw-   0        0        0     2028 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/Current.py
+-rw-rw-rw-   0        0        0     1021 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1442 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.890359 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.894349 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/
+-rw-rw-rw-   0        0        0     1884 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/Current.py
+-rw-rw-rw-   0        0        0     1026 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.899336 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/
+-rw-rw-rw-   0        0        0     2014 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/Current.py
+-rw-rw-rw-   0        0        0     1026 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.904322 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/
+-rw-rw-rw-   0        0        0     2012 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/Current.py
+-rw-rw-rw-   0        0        0     1021 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/__init__.py
+-rw-rw-rw-   0        0        0     1442 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.908311 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/
+-rw-rw-rw-   0        0        0     2016 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/Current.py
+-rw-rw-rw-   0        0        0     1034 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.913297 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.918284 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/
+-rw-rw-rw-   0        0        0     2032 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/Current.py
+-rw-rw-rw-   0        0        0     1026 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/__init__.py
+-rw-rw-rw-   0        0        0     1940 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Current.py
+-rw-rw-rw-   0        0        0     1259 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/__init__.py
+-rw-rw-rw-   0        0        0     2476 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/__init__.py
+-rw-rw-rw-   0        0        0     4393 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.921280 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.923271 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.937234 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/
+-rw-rw-rw-   0        0        0    12080 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Average.py
+-rw-rw-rw-   0        0        0    12080 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Maximum.py
+-rw-rw-rw-   0        0        0    12080 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Minimum.py
+-rw-rw-rw-   0        0        0     5527 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Statistics.py
+-rw-rw-rw-   0        0        0     1791 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.940226 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.946210 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/
+-rw-rw-rw-   0        0        0     5298 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/Current.py
+-rw-rw-rw-   0        0        0     1036 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.951196 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/
+-rw-rw-rw-   0        0        0     4350 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/__init__.py
+-rw-rw-rw-   0        0        0     1265 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.963164 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/
+-rw-rw-rw-   0        0        0     5818 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Average.py
+-rw-rw-rw-   0        0        0     5818 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Maximum.py
+-rw-rw-rw-   0        0        0     5818 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Minimum.py
+-rw-rw-rw-   0        0        0     3434 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Statistics.py
+-rw-rw-rw-   0        0        0     1796 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/__init__.py
+-rw-rw-rw-   0        0        0     2350 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.977127 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/
+-rw-rw-rw-   0        0        0     3988 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Average.py
+-rw-rw-rw-   0        0        0     3988 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Maximum.py
+-rw-rw-rw-   0        0        0     2531 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimum.py
+-rw-rw-rw-   0        0        0     1953 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimumc.py
+-rw-rw-rw-   0        0        0     1910 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Statistics.py
+-rw-rw-rw-   0        0        0     2031 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.982114 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/
+-rw-rw-rw-   0        0        0     2089 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/All.py
+-rw-rw-rw-   0        0        0     2730 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.984110 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.987100 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:18.992088 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/
+-rw-rw-rw-   0        0        0     2078 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:19.004055 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/
+-rw-rw-rw-   0        0        0     2216 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Average.py
+-rw-rw-rw-   0        0        0     2216 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Maximum.py
+-rw-rw-rw-   0        0        0     2216 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Minimum.py
+-rw-rw-rw-   0        0        0     2095 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Statistics.py
+-rw-rw-rw-   0        0        0     1795 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/__init__.py
+-rw-rw-rw-   0        0        0     1256 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/__init__.py
+-rw-rw-rw-   0        0        0     4325 2024-04-19 09:04:12.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/__init__.py
+-rw-rw-rw-   0        0        0     2005 2024-04-19 09:04:09.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:19.085836 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/
+-rw-rw-rw-   0        0        0      586 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4165 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1116 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1145 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9097 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5751 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3439 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2546 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5238 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    25419 2024-04-03 11:15:31.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3775 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4768 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    14213 2024-04-03 11:15:31.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Core.py
+-rw-rw-rw-   0        0        0     1386 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/GlobalData.py
+-rw-rw-rw-   0        0        0    60862 2024-04-03 11:15:31.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4785 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2225 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0    16156 2024-04-03 11:15:31.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3518 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4390 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0      387 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Properties.py
+-rw-rw-rw-   0        0        0     4289 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4745 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ScpiEnums.py
+-rw-rw-rw-   0        0        0    35525 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ScpiLogger.py
+-rw-rw-rw-   0        0        0     5098 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5856 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1114 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3608 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Types.py
+-rw-rw-rw-   0        0        0     5498 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5716 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    51976 2024-04-03 11:15:31.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7512 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0       29 2024-02-28 16:27:53.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/__init__.py
+-rw-rw-rw-   0        0        0    12844 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/RsCMPX_WcdmaMeas.py
+-rw-rw-rw-   0        0        0      952 2024-04-19 09:04:13.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-19 09:04:07.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/enums.py
+-rw-rw-rw-   0        0        0     5117 2024-04-19 09:02:57.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/repcap.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:04:17.203869 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/
+-rw-rw-rw-   0        0        0     2860 2024-04-19 09:04:16.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    59717 2024-04-19 09:04:16.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:04:16.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-19 09:04:16.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-19 09:04:16.000000 RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:04:19.088828 RsCMPX_WcdmaMeas-5.0.40/setup.cfg
+-rw-rw-rw-   0        0        0     1490 2024-04-19 09:04:14.000000 RsCMPX_WcdmaMeas-5.0.40/setup.py
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/PKG-INFO` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: RsCMPX_WcdmaMeas
-Version: 4.0.186
+Name: RsCMPX-WcdmaMeas
+Version: 5.0.40
 Summary: CMP180 WCDMA Measurement Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_WcdmaMeas
         ==================================
@@ -44,15 +44,18 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Fixed documentation
+        	Latest release notes summary: Update for FW 5.0.40
+        
+        	Version 5.0.40
+        		- Update for FW 5.0.40
         
         	Version 4.0.186
         		- Fixed documentation
         
         	Version 4.0.185
         		- First released version for FW 4.0.185
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/README.rst` & `RsCMPX_WcdmaMeas-5.0.40/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
 Examples: https://github.com/Rohde-Schwarz/Examples/
 
 
 Version history
 ----------------
 
-	Latest release notes summary: Fixed documentation
+	Latest release notes summary: Update for FW 5.0.40
+
+	Version 5.0.40
+		- Update for FW 5.0.40
 
 	Version 4.0.186
 		- Fixed documentation
 
 	Version 4.0.185
 		- First released version for FW 4.0.185
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/events.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/events.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/reliability.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/CustomFiles/utilities.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/CustomFiles/utilities.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/Band.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/Band.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/Scode.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/Scode.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Cell/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Amode.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Amode.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/CdThreshold.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/CdThreshold.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Dmode.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Dmode.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/DsFactor.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/DsFactor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/Relative.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/Relative.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Aclr/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 			from .Relative import RelativeCls
 			self._relative = RelativeCls(self._core, self._cmd_group)
 		return self._relative
 
 	def get_absolute(self) -> float or bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:ACLR:ABSolute \n
 		Snippet: value: float or bool = driver.configure.wcdmaMeas.multiEval.limit.aclr.get_absolute() \n
-		Defines an absolute upper limit for the ACLR. If the absolute upper limit is exceeded, relative limits are evaluated
+		It defines an absolute upper limit for the ACLR. If the absolute upper limit is exceeded, relative limits are evaluated
 		(method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Limit.Aclr.Relative.set) . \n
 			:return: limit_3_m_84: (float or boolean) No help available
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:ACLR:ABSolute?')
 		return Conversions.str_to_float_or_bool(response)
 
 	def set_absolute(self, limit_3_m_84: float or bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:ACLR:ABSolute \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.aclr.set_absolute(limit_3_m_84 = 1.0) \n
-		Defines an absolute upper limit for the ACLR. If the absolute upper limit is exceeded, relative limits are evaluated
+		It defines an absolute upper limit for the ACLR. If the absolute upper limit is exceeded, relative limits are evaluated
 		(method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Limit.Aclr.Relative.set) . \n
 			:param limit_3_m_84: (float or boolean) No help available
 		"""
 		param = Conversions.decimal_or_bool_value_to_str(limit_3_m_84)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:ACLR:ABSolute {param}')
 
 	def clone(self) -> 'AclrCls':
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Absolute.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Absolute.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("absolute", core, parent)
 
 	def set(self, limit_g_3_m_84: float or bool, limit_h_1_mhz: float or bool, limit_h_30_khz: float or bool, limit_hmode: enums.LimitHmode) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:EMASk:ABSolute \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.emask.absolute.set(limit_g_3_m_84 = 1.0, limit_h_1_mhz = 1.0, limit_h_30_khz = 1.0, limit_hmode = enums.LimitHmode.A) \n
 		Defines absolute limits for the spectrum emission curves. \n
-			:param limit_g_3_m_84: (float or boolean) Absolute limit line G referenced to a 3.84 MHz filter
-			:param limit_h_1_mhz: (float or boolean) Absolute limit line H referenced to a 1 MHz or 100 kHz filter, depending on the line H mode
-			:param limit_h_30_khz: (float or boolean) Absolute limit line H referenced to a 30 kHz filter
+			:param limit_g_3_m_84: (float or boolean) Absolute limit line G referenced to a 3.84 MHz filter.
+			:param limit_h_1_mhz: (float or boolean) Absolute limit line H is referenced to a 1 MHz or 100 kHz filter, depending on the line H mode.
+			:param limit_h_30_khz: (float or boolean) Absolute limit line H referenced to a 30 kHz filter.
 			:param limit_hmode: Line H mode
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('limit_g_3_m_84', limit_g_3_m_84, DataType.FloatExt), ArgSingle('limit_h_1_mhz', limit_h_1_mhz, DataType.FloatExt), ArgSingle('limit_h_30_khz', limit_h_30_khz, DataType.FloatExt), ArgSingle('limit_hmode', limit_hmode, DataType.Enum, enums.LimitHmode))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:EMASk:ABSolute {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class AbsoluteStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Limit_G_3_M_84: float or bool: Absolute limit line G referenced to a 3.84 MHz filter
-			- Limit_H_1_Mhz: float or bool: Absolute limit line H referenced to a 1 MHz or 100 kHz filter, depending on the line H mode
-			- Limit_H_30_Khz: float or bool: Absolute limit line H referenced to a 30 kHz filter
+			- Limit_G_3_M_84: float or bool: Absolute limit line G referenced to a 3.84 MHz filter.
+			- Limit_H_1_Mhz: float or bool: Absolute limit line H is referenced to a 1 MHz or 100 kHz filter, depending on the line H mode.
+			- Limit_H_30_Khz: float or bool: Absolute limit line H referenced to a 30 kHz filter.
 			- Limit_Hmode: enums.LimitHmode: Line H mode"""
 		__meta_args_list = [
 			ArgStruct.scalar_float_ext('Limit_G_3_M_84'),
 			ArgStruct.scalar_float_ext('Limit_H_1_Mhz'),
 			ArgStruct.scalar_float_ext('Limit_H_30_Khz'),
 			ArgStruct.scalar_enum('Limit_Hmode', enums.LimitHmode)]
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/Absolute.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/Absolute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/Dcarrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Emask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/EvMagnitude.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/EvMagnitude.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Merror.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Merror.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/EpStep.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/EpStep.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/Hsdpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/Hsdpcch.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
 	def set(self, enable: bool, dtx_to_nack: float, nack_to_cqi: float, cqi_to_dtx: float, test_case: enums.TestCase = None) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:PCONtrol:HSDPcch \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.pcontrol.hsdpcch.set(enable = False, dtx_to_nack = 1.0, nack_to_cqi = 1.0, cqi_to_dtx = 1.0, test_case = enums.TestCase.T0DB) \n
 		Defines nominal power steps for the HS-DPCCH limit set. Measurements at maximum UE power and below maximum UE power are
 		supported. Separate values can be defined for the boundaries DTX > (N) ACK, (N) ACK > CQI and CQI > DTX. Also the limit
 		check can be enabled or disabled. \n
-			:param enable: Disables | enables the limit check
+			:param enable: Disables | enables the limit check.
 			:param dtx_to_nack: No help available
 			:param nack_to_cqi: No help available
 			:param cqi_to_dtx: No help available
 			:param test_case: T0DB: measurement below maximum UE power with TPC command = 0 dB T1DB: measurement at maximum UE power with TPC command = 1 dB
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('dtx_to_nack', dtx_to_nack, DataType.Float), ArgSingle('nack_to_cqi', nack_to_cqi, DataType.Float), ArgSingle('cqi_to_dtx', cqi_to_dtx, DataType.Float), ArgSingle('test_case', test_case, DataType.Enum, enums.TestCase, is_optional=True))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:PCONtrol:HSDPcch {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class HsdpcchStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
+			- Enable: bool: Disables | enables the limit check.
 			- Dtx_To_Nack: float: No parameter help available
 			- Nack_To_Cqi: float: No parameter help available
 			- Cqi_To_Dtx: float: No parameter help available
 			- Test_Case: enums.TestCase: T0DB: measurement below maximum UE power with TPC command = 0 dB T1DB: measurement at maximum UE power with TPC command = 1 dB"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Dtx_To_Nack'),
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Pcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Perror.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Perror.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("perror", core, parent)
 
 	def set(self, rms: float or bool, peak: float or bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:PERRor \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.perror.set(rms = 1.0, peak = 1.0) \n
 		Defines symmetric limits for the RMS and peak values of the phase error. The limit check fails if the absolute value of
-		the measured phase error exceeds the specified values. \n
+		the measured phase error exceeds the specified value. \n
 			:param rms: (float or boolean) No help available
 			:param peak: (float or boolean) No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('rms', rms, DataType.FloatExt), ArgSingle('peak', peak, DataType.FloatExt))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:PERRor {param}'.rstrip())
 
 	# noinspection PyTypeChecker
@@ -40,10 +40,10 @@
 			self.Rms: float or bool = None
 			self.Peak: float or bool = None
 
 	def get(self) -> PerrorStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:PERRor \n
 		Snippet: value: PerrorStruct = driver.configure.wcdmaMeas.multiEval.limit.perror.get() \n
 		Defines symmetric limits for the RMS and peak values of the phase error. The limit check fails if the absolute value of
-		the measured phase error exceeds the specified values. \n
+		the measured phase error exceeds the specified value. \n
 			:return: structure: for return value, see the help for PerrorStruct structure arguments."""
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:PERRor?', self.__class__.PerrorStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Phd.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/Phd.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 		self._cmd_group = CommandsGroup("phd", core, parent)
 
 	def set(self, enable: bool, upper: float, dynamic: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:PHD \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.phd.set(enable = False, upper = 1.0, dynamic = 1.0) \n
 		Defines upper and dynamic limits for the phase discontinuity determined by full-slot measurements (signals without HSPA
 		channels) . \n
-			:param enable: Disables | enables the limit check
+			:param enable: Disables | enables the limit check.
 			:param upper: No help available
 			:param dynamic: No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('upper', upper, DataType.Float), ArgSingle('dynamic', dynamic, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:PHD {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class PhdStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
+			- Enable: bool: Disables | enables the limit check.
 			- Upper: float: No parameter help available
 			- Dynamic: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Upper'),
 			ArgStruct.scalar_float('Dynamic')]
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/PhsDpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/PhsDpcch.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
 	def set(self, enable: bool, measure_point_a: float, measure_point_b: float, dynamic: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:PHSDpcch \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.phsDpcch.set(enable = False, measure_point_a = 1.0, measure_point_b = 1.0, dynamic = 1.0) \n
 		Defines a dynamic limit for the phase discontinuity determined by half-slot measurements (signals with HS-DPCCH) .
 		The limit is checked at point A and point B. As the phase discontinuity is measured at half-slot boundaries (x.5, not x.
 		0) points A and B have to be set to half-slot positions. \n
-			:param enable: Disables | enables the limit check
+			:param enable: Disables | enables the limit check.
 			:param measure_point_a: No help available
 			:param measure_point_b: No help available
 			:param dynamic: No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('measure_point_a', measure_point_a, DataType.Float), ArgSingle('measure_point_b', measure_point_b, DataType.Float), ArgSingle('dynamic', dynamic, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:PHSDpcch {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class PhsDpcchStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
+			- Enable: bool: Disables | enables the limit check.
 			- Measure_Point_A: float: No parameter help available
 			- Measure_Point_B: float: No parameter help available
 			- Dynamic: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Measure_Point_A'),
 			ArgStruct.scalar_float('Measure_Point_B'),
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpcch.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("dpcch", core, parent)
 
 	def set(self, enable: bool, beta_factor: int, spreading_factor: int, carrier=repcap.Carrier.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:DPCCh \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.dpcch.set(enable = False, beta_factor = 1, spreading_factor = 1, carrier = repcap.Carrier.Default) \n
 		Specifies the presence of a DPCCH in the uplink signal and the beta factor and spreading factor of the channel. A query
-		returns also the nominal CDP and effective CDP resulting from these settings. \n
+		also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param enable: Channel disabled | enabled
 			:param beta_factor: No help available
 			:param spreading_factor: No help available
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('beta_factor', beta_factor, DataType.Integer), ArgSingle('spreading_factor', spreading_factor, DataType.Integer))
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
@@ -53,12 +53,12 @@
 			self.Nominal_Cdp: float = None
 			self.Effective_Cdp: float = None
 
 	def get(self, carrier=repcap.Carrier.Default) -> GetStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:DPCCh \n
 		Snippet: value: GetStruct = driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.dpcch.get(carrier = repcap.Carrier.Default) \n
 		Specifies the presence of a DPCCH in the uplink signal and the beta factor and spreading factor of the channel. A query
-		returns also the nominal CDP and effective CDP resulting from these settings. \n
+		also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier{carrier_cmd_val}:DPCCh?', self.__class__.GetStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpdch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Dpdch.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("dpdch", core, parent)
 
 	def set(self, enable: bool, beta_factor: int, spreading_factor: int, carrier=repcap.Carrier.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:DPDCh \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.dpdch.set(enable = False, beta_factor = 1, spreading_factor = 1, carrier = repcap.Carrier.Default) \n
 		Specifies the presence of a DPDCH in the uplink signal and the beta factor and spreading factor of the channel. A query
-		returns also the nominal CDP and effective CDP resulting from these settings. \n
+		also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param enable: Channel disabled | enabled
 			:param beta_factor: No help available
 			:param spreading_factor: No help available
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('beta_factor', beta_factor, DataType.Integer), ArgSingle('spreading_factor', spreading_factor, DataType.Integer))
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
@@ -53,12 +53,12 @@
 			self.Nominal_Cdp: float = None
 			self.Effective_Cdp: float = None
 
 	def get(self, carrier=repcap.Carrier.Default) -> GetStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:DPDCh \n
 		Snippet: value: GetStruct = driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.dpdch.get(carrier = repcap.Carrier.Default) \n
 		Specifies the presence of a DPDCH in the uplink signal and the beta factor and spreading factor of the channel. A query
-		returns also the nominal CDP and effective CDP resulting from these settings. \n
+		also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier{carrier_cmd_val}:DPDCh?', self.__class__.GetStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpcch.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("edpcch", core, parent)
 
 	def set(self, enable: bool, beta_factor: int, spreading_factor: int, carrier=repcap.Carrier.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:EDPCch \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.edpcch.set(enable = False, beta_factor = 1, spreading_factor = 1, carrier = repcap.Carrier.Default) \n
 		Specifies the presence of an E-DPCCH in the uplink signal and the beta factor and spreading factor of the channel.
-		A query returns also the nominal CDP and effective CDP resulting from these settings. \n
+		A query also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param enable: Channel disabled | enabled
 			:param beta_factor: No help available
 			:param spreading_factor: No help available
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('beta_factor', beta_factor, DataType.Integer), ArgSingle('spreading_factor', spreading_factor, DataType.Integer))
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
@@ -53,12 +53,12 @@
 			self.Nominal_Cdp: float = None
 			self.Effective_Cdp: float = None
 
 	def get(self, carrier=repcap.Carrier.Default) -> GetStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:EDPCch \n
 		Snippet: value: GetStruct = driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.edpcch.get(carrier = repcap.Carrier.Default) \n
 		Specifies the presence of an E-DPCCH in the uplink signal and the beta factor and spreading factor of the channel.
-		A query returns also the nominal CDP and effective CDP resulting from these settings. \n
+		A query also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier{carrier_cmd_val}:EDPCch?', self.__class__.GetStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpdch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Edpdch.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 		# noinspection PyTypeChecker
 		return self._cmd_group.get_repcap_enum_value()
 
 	def set(self, enable: bool, beta_factor: int, spreading_factor: int, carrier=repcap.Carrier.Default, edpdChannel=repcap.EdpdChannel.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:EDPDch<nr> \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.edpdch.set(enable = False, beta_factor = 1, spreading_factor = 1, carrier = repcap.Carrier.Default, edpdChannel = repcap.EdpdChannel.Default) \n
 		Specifies the presence of a selected E-DPDCH (1 to 4) in the uplink signal and the beta factor and spreading factor of
-		the channel. A query returns also the nominal CDP and effective CDP resulting from these settings. \n
+		the channel. A query also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param enable: Channel disabled | enabled
 			:param beta_factor: No help available
 			:param spreading_factor: No help available
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:param edpdChannel: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Edpdch')
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('beta_factor', beta_factor, DataType.Integer), ArgSingle('spreading_factor', spreading_factor, DataType.Integer))
@@ -69,15 +69,15 @@
 			self.Nominal_Cdp: float = None
 			self.Effective_Cdp: float = None
 
 	def get(self, carrier=repcap.Carrier.Default, edpdChannel=repcap.EdpdChannel.Default) -> GetStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:EDPDch<nr> \n
 		Snippet: value: GetStruct = driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.edpdch.get(carrier = repcap.Carrier.Default, edpdChannel = repcap.EdpdChannel.Default) \n
 		Specifies the presence of a selected E-DPDCH (1 to 4) in the uplink signal and the beta factor and spreading factor of
-		the channel. A query returns also the nominal CDP and effective CDP resulting from these settings. \n
+		the channel. A query also returns the nominal CDP and effective CDP resulting from these settings. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:param edpdChannel: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Edpdch')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		edpdChannel_cmd_val = self._cmd_group.get_repcap_cmd_value(edpdChannel, repcap.EdpdChannel)
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier{carrier_cmd_val}:EDPDch{edpdChannel_cmd_val}?', self.__class__.GetStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/Config.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/Config.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/Hsdpcch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 			self._config = ConfigCls(self._core, self._cmd_group)
 		return self._config
 
 	def set(self, enable: bool, beta_factor: int, spreading_factor: int, carrier=repcap.Carrier.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:HSDPcch \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.hsdpcch.set(enable = False, beta_factor = 1, spreading_factor = 1, carrier = repcap.Carrier.Default) \n
 		Specifies the presence of an HS-DPCCH in the uplink signal and the beta factor and spreading factor of the channel.
-		A query returns also the nominal CDP and effective CDP resulting from these settings. For the HS-DPCCH three sets of beta
+		A query also returns the nominal CDP and effective CDP resulting from these settings. For the HS-DPCCH three sets of beta
 		factor and spreading factor can be configured, depending on whether it transports an ACK, NACK or CQI. This command
 		configures/returns the values related to the currently active set. For selection of the active set, see method
 		RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Limit.RcdError.Eecdp.Carrier.Hsdpcch.Config.set. \n
 			:param enable: Channel disabled | enabled
 			:param beta_factor: No help available
 			:param spreading_factor: No help available
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
@@ -64,15 +64,15 @@
 			self.Nominal_Cdp: float = None
 			self.Effective_Cdp: float = None
 
 	def get(self, carrier=repcap.Carrier.Default) -> GetStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier<carrier>:HSDPcch \n
 		Snippet: value: GetStruct = driver.configure.wcdmaMeas.multiEval.limit.rcdError.eecdp.carrier.hsdpcch.get(carrier = repcap.Carrier.Default) \n
 		Specifies the presence of an HS-DPCCH in the uplink signal and the beta factor and spreading factor of the channel.
-		A query returns also the nominal CDP and effective CDP resulting from these settings. For the HS-DPCCH three sets of beta
+		A query also returns the nominal CDP and effective CDP resulting from these settings. For the HS-DPCCH three sets of beta
 		factor and spreading factor can be configured, depending on whether it transports an ACK, NACK or CQI. This command
 		configures/returns the values related to the currently active set. For selection of the active set, see method
 		RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Limit.RcdError.Eecdp.Carrier.Hsdpcch.Config.set. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for GetStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:RCDerror:EECDp:CARRier{carrier_cmd_val}:HSDPcch?', self.__class__.GetStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/Eecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/RcdError/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 			self.Threshold_4_Pam_2: float = None
 			self.Limit_4_Pam_1: float = None
 			self.Limit_4_Pam_2: float = None
 
 	def get_ecdp(self) -> EcdpStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:ECDP \n
 		Snippet: value: EcdpStruct = driver.configure.wcdmaMeas.multiEval.limit.rcdError.get_ecdp() \n
-		Defines upper limits for the relative CDE (RCDE) of BPSK and 4PAM modulated channels. For each modulation type, two
+		Defines upper limits for the relative CDE (RCDE) of BPSK and 4PAM modulated channels. For each modulation format, two
 		requirements are defined. \n
 			:return: structure: for return value, see the help for EcdpStruct structure arguments.
 		"""
 		return self._core.io.query_struct('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:RCDerror:ECDP?', self.__class__.EcdpStruct())
 
 	def set_ecdp(self, value: EcdpStruct) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIMit:RCDerror:ECDP \n
@@ -70,15 +70,15 @@
 		structure.Limit_Bpsk_1: float = 1.0 \n
 		structure.Limit_Bpks_2: float = 1.0 \n
 		structure.Threshold_4_Pam_1: float = 1.0 \n
 		structure.Threshold_4_Pam_2: float = 1.0 \n
 		structure.Limit_4_Pam_1: float = 1.0 \n
 		structure.Limit_4_Pam_2: float = 1.0 \n
 		driver.configure.wcdmaMeas.multiEval.limit.rcdError.set_ecdp(value = structure) \n
-		Defines upper limits for the relative CDE (RCDE) of BPSK and 4PAM modulated channels. For each modulation type, two
+		Defines upper limits for the relative CDE (RCDE) of BPSK and 4PAM modulated channels. For each modulation format, two
 		requirements are defined. \n
 			:param value: see the help for EcdpStruct structure arguments.
 		"""
 		self._core.io.write_struct('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIMit:RCDerror:ECDP', value)
 
 	def clone(self) -> 'RcdErrorCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Limit/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/CdPower.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/CdPower.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIST:SEGMent<nr>:CDPower \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.listPy.segment.cdPower.set(mod_statistics = 1, enable_cdp = False, enable_cde = False, enable_pcde = False, segment = repcap.Segment.Default) \n
 		Defines the statistical length for the AVERage, MINimum, MAXimum and SDEViation calculation and enables the calculation
 		of the different code domain results in segment no. <no>; see 'Multi-evaluation list mode'. The statistical length for
 		CDP, CDE, PCDE and modulation results is identical (see also method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.ListPy.
 		Segment.Modulation.set) . \n
 			:param mod_statistics: The statistical length is limited by the length of the segment (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.ListPy.Segment.Setup.set) .
-			:param enable_cdp: OFF: Disable measurement ON: Enable measurement of code domain power
-			:param enable_cde: Disable or enable measurement of code domain error
-			:param enable_pcde: Disable or enable measurement of peak code domain error
+			:param enable_cdp: OFF: Disable measurement ON: Enable measurement of code domain power.
+			:param enable_cde: Disable or enable measurement of code domain error.
+			:param enable_pcde: Disable or enable measurement of peak code domain error.
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('mod_statistics', mod_statistics, DataType.Integer), ArgSingle('enable_cdp', enable_cdp, DataType.Boolean), ArgSingle('enable_cde', enable_cde, DataType.Boolean), ArgSingle('enable_pcde', enable_pcde, DataType.Boolean, None, is_optional=True))
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:CDPower {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class CdPowerStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Mod_Statistics: int: The statistical length is limited by the length of the segment (see [CMDLINKRESOLVED Configure.WcdmaMeas.MultiEval.ListPy.Segment.Setup#set CMDLINKRESOLVED]) .
-			- Enable_Cdp: bool: OFF: Disable measurement ON: Enable measurement of code domain power
-			- Enable_Cde: bool: Disable or enable measurement of code domain error
-			- Enable_Pcde: bool: Disable or enable measurement of peak code domain error"""
+			- Enable_Cdp: bool: OFF: Disable measurement ON: Enable measurement of code domain power.
+			- Enable_Cde: bool: Disable or enable measurement of code domain error.
+			- Enable_Pcde: bool: Disable or enable measurement of peak code domain error."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Mod_Statistics'),
 			ArgStruct.scalar_bool('Enable_Cdp'),
 			ArgStruct.scalar_bool('Enable_Cde'),
 			ArgStruct.scalar_bool('Enable_Pcde')]
 
 		def __init__(self):
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Cidx.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Cidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("cidx", core, parent)
 
 	def set(self, connection_index: int, segment=repcap.Segment.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent<nr>:CIDX \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.listPy.segment.cidx.set(connection_index = 1, segment = repcap.Segment.Default) \n
-		Selects the RF connection index for segment <no>. For definition of the connection indices, see ROUTe:WCDMa:MEAS<i>:SPATh. \n
+		Selects the RF connection index for segment <no>. For a definition of the connection indices,
+		see ROUTe:WCDMa:MEAS<i>:SPATh. \n
 			:param connection_index: Index of the connection to be used for the segment.
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 		"""
 		param = Conversions.decimal_value_to_str(connection_index)
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:CIDX {param}')
 
 	def get(self, segment=repcap.Segment.Default) -> int:
 		"""SCPI: CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent<nr>:CIDX \n
 		Snippet: value: int = driver.configure.wcdmaMeas.multiEval.listPy.segment.cidx.get(segment = repcap.Segment.Default) \n
-		Selects the RF connection index for segment <no>. For definition of the connection indices, see ROUTe:WCDMa:MEAS<i>:SPATh. \n
+		Selects the RF connection index for segment <no>. For a definition of the connection indices,
+		see ROUTe:WCDMa:MEAS<i>:SPATh. \n
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 			:return: connection_index: Index of the connection to be used for the segment."""
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		response = self._core.io.query_str(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:CIDX?')
 		return Conversions.str_to_int(response)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Modulation.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Modulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("modulation", core, parent)
 
 	# noinspection PyTypeChecker
 	class ModulationStruct(StructBase):
 		"""Structure for setting input parameters. Fields: \n
 			- Mod_Statistics: int: The statistical length is limited by the length of the segment (see [CMDLINKRESOLVED Configure.WcdmaMeas.MultiEval.ListPy.Segment.Setup#set CMDLINKRESOLVED]) .
-			- Enable_Ue_Power: bool: OFF: Disable measurement ON: Enable measurement of UE power
-			- Enable_Evm: bool: Disable or enable measurement of EVM
-			- Enable_Mag_Error: bool: Disable or enable measurement of magnitude error
-			- Enable_Phase_Err: bool: Disable or enable measurement of phase error
-			- Enable_Freq_Error: bool: Disable or enable measurement of frequency error
-			- Enable_Iq: bool: Disable or enable measurement of I/Q origin offset and imbalance"""
+			- Enable_Ue_Power: bool: OFF: Disable measurement. ON: Enable measurement of UE power.
+			- Enable_Evm: bool: Disable or enable measurement of EVM.
+			- Enable_Mag_Error: bool: Disable or enable measurement of magnitude error.
+			- Enable_Phase_Err: bool: Disable or enable measurement of phase error.
+			- Enable_Freq_Error: bool: Disable or enable measurement of frequency error.
+			- Enable_Iq: bool: Disable or enable measurement of I/Q origin offset and imbalance."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Mod_Statistics'),
 			ArgStruct.scalar_bool('Enable_Ue_Power'),
 			ArgStruct.scalar_bool('Enable_Evm'),
 			ArgStruct.scalar_bool('Enable_Mag_Error'),
 			ArgStruct.scalar_bool('Enable_Phase_Err'),
 			ArgStruct.scalar_bool('Enable_Freq_Error'),
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Phd.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Phd.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Setup.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,28 @@
 
 	def set(self, segment_length: int, level: float, frequency: float, retrigger: enums.Retrigger = None, segment=repcap.Segment.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIST:SEGMent<nr>:SETup \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.listPy.segment.setup.set(segment_length = 1, level = 1.0, frequency = 1.0, retrigger = enums.Retrigger.IFPower, segment = repcap.Segment.Default) \n
 		Defines the length and analyzer settings of a selected segment. In general, this command must be sent for all segments
 		measured. \n
 			:param segment_length: Number of measured timeslots in the segment. The sum of the length of all active segments must not exceed 6000. Ignoring this limit results in NCAPs for the remaining slots. The statistical length for result calculation covers at most the first 1000 slots of a segment. The sum of the length of all segments (active plus inactive) must not exceed 12000. 'Inactive' means that no measurement at all is enabled for the segment.
-			:param level: Expected nominal power in the segment. The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			:param level: Expected nominal power in the segment. The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 			:param frequency: No help available
 			:param retrigger: Specifies whether a trigger event is required for the segment or not. The setting is ignored for the first segment of a measurement and for trigger mode ONCE (see method RsCMPX_WcdmaMeas.Trigger.WcdmaMeas.MultiEval.ListPy.mode) . OFF: measure the segment without retrigger ON: trigger event required, trigger source configured via method RsCMPX_WcdmaMeas.Trigger.WcdmaMeas.MultiEval.source IFPower: trigger event required, IF Power trigger IFPSync: trigger event required, IF Power (Sync) trigger
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('segment_length', segment_length, DataType.Integer), ArgSingle('level', level, DataType.Float), ArgSingle('frequency', frequency, DataType.Float), ArgSingle('retrigger', retrigger, DataType.Enum, enums.Retrigger, is_optional=True))
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:SETup {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class SetupStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Segment_Length: int: Number of measured timeslots in the segment. The sum of the length of all active segments must not exceed 6000. Ignoring this limit results in NCAPs for the remaining slots. The statistical length for result calculation covers at most the first 1000 slots of a segment. The sum of the length of all segments (active plus inactive) must not exceed 12000. 'Inactive' means that no measurement at all is enabled for the segment.
-			- Level: float: Expected nominal power in the segment. The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			- Level: float: Expected nominal power in the segment. The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 			- Frequency: float: No parameter help available
 			- Retrigger: enums.Retrigger: Specifies whether a trigger event is required for the segment or not. The setting is ignored for the first segment of a measurement and for trigger mode ONCE (see [CMDLINKRESOLVED Trigger.WcdmaMeas.MultiEval.ListPy#Mode CMDLINKRESOLVED]) . OFF: measure the segment without retrigger ON: trigger event required, trigger source configured via [CMDLINKRESOLVED Trigger.WcdmaMeas.MultiEval#Source CMDLINKRESOLVED] IFPower: trigger event required, IF Power trigger IFPSync: trigger event required, IF Power (Sync) trigger"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Segment_Length'),
 			ArgStruct.scalar_float('Level'),
 			ArgStruct.scalar_float('Frequency'),
 			ArgStruct.scalar_enum('Retrigger', enums.Retrigger)]
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/Connector.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/SingleCmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 
 	def set(self, spec_statistics: int, enable_aclr: bool, enable_emask: bool, enable_obw: bool, segment=repcap.Segment.Default) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:LIST:SEGMent<nr>:SPECtrum \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.listPy.segment.spectrum.set(spec_statistics = 1, enable_aclr = False, enable_emask = False, enable_obw = False, segment = repcap.Segment.Default) \n
 		Defines the statistical length for the AVERage and MAXimum calculation and enables the calculation of the different
 		spectrum results in segment no. <no>; see 'Multi-evaluation list mode'. \n
 			:param spec_statistics: The statistical length is limited by the length of the segment (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.ListPy.Segment.Setup.set) .
-			:param enable_aclr: OFF: Disable measurement ON: Enable measurement of ACLR
-			:param enable_emask: Disable or enable measurement of spectrum emission mask
-			:param enable_obw: Disable or enable measurement of occupied bandwidth
+			:param enable_aclr: OFF: Disable measurement. ON: Enable measurement of ACLR.
+			:param enable_emask: Disable or enable measurement of spectrum emission mask.
+			:param enable_obw: Disable or enable measurement of occupied bandwidth.
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('spec_statistics', spec_statistics, DataType.Integer), ArgSingle('enable_aclr', enable_aclr, DataType.Boolean), ArgSingle('enable_emask', enable_emask, DataType.Boolean), ArgSingle('enable_obw', enable_obw, DataType.Boolean))
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:SPECtrum {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class SpectrumStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Spec_Statistics: int: The statistical length is limited by the length of the segment (see [CMDLINKRESOLVED Configure.WcdmaMeas.MultiEval.ListPy.Segment.Setup#set CMDLINKRESOLVED]) .
-			- Enable_Aclr: bool: OFF: Disable measurement ON: Enable measurement of ACLR
-			- Enable_Emask: bool: Disable or enable measurement of spectrum emission mask
-			- Enable_Obw: bool: Disable or enable measurement of occupied bandwidth"""
+			- Enable_Aclr: bool: OFF: Disable measurement. ON: Enable measurement of ACLR.
+			- Enable_Emask: bool: Disable or enable measurement of spectrum emission mask.
+			- Enable_Obw: bool: Disable or enable measurement of occupied bandwidth."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Spec_Statistics'),
 			ArgStruct.scalar_bool('Enable_Aclr'),
 			ArgStruct.scalar_bool('Enable_Emask'),
 			ArgStruct.scalar_bool('Enable_Obw')]
 
 		def __init__(self):
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/UePower.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/UePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/SingleCmw.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/SingleCmw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Mperiod.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Mperiod.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/Chip.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/Chip.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CHIP:PERRor \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.chip.set_perror(enable_ph_err_chip = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_ph_err_chip: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_ph_err_chip: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_ph_err_chip)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:CHIP:PERRor {param}')
 
 	def get_merror(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CHIP:MERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.chip.get_merror() \n
@@ -54,15 +54,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CHIP:MERRor \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.chip.set_merror(enable_merr_chip = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_merr_chip: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_merr_chip: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_merr_chip)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:CHIP:MERRor {param}')
 
 	def get_evm(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CHIP:EVM \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.chip.get_evm() \n
@@ -80,11 +80,11 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CHIP:EVM \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.chip.set_evm(enable_evm_chip = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_evm_chip: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_evm_chip: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_evm_chip)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:CHIP:EVM {param}')
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Result/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:RCDerror \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_rcd_error(enable_rcde = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_rcde: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_rcde: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_rcde)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:RCDerror {param}')
 
 	def get_iq(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:IQ \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_iq() \n
@@ -82,15 +82,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:IQ \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_iq(enable_iq = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_iq: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_iq: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_iq)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:IQ {param}')
 
 	def get_ber(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:BER \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_ber() \n
@@ -108,15 +108,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:BER \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_ber(enable_ber = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_ber: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_ber: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_ber)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:BER {param}')
 
 	def get_psteps(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:PSTeps \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_psteps() \n
@@ -134,15 +134,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:PSTeps \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_psteps(enable_pow_steps = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_pow_steps: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_pow_steps: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_pow_steps)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:PSTeps {param}')
 
 	def get_phd(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:PHD \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_phd() \n
@@ -160,15 +160,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:PHD \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_phd(enable_phase_disc = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_phase_disc: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_phase_disc: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_phase_disc)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:PHD {param}')
 
 	def get_freq_error(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:FERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_freq_error() \n
@@ -186,15 +186,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:FERRor \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_freq_error(enable_freq_error = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_freq_error: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_freq_error: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_freq_error)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:FERRor {param}')
 
 	def get_ue_power(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:UEPower \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_ue_power() \n
@@ -212,23 +212,23 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:UEPower \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_ue_power(enable_ue_power = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_ue_power: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_ue_power: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_ue_power)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:UEPower {param}')
 
 	# noinspection PyTypeChecker
 	class AllStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
 		"""Structure for setting input parameters. Contains optional set arguments. Fields: \n
-			- Enable_Evm: bool: Error vector magnitude OFF: Do not evaluate results ON: Evaluate results
+			- Enable_Evm: bool: Error vector magnitude OFF: Do not evaluate results. ON: Evaluate results
 			- Enable_Mag_Error: bool: Magnitude error
 			- Enable_Phase_Err: bool: Phase error
 			- Enable_Aclr: bool: Adjacent channel leakage power ratio
 			- Enable_Emask: bool: Spectrum emission mask
 			- Enable_Cd_Monitor: bool: Code domain monitor
 			- Enable_Cdp: bool: Code domain power
 			- Enable_Cde: bool: Code domain error
@@ -342,15 +342,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CDERror \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_cd_error(enable_cde = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_cde: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_cde: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_cde)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:CDERror {param}')
 
 	def get_cd_power(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CDPower \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_cd_power() \n
@@ -368,15 +368,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CDPower \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_cd_power(enable_cdp = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_cdp: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_cdp: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_cdp)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:CDPower {param}')
 
 	def get_cdp_monitor(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CDPMonitor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_cdp_monitor() \n
@@ -394,15 +394,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:CDPMonitor \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_cdp_monitor(enable_cd_monitor = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_cd_monitor: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_cd_monitor: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_cd_monitor)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:CDPMonitor {param}')
 
 	def get_emask(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:EMASk \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_emask() \n
@@ -420,15 +420,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:EMASk \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_emask(enable_emask = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_emask: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_emask: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_emask)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:EMASk {param}')
 
 	def get_aclr(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:ACLR \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_aclr() \n
@@ -446,15 +446,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:ACLR \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_aclr(enable_aclr = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_aclr: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_aclr: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_aclr)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:ACLR {param}')
 
 	def get_perror(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:PERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_perror() \n
@@ -472,15 +472,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:PERRor \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_perror(enable_phase_err = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_phase_err: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_phase_err: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_phase_err)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:PERRor {param}')
 
 	def get_ev_magnitude(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:EVMagnitude \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_ev_magnitude() \n
@@ -498,15 +498,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:EVMagnitude \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_ev_magnitude(enable_evm = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_evm: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_evm: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_evm)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:EVMagnitude {param}')
 
 	def get_merror(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:MERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.result.get_merror() \n
@@ -524,15 +524,15 @@
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:RESult:MERRor \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.result.set_merror(enable_mag_error = False) \n
 		Enables or disables the evaluation of results of the multi-evaluation measurement identified by the last command
 		mnemonics: error vector magnitude (EVM) , magnitude error, phase error, adjacent channel leakage power ratio, spectrum
 		emission mask, code domain monitor, code domain power, code domain error (CDE) , EVM vs chip, magnitude error vs chip,
 		phase error vs chip, UE power, frequency error, phase discontinuity, power steps, bit error rate, I/Q constellation, and
 		relative CDE results. \n
-			:param enable_mag_error: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_mag_error: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_mag_error)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:RESult:MERRor {param}')
 
 	def clone(self) -> 'ResultCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Rotation.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Rotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("rotation", core, parent)
 
 	def get_modulation(self) -> int:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:ROTation:MODulation \n
 		Snippet: value: int = driver.configure.wcdmaMeas.multiEval.rotation.get_modulation() \n
 		Defines the initial phase reference (φ=0) for I/Q constellation diagrams of QPSK signals. \n
-			:return: rotation: The entered value is rounded to 0 deg or 45 deg. 0 deg: constellation points on I- and Q-axes 45 deg: constellation points on angle bisectors between I- and Q-axes
+			:return: rotation: The entered value is rounded to 0 deg or 45 deg. 0 deg: constellation points on the I- and Q-axes 45 deg: constellation points on angle bisectors between the I- and Q-axes
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:ROTation:MODulation?')
 		return Conversions.str_to_int(response)
 
 	def set_modulation(self, rotation: int) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:ROTation:MODulation \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.rotation.set_modulation(rotation = 1) \n
 		Defines the initial phase reference (φ=0) for I/Q constellation diagrams of QPSK signals. \n
-			:param rotation: The entered value is rounded to 0 deg or 45 deg. 0 deg: constellation points on I- and Q-axes 45 deg: constellation points on angle bisectors between I- and Q-axes
+			:param rotation: The entered value is rounded to 0 deg or 45 deg. 0 deg: constellation points on the I- and Q-axes 45 deg: constellation points on angle bisectors between the I- and Q-axes
 		"""
 		param = Conversions.decimal_value_to_str(rotation)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:ROTation:MODulation {param}')
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Scount.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Scount.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Sscalar.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/Sscalar.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("sscalar", core, parent)
 
 	def get_modulation(self) -> float:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:SSCalar:MODulation \n
 		Snippet: value: float = driver.configure.wcdmaMeas.multiEval.sscalar.get_modulation() \n
-		Selects a particular slot or half-slot within the measurement length where the R&S CMP180 evaluates the statistical
+		Selects a particular slot or half-slot within the measurement length where the CMP180 evaluates the statistical
 		measurement results for multislot measurements. The slot number must be smaller than the number of measured slots (see
 		method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 			:return: slot_number: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:SSCalar:MODulation?')
 		return Conversions.str_to_float(response)
 
 	def set_modulation(self, slot_number: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:SSCalar:MODulation \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.sscalar.set_modulation(slot_number = 1.0) \n
-		Selects a particular slot or half-slot within the measurement length where the R&S CMP180 evaluates the statistical
+		Selects a particular slot or half-slot within the measurement length where the CMP180 evaluates the statistical
 		measurement results for multislot measurements. The slot number must be smaller than the number of measured slots (see
 		method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 			:param slot_number: No help available
 		"""
 		param = Conversions.decimal_value_to_str(slot_number)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:SSCalar:MODulation {param}')
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/MultiEval/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,67 +147,67 @@
 		"""
 		param = Conversions.decimal_value_to_str(slot_count)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:MSCount {param}')
 
 	def get_pslot(self) -> int:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:PSLot \n
 		Snippet: value: int = driver.configure.wcdmaMeas.multiEval.get_pslot() \n
-		Selects the slot where the R&S CMP180 calculates the results of single slot measurements: ACLR, emission mask, EVM vs
-		chip, CD monitor. The number of the preselected slot must be smaller than the number of measured slots (method
-		RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
+		Selects the slot where the CMP180 calculates the results of single slot measurements: ACLR, emission mask, EVM vs chip,
+		CD monitor. The number of the preselected slot must be smaller than the number of measured slots (method RsCMPX_WcdmaMeas.
+		Configure.WcdmaMeas.MultiEval.msCount) . \n
 			:return: slot_number: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:PSLot?')
 		return Conversions.str_to_int(response)
 
 	def set_pslot(self, slot_number: int) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:PSLot \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.set_pslot(slot_number = 1) \n
-		Selects the slot where the R&S CMP180 calculates the results of single slot measurements: ACLR, emission mask, EVM vs
-		chip, CD monitor. The number of the preselected slot must be smaller than the number of measured slots (method
-		RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
+		Selects the slot where the CMP180 calculates the results of single slot measurements: ACLR, emission mask, EVM vs chip,
+		CD monitor. The number of the preselected slot must be smaller than the number of measured slots (method RsCMPX_WcdmaMeas.
+		Configure.WcdmaMeas.MultiEval.msCount) . \n
 			:param slot_number: No help available
 		"""
 		param = Conversions.decimal_value_to_str(slot_number)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:PSLot {param}')
 
 	# noinspection PyTypeChecker
 	def get_synch(self) -> enums.SlotNumber:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:SYNCh \n
 		Snippet: value: enums.SlotNumber = driver.configure.wcdmaMeas.multiEval.get_synch() \n
-		Selects a slot number within the UL WCDMA frames (0 to 14) that the R&S CMP180 displays as the first slot in the
-		measurement interval. \n
+		Selects a slot number within the UL WCDMA frames (0 to 14) that the CMP180 displays as the first slot in the measurement
+		interval. \n
 			:return: slot_number: ANY: No frame synchronization SL0 ... SL14: First slot = slot 0 ... slot 14
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:SYNCh?')
 		return Conversions.str_to_scalar_enum(response, enums.SlotNumber)
 
 	def set_synch(self, slot_number: enums.SlotNumber) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:SYNCh \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.set_synch(slot_number = enums.SlotNumber.ANY) \n
-		Selects a slot number within the UL WCDMA frames (0 to 14) that the R&S CMP180 displays as the first slot in the
-		measurement interval. \n
+		Selects a slot number within the UL WCDMA frames (0 to 14) that the CMP180 displays as the first slot in the measurement
+		interval. \n
 			:param slot_number: ANY: No frame synchronization SL0 ... SL14: First slot = slot 0 ... slot 14
 		"""
 		param = Conversions.enum_scalar_to_str(slot_number, enums.SlotNumber)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:SYNCh {param}')
 
 	def get_mo_exception(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:MOEXception \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.multiEval.get_mo_exception() \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:return: meas_on_exception: OFF: Faulty results are rejected. ON: Results are never rejected.
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:MEValuation:MOEXception?')
 		return Conversions.str_to_bool(response)
 
 	def set_mo_exception(self, meas_on_exception: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:MEValuation:MOEXception \n
 		Snippet: driver.configure.wcdmaMeas.multiEval.set_mo_exception(meas_on_exception = False) \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:param meas_on_exception: OFF: Faulty results are rejected. ON: Results are never rejected.
 		"""
 		param = Conversions.bool_to_str(meas_on_exception)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:MEValuation:MOEXception {param}')
 
 	# noinspection PyTypeChecker
 	def get_scondition(self) -> enums.StopCondition:
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OlpControl.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OlpControl.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/Limit.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/Limit.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/OoSync/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/EvMagnitude.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/EvMagnitude.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Merror.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Merror.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/UserDefined.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/UserDefined.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/MaxPower/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PCONtrol:MAXPower:URPClass {param}')
 
 	def set(self, enable: bool, active_limit: enums.ActiveLimit) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:LIMit:PCONtrol:MAXPower \n
 		Snippet: driver.configure.wcdmaMeas.prach.limit.pcontrol.maxPower.set(enable = False, active_limit = enums.ActiveLimit.PC1) \n
 		Enables or disables the check of the maximum output power limits and selects the set of limit settings to be used. \n
-			:param enable: Disables | enables the limit check
+			:param enable: Disables | enables the limit check.
 			:param active_limit: To use the limits defined by 3GPP, select the power class of the UE (PC1 to PC4 = power class 1, 2, 3, 3bis, 4) . For user-defined limit values, select USER and define the limits via method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.Limit.Pcontrol.MaxPower.UserDefined.set.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('active_limit', active_limit, DataType.Enum, enums.ActiveLimit))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PCONtrol:MAXPower {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class MaxPowerStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
+			- Enable: bool: Disables | enables the limit check.
 			- Active_Limit: enums.ActiveLimit: To use the limits defined by 3GPP, select the power class of the UE (PC1 to PC4 = power class 1, 2, 3, 3bis, 4) . For user-defined limit values, select USER and define the limits via [CMDLINKRESOLVED Configure.WcdmaMeas.Prach.Limit.Pcontrol.MaxPower.UserDefined#set CMDLINKRESOLVED]."""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_enum('Active_Limit', enums.ActiveLimit)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/OlPower.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/OlPower.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("olPower", core, parent)
 
 	def set(self, enable: bool, init_preamble_pwr: float, olp_limit: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:LIMit:PCONtrol:OLPower \n
 		Snippet: driver.configure.wcdmaMeas.prach.limit.pcontrol.olPower.set(enable = False, init_preamble_pwr = 1.0, olp_limit = 1.0) \n
 		Enables or disables the check of the open loop power limits and specifies these limits. \n
-			:param enable: Disables | enables the limit check
+			:param enable: Disables | enables the limit check.
 			:param init_preamble_pwr: Initial preamble power
-			:param olp_limit: Open loop power tolerance value
+			:param olp_limit: Open loop power tolerance value.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('init_preamble_pwr', init_preamble_pwr, DataType.Float), ArgSingle('olp_limit', olp_limit, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PCONtrol:OLPower {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class OlPowerStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
+			- Enable: bool: Disables | enables the limit check.
 			- Init_Preamble_Pwr: float: Initial preamble power
-			- Olp_Limit: float: Open loop power tolerance value"""
+			- Olp_Limit: float: Open loop power tolerance value."""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Init_Preamble_Pwr'),
 			ArgStruct.scalar_float('Olp_Limit')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/Pstep.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/Pstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("pstep", core, parent)
 
 	def set(self, enable: bool, preamble_pwr_step: float, pwr_step_limit: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:LIMit:PCONtrol:PSTep \n
 		Snippet: driver.configure.wcdmaMeas.prach.limit.pcontrol.pstep.set(enable = False, preamble_pwr_step = 1.0, pwr_step_limit = 1.0) \n
 		Enables or disables the check of the preamble power step limits and specifies these limits. \n
-			:param enable: Disables | enables the limit check
-			:param preamble_pwr_step: Expected preamble power step size
-			:param pwr_step_limit: Preamble power step tolerance value
+			:param enable: Disables | enables the limit check.
+			:param preamble_pwr_step: Expected preamble power step size.
+			:param pwr_step_limit: Preamble power step tolerance value.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('preamble_pwr_step', preamble_pwr_step, DataType.Float), ArgSingle('pwr_step_limit', pwr_step_limit, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PCONtrol:PSTep {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class PstepStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
-			- Preamble_Pwr_Step: float: Expected preamble power step size
-			- Pwr_Step_Limit: float: Preamble power step tolerance value"""
+			- Enable: bool: Disables | enables the limit check.
+			- Preamble_Pwr_Step: float: Expected preamble power step size.
+			- Pwr_Step_Limit: float: Preamble power step tolerance value."""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Preamble_Pwr_Step'),
 			ArgStruct.scalar_float('Pwr_Step_Limit')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Pcontrol/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 			from .OlPower import OlPowerCls
 			self._olPower = OlPowerCls(self._core, self._cmd_group)
 		return self._olPower
 
 	def get_off_power(self) -> float or bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:LIMit:PCONtrol:OFFPower \n
 		Snippet: value: float or bool = driver.configure.wcdmaMeas.prach.limit.pcontrol.get_off_power() \n
-		Defines an upper OFF power limit. Also enables or disables the limit check. \n
+		Defines an upper OFF power limit. It also enables or disables the limit check. \n
 			:return: limit: (float or boolean) No help available
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PCONtrol:OFFPower?')
 		return Conversions.str_to_float_or_bool(response)
 
 	def set_off_power(self, limit: float or bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:LIMit:PCONtrol:OFFPower \n
 		Snippet: driver.configure.wcdmaMeas.prach.limit.pcontrol.set_off_power(limit = 1.0) \n
-		Defines an upper OFF power limit. Also enables or disables the limit check. \n
+		Defines an upper OFF power limit. It also enables or disables the limit check. \n
 			:param limit: (float or boolean) No help available
 		"""
 		param = Conversions.decimal_or_bool_value_to_str(limit)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PCONtrol:OFFPower {param}')
 
 	def clone(self) -> 'PcontrolCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Perror.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/Perror.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("perror", core, parent)
 
 	def set(self, rms: float or bool, peak: float or bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:LIMit:PERRor \n
 		Snippet: driver.configure.wcdmaMeas.prach.limit.perror.set(rms = 1.0, peak = 1.0) \n
 		Defines symmetric limits for the RMS and peak values of the phase error. The limit check fails the UE if the absolute
-		value of the measured phase error exceeds the specified values. \n
+		value of the measured phase error exceeds the specified value. \n
 			:param rms: (float or boolean) No help available
 			:param peak: (float or boolean) No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('rms', rms, DataType.FloatExt), ArgSingle('peak', peak, DataType.FloatExt))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PERRor {param}'.rstrip())
 
 	# noinspection PyTypeChecker
@@ -40,10 +40,10 @@
 			self.Rms: float or bool = None
 			self.Peak: float or bool = None
 
 	def get(self) -> PerrorStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:LIMit:PERRor \n
 		Snippet: value: PerrorStruct = driver.configure.wcdmaMeas.prach.limit.perror.get() \n
 		Defines symmetric limits for the RMS and peak values of the phase error. The limit check fails the UE if the absolute
-		value of the measured phase error exceeds the specified values. \n
+		value of the measured phase error exceeds the specified value. \n
 			:return: structure: for return value, see the help for PerrorStruct structure arguments."""
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:LIMit:PERRor?', self.__class__.PerrorStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Limit/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/Chip.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/Chip.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 	def set_ue_power(self, enable_ue_pchip: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:CHIP:UEPower \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.chip.set_ue_power(enable_ue_pchip = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_ue_pchip: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_ue_pchip: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_ue_pchip)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:CHIP:UEPower {param}')
 
 	def get_perror(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:CHIP:PERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.chip.get_perror() \n
@@ -46,15 +46,15 @@
 
 	def set_perror(self, enable_ph_err_chip: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:CHIP:PERRor \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.chip.set_perror(enable_ph_err_chip = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_ph_err_chip: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_ph_err_chip: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_ph_err_chip)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:CHIP:PERRor {param}')
 
 	def get_merror(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:CHIP:MERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.chip.get_merror() \n
@@ -68,15 +68,15 @@
 
 	def set_merror(self, enable_merr_chip: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:CHIP:MERRor \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.chip.set_merror(enable_merr_chip = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_merr_chip: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_merr_chip: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_merr_chip)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:CHIP:MERRor {param}')
 
 	def get_evm(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:CHIP:EVM \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.chip.get_evm() \n
@@ -90,11 +90,11 @@
 
 	def set_evm(self, enable_evm_chip: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:CHIP:EVM \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.chip.set_evm(enable_evm_chip = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_evm_chip: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_evm_chip: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_evm_chip)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:CHIP:EVM {param}')
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/Result/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 	def set_ue_power(self, enable_ue_power: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:UEPower \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.set_ue_power(enable_ue_power = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_ue_power: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_ue_power: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_ue_power)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:UEPower {param}')
 
 	def get_psteps(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:PSTeps \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.get_psteps() \n
@@ -56,15 +56,15 @@
 
 	def set_psteps(self, enable_pow_steps: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:PSTeps \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.set_psteps(enable_pow_steps = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_pow_steps: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_pow_steps: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_pow_steps)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:PSTeps {param}')
 
 	def get_freq_error(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:FERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.get_freq_error() \n
@@ -78,23 +78,23 @@
 
 	def set_freq_error(self, enable_freq_error: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:FERRor \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.set_freq_error(enable_freq_error = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_freq_error: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_freq_error: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_freq_error)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:FERRor {param}')
 
 	# noinspection PyTypeChecker
 	class AllStruct(StructBase):  # From WriteStructDefinition CmdPropertyTemplate.xml
 		"""Structure for setting input parameters. Fields: \n
-			- Enable_Ue_Power: bool: UE power OFF: Do not evaluate results, hide the view ON: Evaluate results and show the view
+			- Enable_Ue_Power: bool: UE power OFF: Do not evaluate results. ON: Evaluate the results.
 			- Enable_Pow_Steps: bool: Power steps
 			- Enable_Freq_Error: bool: Frequency error
 			- Enable_Evm: bool: Error vector magnitude
 			- Enable_Mag_Error: bool: Magnitude error
 			- Enable_Phase_Err: bool: Phase error
 			- Enable_Ue_Pchip: bool: UE power vs chip
 			- Enable_Evm_Chip: bool: EVM vs chip
@@ -127,15 +127,15 @@
 			self.Enable_Merr_Chip: bool = None
 			self.Enable_Ph_Err_Chip: bool = None
 			self.Enable_Iq: bool = None
 
 	def get_all(self) -> AllStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult[:ALL] \n
 		Snippet: value: AllStruct = driver.configure.wcdmaMeas.prach.result.get_all() \n
-		Enables or disables the evaluation of results and shows or hides the views in the PRACH measurement.
+		Enables or disables the evaluation of results of the PRACH measurement.
 		This command combines all other CONFigure:WCDMa:MEAS<i>:PRACh:RESult... commands. \n
 			:return: structure: for return value, see the help for AllStruct structure arguments.
 		"""
 		return self._core.io.query_struct('CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:ALL?', self.__class__.AllStruct())
 
 	def set_all(self, value: AllStruct) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult[:ALL] \n
@@ -149,15 +149,15 @@
 		structure.Enable_Phase_Err: bool = False \n
 		structure.Enable_Ue_Pchip: bool = False \n
 		structure.Enable_Evm_Chip: bool = False \n
 		structure.Enable_Merr_Chip: bool = False \n
 		structure.Enable_Ph_Err_Chip: bool = False \n
 		structure.Enable_Iq: bool = False \n
 		driver.configure.wcdmaMeas.prach.result.set_all(value = structure) \n
-		Enables or disables the evaluation of results and shows or hides the views in the PRACH measurement.
+		Enables or disables the evaluation of results of the PRACH measurement.
 		This command combines all other CONFigure:WCDMa:MEAS<i>:PRACh:RESult... commands. \n
 			:param value: see the help for AllStruct structure arguments.
 		"""
 		self._core.io.write_struct('CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:ALL', value)
 
 	def get_perror(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:PERRor \n
@@ -172,15 +172,15 @@
 
 	def set_perror(self, enable_phase_err: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:PERRor \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.set_perror(enable_phase_err = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_phase_err: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_phase_err: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_phase_err)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:PERRor {param}')
 
 	def get_ev_magnitude(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:EVMagnitude \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.get_ev_magnitude() \n
@@ -194,15 +194,15 @@
 
 	def set_ev_magnitude(self, enable_evm: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:EVMagnitude \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.set_ev_magnitude(enable_evm = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_evm: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_evm: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_evm)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:EVMagnitude {param}')
 
 	def get_merror(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:MERRor \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.get_merror() \n
@@ -216,15 +216,15 @@
 
 	def set_merror(self, enable_mag_error: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:MERRor \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.set_merror(enable_mag_error = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_mag_error: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_mag_error: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_mag_error)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:MERRor {param}')
 
 	def get_iq(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:IQ \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.result.get_iq() \n
@@ -238,15 +238,15 @@
 
 	def set_iq(self, enable_iq: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:RESult:IQ \n
 		Snippet: driver.configure.wcdmaMeas.prach.result.set_iq(enable_iq = False) \n
 		Enables or disables the evaluation of results of the PRACH measurement identified by the last command mnemonics: UE power,
 		power steps, frequency error, error vector magnitude (EVM) , magnitude error, phase error, UE power vs chip, EVM vs chip,
 		magnitude error vs chip, phase error vs chip, and I/Q constellation measurements. \n
-			:param enable_iq: OFF: Do not evaluate results ON: Evaluate results
+			:param enable_iq: OFF: Do not evaluate results. ON: Evaluate the results.
 		"""
 		param = Conversions.bool_to_str(enable_iq)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:RESult:IQ {param}')
 
 	def clone(self) -> 'ResultCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Prach/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,24 +114,24 @@
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:OFFPower {param}')
 
 	def get_mo_exception(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:MOEXception \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.prach.get_mo_exception() \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:return: meas_on_exception: OFF: Faulty results are rejected. ON: Results are never rejected.
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:PRACh:MOEXception?')
 		return Conversions.str_to_bool(response)
 
 	def set_mo_exception(self, meas_on_exception: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:PRACh:MOEXception \n
 		Snippet: driver.configure.wcdmaMeas.prach.set_mo_exception(meas_on_exception = False) \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:param meas_on_exception: OFF: Faulty results are rejected. ON: Results are never rejected.
 		"""
 		param = Conversions.bool_to_str(meas_on_exception)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:PRACh:MOEXception {param}')
 
 	def clone(self) -> 'PrachCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/Frequency.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Dcarrier.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/Dcarrier.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/RfSettings/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,45 +46,45 @@
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:RFSettings:EATTenuation {param}')
 
 	def get_umargin(self) -> float:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:RFSettings:UMARgin \n
 		Snippet: value: float = driver.configure.wcdmaMeas.rfSettings.get_umargin() \n
 		Sets the margin that the measurement adds to the expected nominal power to determine the reference power. The reference
 		power minus the external input attenuation must be within the power range of the selected input connector. Refer to the
-		data sheet. \n
+		specifications document. \n
 			:return: user_margin: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:RFSettings:UMARgin?')
 		return Conversions.str_to_float(response)
 
 	def set_umargin(self, user_margin: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:RFSettings:UMARgin \n
 		Snippet: driver.configure.wcdmaMeas.rfSettings.set_umargin(user_margin = 1.0) \n
 		Sets the margin that the measurement adds to the expected nominal power to determine the reference power. The reference
 		power minus the external input attenuation must be within the power range of the selected input connector. Refer to the
-		data sheet. \n
+		specifications document. \n
 			:param user_margin: No help available
 		"""
 		param = Conversions.decimal_value_to_str(user_margin)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:RFSettings:UMARgin {param}')
 
 	def get_envelope_power(self) -> float:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:RFSettings:ENPower \n
 		Snippet: value: float = driver.configure.wcdmaMeas.rfSettings.get_envelope_power() \n
 		Sets the expected nominal power of the measured RF signal. \n
-			:return: exp_nom_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			:return: exp_nom_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:RFSettings:ENPower?')
 		return Conversions.str_to_float(response)
 
 	def set_envelope_power(self, exp_nom_power: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:RFSettings:ENPower \n
 		Snippet: driver.configure.wcdmaMeas.rfSettings.set_envelope_power(exp_nom_power = 1.0) \n
 		Sets the expected nominal power of the measured RF signal. \n
-			:param exp_nom_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the data sheet.
+			:param exp_nom_power: The range of the expected nominal power can be calculated as follows: Range (Expected Nominal Power) = Range (Input Power) + External Attenuation - User Margin The input power range is stated in the specifications document.
 		"""
 		param = Conversions.decimal_value_to_str(exp_nom_power)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:RFSettings:ENPower {param}')
 
 	def clone(self) -> 'RfSettingsCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/Mlength.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/Mlength.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 		self._cmd_group = CommandsGroup("mlength", core, parent)
 
 	def set(self, nr_steps: int) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:CTFC:MLENgth \n
 		Snippet: driver.configure.wcdmaMeas.tpc.ctfc.mlength.set(nr_steps = 1) \n
 		Specifies the number of power steps to be measured per step direction (n up steps + n down steps) . A query returns the
 		configured number of steps and the resulting measurement length. \n
-			:param nr_steps: Number of steps to be measured per direction
+			:param nr_steps: Number of steps to be measured per direction.
 		"""
 		param = Conversions.decimal_value_to_str(nr_steps)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:CTFC:MLENgth {param}')
 
 	# noinspection PyTypeChecker
 	class GetStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Nr_Steps: int: Number of steps to be measured per direction
-			- Meas_Length: int: Number of slots to be measured"""
+			- Nr_Steps: int: Number of steps to be measured per direction.
+			- Meas_Length: int: Number of slots to be measured."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Nr_Steps'),
 			ArgStruct.scalar_int('Meas_Length')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Nr_Steps: int = None
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ctfc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Dhib.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Dhib.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsef.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsef.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsgh.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/Tsgh.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/IlpControl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ctfc.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ctfc.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("ctfc", core, parent)
 
 	def set(self, power_step_limit: float, calc_beta_factors: bool, power_step_size: float = None) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:CTFC \n
 		Snippet: driver.configure.wcdmaMeas.tpc.limit.ctfc.set(power_step_limit = 1.0, calc_beta_factors = False, power_step_size = 1.0) \n
 		Configures a power step limit for the measurement mode Change of TFC. \n
-			:param power_step_limit: Symmetrical tolerance value for the power step size
-			:param calc_beta_factors: Enables or disables the automatic calculation of the expected power step size from the configured beta factors
-			:param power_step_size: Expected power step size applicable if the automatic calculation from beta factors is disabled
+			:param power_step_limit: Symmetrical tolerance value for the power step size.
+			:param calc_beta_factors: Enables or disables the automatic calculation of the expected power step size from the configured beta factors.
+			:param power_step_size: The expected power step size applicable if the automatic calculation from beta factors is disabled.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('power_step_limit', power_step_limit, DataType.Float), ArgSingle('calc_beta_factors', calc_beta_factors, DataType.Boolean), ArgSingle('power_step_size', power_step_size, DataType.Float, None, is_optional=True))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:CTFC {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class CtfcStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Power_Step_Limit: float: Symmetrical tolerance value for the power step size
-			- Calc_Beta_Factors: bool: Enables or disables the automatic calculation of the expected power step size from the configured beta factors
-			- Power_Step_Size: float: Expected power step size applicable if the automatic calculation from beta factors is disabled"""
+			- Power_Step_Limit: float: Symmetrical tolerance value for the power step size.
+			- Calc_Beta_Factors: bool: Enables or disables the automatic calculation of the expected power step size from the configured beta factors.
+			- Power_Step_Size: float: The expected power step size applicable if the automatic calculation from beta factors is disabled."""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Power_Step_Limit'),
 			ArgStruct.scalar_bool('Calc_Beta_Factors'),
 			ArgStruct.scalar_float('Power_Step_Size')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/EpStep.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/EpStep.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/UserDefined.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/UserDefined.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MaxPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MinPower.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/MinPower.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("minPower", core, parent)
 
 	def set(self, enable: bool, upper_limit: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:ILPControl:MINPower \n
 		Snippet: driver.configure.wcdmaMeas.tpc.limit.ilpControl.minPower.set(enable = False, upper_limit = 1.0) \n
-		Defines an Inner Loop Power Control limit: upper limit for the minimum UE output power. Also enables or disables the
+		Defines an Inner Loop Power Control limit: upper limit for the minimum UE output power. Also it enables or disables the
 		limit check. \n
-			:param enable: Disables | enables the limit check
+			:param enable: Disables | enables the limit check.
 			:param upper_limit: No help available
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('upper_limit', upper_limit, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:ILPControl:MINPower {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class MinPowerStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
+			- Enable: bool: Disables | enables the limit check.
 			- Upper_Limit: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Upper_Limit')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Enable: bool = None
 			self.Upper_Limit: float = None
 
 	def get(self) -> MinPowerStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:ILPControl:MINPower \n
 		Snippet: value: MinPowerStruct = driver.configure.wcdmaMeas.tpc.limit.ilpControl.minPower.get() \n
-		Defines an Inner Loop Power Control limit: upper limit for the minimum UE output power. Also enables or disables the
+		Defines an Inner Loop Power Control limit: upper limit for the minimum UE output power. Also it enables or disables the
 		limit check. \n
 			:return: structure: for return value, see the help for MinPowerStruct structure arguments."""
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:ILPControl:MINPower?', self.__class__.MinPowerStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/PsGroup.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/PsGroup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("psGroup", core, parent)
 
 	def set(self, enable: bool, group_10_x_0_db: float, group_10_x_1_dba_lg_2: float, group_10_x_1_db: float, group_10_x_2_db: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:ILPControl:PSGRoup \n
 		Snippet: driver.configure.wcdmaMeas.tpc.limit.ilpControl.psGroup.set(enable = False, group_10_x_0_db = 1.0, group_10_x_1_dba_lg_2 = 1.0, group_10_x_1_db = 1.0, group_10_x_2_db = 1.0) \n
 		Defines Inner Loop Power Control limits: upper limits for the absolute value of the power step group error, depending on
-		the expected step size. Also enables or disables the limit check. \n
-			:param enable: Disables | enables the limit check
-			:param group_10_x_0_db: Limit for groups with expected step size 10 x 0 dB (algorithm 2)
-			:param group_10_x_1_dba_lg_2: Limit for groups with expected step size 10 x ±1 dB + 40 x 0 dB (algorithm 2)
-			:param group_10_x_1_db: Limit for groups with expected step size 10 x ±1 dB (algorithm 1)
-			:param group_10_x_2_db: Limit for groups with expected step size 10 x ±2 dB (algorithm 1)
+		the expected step size. Also it enables or disables the limit check. \n
+			:param enable: Disables | enables the limit check.
+			:param group_10_x_0_db: Limit for groups with expected step size 10 x 0 dB (algorithm 2) .
+			:param group_10_x_1_dba_lg_2: Limit for groups with expected step size 10 x ±1 dB + 40 x 0 dB (algorithm 2) .
+			:param group_10_x_1_db: Limit for groups with expected step size 10 x ±1 dB (algorithm 1) .
+			:param group_10_x_2_db: Limit for groups with expected step size 10 x ±2 dB (algorithm 1) .
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('group_10_x_0_db', group_10_x_0_db, DataType.Float), ArgSingle('group_10_x_1_dba_lg_2', group_10_x_1_dba_lg_2, DataType.Float), ArgSingle('group_10_x_1_db', group_10_x_1_db, DataType.Float), ArgSingle('group_10_x_2_db', group_10_x_2_db, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:ILPControl:PSGRoup {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class PsGroupStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
-			- Group_10_X_0_Db: float: Limit for groups with expected step size 10 x 0 dB (algorithm 2)
-			- Group_10_X_1_Dba_Lg_2: float: Limit for groups with expected step size 10 x ±1 dB + 40 x 0 dB (algorithm 2)
-			- Group_10_X_1_Db: float: Limit for groups with expected step size 10 x ±1 dB (algorithm 1)
-			- Group_10_X_2_Db: float: Limit for groups with expected step size 10 x ±2 dB (algorithm 1)"""
+			- Enable: bool: Disables | enables the limit check.
+			- Group_10_X_0_Db: float: Limit for groups with expected step size 10 x 0 dB (algorithm 2) .
+			- Group_10_X_1_Dba_Lg_2: float: Limit for groups with expected step size 10 x ±1 dB + 40 x 0 dB (algorithm 2) .
+			- Group_10_X_1_Db: float: Limit for groups with expected step size 10 x ±1 dB (algorithm 1) .
+			- Group_10_X_2_Db: float: Limit for groups with expected step size 10 x ±2 dB (algorithm 1) ."""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Group_10_X_0_Db'),
 			ArgStruct.scalar_float('Group_10_X_1_Dba_Lg_2'),
 			ArgStruct.scalar_float('Group_10_X_1_Db'),
 			ArgStruct.scalar_float('Group_10_X_2_Db')]
 
@@ -52,10 +52,10 @@
 			self.Group_10_X_1_Db: float = None
 			self.Group_10_X_2_Db: float = None
 
 	def get(self) -> PsGroupStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:ILPControl:PSGRoup \n
 		Snippet: value: PsGroupStruct = driver.configure.wcdmaMeas.tpc.limit.ilpControl.psGroup.get() \n
 		Defines Inner Loop Power Control limits: upper limits for the absolute value of the power step group error, depending on
-		the expected step size. Also enables or disables the limit check. \n
+		the expected step size. Also it enables or disables the limit check. \n
 			:return: structure: for return value, see the help for PsGroupStruct structure arguments."""
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:ILPControl:PSGRoup?', self.__class__.PsGroupStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/Pstep.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/Pstep.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("pstep", core, parent)
 
 	def set(self, enable: bool, step_0_db: float, step_1_db: float, step_2_db: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:ILPControl:PSTep \n
 		Snippet: driver.configure.wcdmaMeas.tpc.limit.ilpControl.pstep.set(enable = False, step_0_db = 1.0, step_1_db = 1.0, step_2_db = 1.0) \n
 		Defines Inner Loop Power Control limits: upper limits for the absolute value of the power step error, depending on the
-		expected step size. Also enables or disables the limit check. \n
-			:param enable: Disables | enables the limit check
-			:param step_0_db: Limit for steps with expected step size 0 dB
-			:param step_1_db: Limit for steps with expected step size ±1 dB
-			:param step_2_db: Limit for steps with expected step size ±2 dB
+		expected step size. Also it enables or disables the limit check. \n
+			:param enable: Disables | enables the limit check.
+			:param step_0_db: Limit for steps with expected step size 0 dB.
+			:param step_1_db: Limit for steps with expected step size ±1 dB.
+			:param step_2_db: Limit for steps with expected step size ±2 dB.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('step_0_db', step_0_db, DataType.Float), ArgSingle('step_1_db', step_1_db, DataType.Float), ArgSingle('step_2_db', step_2_db, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:ILPControl:PSTep {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class PstepStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
-			- Step_0_Db: float: Limit for steps with expected step size 0 dB
-			- Step_1_Db: float: Limit for steps with expected step size ±1 dB
-			- Step_2_Db: float: Limit for steps with expected step size ±2 dB"""
+			- Enable: bool: Disables | enables the limit check.
+			- Step_0_Db: float: Limit for steps with expected step size 0 dB.
+			- Step_1_Db: float: Limit for steps with expected step size ±1 dB.
+			- Step_2_Db: float: Limit for steps with expected step size ±2 dB."""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Step_0_Db'),
 			ArgStruct.scalar_float('Step_1_Db'),
 			ArgStruct.scalar_float('Step_2_Db')]
 
 		def __init__(self):
@@ -48,10 +48,10 @@
 			self.Step_1_Db: float = None
 			self.Step_2_Db: float = None
 
 	def get(self) -> PstepStruct:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:ILPControl:PSTep \n
 		Snippet: value: PstepStruct = driver.configure.wcdmaMeas.tpc.limit.ilpControl.pstep.get() \n
 		Defines Inner Loop Power Control limits: upper limits for the absolute value of the power step error, depending on the
-		expected step size. Also enables or disables the limit check. \n
+		expected step size. Also it enables or disables the limit check. \n
 			:return: structure: for return value, see the help for PstepStruct structure arguments."""
 		return self._core.io.query_struct(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:ILPControl:PSTep?', self.__class__.PstepStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/IlpControl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Mpedch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Mpedch.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("mpedch", core, parent)
 
 	def set(self, enable: bool, nom_max_power: float, upper_limit: float, lower_limit: float) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:LIMit:MPEDch \n
 		Snippet: driver.configure.wcdmaMeas.tpc.limit.mpedch.set(enable = False, nom_max_power = 1.0, upper_limit = 1.0, lower_limit = 1.0) \n
 		Configures UE power limits for the measurement mode Max. Power E-DCH. \n
-			:param enable: Disables | enables the limit check
-			:param nom_max_power: Nominal maximum UE power
-			:param upper_limit: Upper limit = nominal power + this value
-			:param lower_limit: Lower limit = nominal power + this value
+			:param enable: Disables | enables the limit check.
+			:param nom_max_power: Nominal maximum UE power.
+			:param upper_limit: Upper limit = nominal power + this value.
+			:param lower_limit: Lower limit = nominal power + this value.
 		"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('enable', enable, DataType.Boolean), ArgSingle('nom_max_power', nom_max_power, DataType.Float), ArgSingle('upper_limit', upper_limit, DataType.Float), ArgSingle('lower_limit', lower_limit, DataType.Float))
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:LIMit:MPEDch {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class MpedchStruct(StructBase):
 		"""Response structure. Fields: \n
-			- Enable: bool: Disables | enables the limit check
-			- Nom_Max_Power: float: Nominal maximum UE power
-			- Upper_Limit: float: Upper limit = nominal power + this value
-			- Lower_Limit: float: Lower limit = nominal power + this value"""
+			- Enable: bool: Disables | enables the limit check.
+			- Nom_Max_Power: float: Nominal maximum UE power.
+			- Upper_Limit: float: Upper limit = nominal power + this value.
+			- Lower_Limit: float: Lower limit = nominal power + this value."""
 		__meta_args_list = [
 			ArgStruct.scalar_bool('Enable'),
 			ArgStruct.scalar_float('Nom_Max_Power'),
 			ArgStruct.scalar_float('Upper_Limit'),
 			ArgStruct.scalar_float('Lower_Limit')]
 
 		def __init__(self):
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pa.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pa.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pb.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/Pb.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/Ulcm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Limit/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Monitor.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Monitor.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Mpedch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Mpedch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ulcm.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/Ulcm.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/Tpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,24 +115,24 @@
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:TPC:MODE?')
 		return Conversions.str_to_scalar_enum(response, enums.MeasMode)
 
 	def get_mo_exception(self) -> bool:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:MOEXception \n
 		Snippet: value: bool = driver.configure.wcdmaMeas.tpc.get_mo_exception() \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:return: meas_on_exception: OFF: Faulty results are rejected. ON: Results are never rejected.
 		"""
 		response = self._core.io.query_str('CONFigure:WCDMa:MEASurement<Instance>:TPC:MOEXception?')
 		return Conversions.str_to_bool(response)
 
 	def set_mo_exception(self, meas_on_exception: bool) -> None:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:MOEXception \n
 		Snippet: driver.configure.wcdmaMeas.tpc.set_mo_exception(meas_on_exception = False) \n
-		Specifies whether measurement results that the R&S CMP180 identifies as faulty or inaccurate are rejected. \n
+		Specifies whether measurement results that the CMP180 identifies as faulty or inaccurate are rejected. \n
 			:param meas_on_exception: OFF: Faulty results are rejected. ON: Results are never rejected.
 		"""
 		param = Conversions.bool_to_str(meas_on_exception)
 		self._core.io.write(f'CONFigure:WCDMa:MEASurement<Instance>:TPC:MOEXception {param}')
 
 	def get_timeout(self) -> float:
 		"""SCPI: CONFigure:WCDMa:MEASurement<instance>:TPC:TOUT \n
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpcch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpdch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Dpdch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpcch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpdch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Edpdch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/Config.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/Config.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/Hsdpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeChannels/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/Scode.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/Scode.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/UeSignal/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/WcdmaMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Configure/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Configure/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/MaProtocol.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/MaProtocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("maProtocol", core, parent)
 
 	def set(self, controler: str = None) -> None:
 		"""SCPI: ROUTe:WCDMa:MEASurement<instance>:SCENario:MAPRotocol \n
-		Snippet: driver.route.wcdmaMeas.scenario.maProtocol.set(controler = '1') \n
+		Snippet: driver.route.wcdmaMeas.scenario.maProtocol.set(controler = 'abc') \n
 		No command help available \n
 			:param controler: No help available
 		"""
 		param = ''
 		if controler:
 			param = Conversions.value_to_quoted_str(controler)
 		self._core.io.write(f'ROUTe:WCDMa:MEASurement<Instance>:SCENario:MAPRotocol {param}'.strip())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/Salone.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/Salone.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/Scenario/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 			:return: master: No help available
 		"""
 		response = self._core.io.query_str('ROUTe:WCDMa:MEASurement<Instance>:SCENario:CSPath?')
 		return trim_str_response(response)
 
 	def set_cspath(self, master: str) -> None:
 		"""SCPI: ROUTe:WCDMa:MEASurement<instance>:SCENario:CSPath \n
-		Snippet: driver.route.wcdmaMeas.scenario.set_cspath(master = '1') \n
+		Snippet: driver.route.wcdmaMeas.scenario.set_cspath(master = 'abc') \n
 		No command help available \n
 			:param master: No help available
 		"""
 		param = Conversions.value_to_quoted_str(master)
 		self._core.io.write(f'ROUTe:WCDMa:MEASurement<Instance>:SCENario:CSPath {param}')
 
 	# noinspection PyTypeChecker
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/WcdmaMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Route/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Route/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/Catalog.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/ListPy.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/ListPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/MultiEval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 			self._catalog = CatalogCls(self._core, self._cmd_group)
 		return self._catalog
 
 	def get_delay(self) -> float:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:MEValuation:DELay \n
 		Snippet: value: float = driver.trigger.wcdmaMeas.multiEval.get_delay() \n
 		Defines a time delaying the start of the measurement relative to the trigger event. A delay is useful if the trigger
-		event and the uplink DPCH slot border are not synchronous. A measurement starts always at an uplink DPCH slot border.
+		event and the uplink DPCH slot border are not synchronous. A measurement always starts at an uplink DPCH slot border.
 		Triggering a measurement at another time can yield a synchronization error. For internal trigger sources aligned to the
 		downlink DPCH, an additional delay of 1024 chips is automatically applied. It corresponds to the assumed delay between
 		downlink and uplink slot. This setting has no influence on free run measurements. \n
 			:return: delay: No help available
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:MEValuation:DELay?')
 		return Conversions.str_to_float(response)
 
 	def set_delay(self, delay: float) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:MEValuation:DELay \n
 		Snippet: driver.trigger.wcdmaMeas.multiEval.set_delay(delay = 1.0) \n
 		Defines a time delaying the start of the measurement relative to the trigger event. A delay is useful if the trigger
-		event and the uplink DPCH slot border are not synchronous. A measurement starts always at an uplink DPCH slot border.
+		event and the uplink DPCH slot border are not synchronous. A measurement always starts at an uplink DPCH slot border.
 		Triggering a measurement at another time can yield a synchronization error. For internal trigger sources aligned to the
 		downlink DPCH, an additional delay of 1024 chips is automatically applied. It corresponds to the assumed delay between
 		downlink and uplink slot. This setting has no influence on free run measurements. \n
 			:param delay: No help available
 		"""
 		param = Conversions.decimal_value_to_str(delay)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:MEValuation:DELay {param}')
@@ -143,15 +143,15 @@
 			:return: source: 'Free Run (Standard) ': Free run (standard synchronization) 'Free Run (Fast Sync) ': Free run (fast synchronization) 'IF Power': Power trigger (normal synchronization) 'IF Power (Sync) ': Power trigger (extended synchronization)
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:MEValuation:SOURce?')
 		return trim_str_response(response)
 
 	def set_source(self, source: str) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:MEValuation:SOURce \n
-		Snippet: driver.trigger.wcdmaMeas.multiEval.set_source(source = '1') \n
+		Snippet: driver.trigger.wcdmaMeas.multiEval.set_source(source = 'abc') \n
 		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
 		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
 		:CATalog:SOURce?. \n
 			:param source: 'Free Run (Standard) ': Free run (standard synchronization) 'Free Run (Fast Sync) ': Free run (fast synchronization) 'IF Power': Power trigger (normal synchronization) 'IF Power (Sync) ': Power trigger (extended synchronization)
 		"""
 		param = Conversions.value_to_quoted_str(source)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:MEValuation:SOURce {param}')
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/Catalog.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OlpControl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 			:return: source: No help available
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:OLPControl:SOURce?')
 		return trim_str_response(response)
 
 	def set_source(self, source: str) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:OLPControl:SOURce \n
-		Snippet: driver.trigger.wcdmaMeas.olpControl.set_source(source = '1') \n
+		Snippet: driver.trigger.wcdmaMeas.olpControl.set_source(source = 'abc') \n
 		No command help available \n
 			:param source: No help available
 		"""
 		param = Conversions.value_to_quoted_str(source)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:OLPControl:SOURce {param}')
 
 	def clone(self) -> 'OlpControlCls':
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/Catalog.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/OoSync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 			:return: source: No help available
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:OOSYnc:SOURce?')
 		return trim_str_response(response)
 
 	def set_source(self, source: str) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:OOSYnc:SOURce \n
-		Snippet: driver.trigger.wcdmaMeas.ooSync.set_source(source = '1') \n
+		Snippet: driver.trigger.wcdmaMeas.ooSync.set_source(source = 'abc') \n
 		No command help available \n
 			:param source: No help available
 		"""
 		param = Conversions.value_to_quoted_str(source)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:OOSYnc:SOURce {param}')
 
 	def clone(self) -> 'OoSyncCls':
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/Catalog.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Prach/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,26 +97,26 @@
 		"""
 		param = Conversions.enum_scalar_to_str(slope, enums.SignalSlope)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:PRACh:SLOPe {param}')
 
 	def get_timeout(self) -> float or bool:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:PRACh:TOUT \n
 		Snippet: value: float or bool = driver.trigger.wcdmaMeas.prach.get_timeout() \n
-		Selects the maximum time that the R&S CMP180 waits for a trigger event before it stops the measurement in remote control
-		mode or indicates a trigger timeout in manual operation mode. \n
+		Selects the maximum time that the CMP180 waits for a trigger event before it stops the measurement in remote control mode
+		or indicates a trigger timeout in manual operation mode. \n
 			:return: timeout: (float or boolean) No help available
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:PRACh:TOUT?')
 		return Conversions.str_to_float_or_bool(response)
 
 	def set_timeout(self, timeout: float or bool) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:PRACh:TOUT \n
 		Snippet: driver.trigger.wcdmaMeas.prach.set_timeout(timeout = 1.0) \n
-		Selects the maximum time that the R&S CMP180 waits for a trigger event before it stops the measurement in remote control
-		mode or indicates a trigger timeout in manual operation mode. \n
+		Selects the maximum time that the CMP180 waits for a trigger event before it stops the measurement in remote control mode
+		or indicates a trigger timeout in manual operation mode. \n
 			:param timeout: (float or boolean) No help available
 		"""
 		param = Conversions.decimal_or_bool_value_to_str(timeout)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:PRACh:TOUT {param}')
 
 	def get_source(self) -> str:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:PRACh:SOURce \n
@@ -127,15 +127,15 @@
 			:return: source: 'IF Power (Sync) ': Power trigger (extended synchronization)
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:PRACh:SOURce?')
 		return trim_str_response(response)
 
 	def set_source(self, source: str) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:PRACh:SOURce \n
-		Snippet: driver.trigger.wcdmaMeas.prach.set_source(source = '1') \n
+		Snippet: driver.trigger.wcdmaMeas.prach.set_source(source = 'abc') \n
 		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
 		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
 		:CATalog:SOURce?. \n
 			:param source: 'IF Power (Sync) ': Power trigger (extended synchronization)
 		"""
 		param = Conversions.value_to_quoted_str(source)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:PRACh:SOURce {param}')
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/Catalog.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/Tpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 			self._catalog = CatalogCls(self._core, self._cmd_group)
 		return self._catalog
 
 	def get_delay(self) -> float:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:TPC:DELay \n
 		Snippet: value: float = driver.trigger.wcdmaMeas.tpc.get_delay() \n
 		Defines a time delaying the start of the measurement relative to the trigger event. The delay is useful if the trigger
-		event and the uplink DPCH slot border are not synchronous. A measurement starts always at an uplink DPCH slot border.
+		event and the uplink DPCH slot border are not synchronous. A measurement always starts at an uplink DPCH slot border.
 		Triggering a measurement at another time yields a synchronization error. For internal trigger sources aligned to the
 		downlink DPCH, an additional delay of 1024 chips is automatically applied. It corresponds to the assumed delay between
 		downlink and uplink slot. This setting has no influence on Free Run measurements. \n
 			:return: delay: No help available
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:TPC:DELay?')
 		return Conversions.str_to_float(response)
 
 	def set_delay(self, delay: float) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:TPC:DELay \n
 		Snippet: driver.trigger.wcdmaMeas.tpc.set_delay(delay = 1.0) \n
 		Defines a time delaying the start of the measurement relative to the trigger event. The delay is useful if the trigger
-		event and the uplink DPCH slot border are not synchronous. A measurement starts always at an uplink DPCH slot border.
+		event and the uplink DPCH slot border are not synchronous. A measurement always starts at an uplink DPCH slot border.
 		Triggering a measurement at another time yields a synchronization error. For internal trigger sources aligned to the
 		downlink DPCH, an additional delay of 1024 chips is automatically applied. It corresponds to the assumed delay between
 		downlink and uplink slot. This setting has no influence on Free Run measurements. \n
 			:param delay: No help available
 		"""
 		param = Conversions.decimal_value_to_str(delay)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:TPC:DELay {param}')
@@ -135,15 +135,15 @@
 			:return: source: 'Free Run (Standard) ': Free run (standard synchronization) 'Free Run (Fast Sync) ': Free run (fast synchronization) 'IF Power': Power trigger (normal synchronization) 'IF Power (Sync) ': Power trigger (extended synchronization)
 		"""
 		response = self._core.io.query_str('TRIGger:WCDMa:MEASurement<Instance>:TPC:SOURce?')
 		return trim_str_response(response)
 
 	def set_source(self, source: str) -> None:
 		"""SCPI: TRIGger:WCDMa:MEASurement<instance>:TPC:SOURce \n
-		Snippet: driver.trigger.wcdmaMeas.tpc.set_source(source = '1') \n
+		Snippet: driver.trigger.wcdmaMeas.tpc.set_source(source = 'abc') \n
 		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
 		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
 		:CATalog:SOURce?. \n
 			:param source: 'Free Run (Standard) ': Free run (standard synchronization) 'Free Run (Fast Sync) ': Free run (fast synchronization) 'IF Power': Power trigger (normal synchronization) 'IF Power (Sync) ': Power trigger (extended synchronization)
 		"""
 		param = Conversions.value_to_quoted_str(source)
 		self._core.io.write(f'TRIGger:WCDMa:MEASurement<Instance>:TPC:SOURce {param}')
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/WcdmaMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/Trigger/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/Trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Ber.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Ber.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/CdPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Current.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
-from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class AverageCls:
-	"""Average commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
+class CurrentCls:
+	"""Current commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("average", core, parent)
+		self._cmd_group = CommandsGroup("current", core, parent)
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value
-			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float or bool: Magnitude error RMS value
-			- Mag_Error_Peak: float or bool: Magnitude error peak value
+			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float or bool: Magnitude error RMS value.
+			- Mag_Error_Peak: float or bool: Magnitude error peak value.
 			- Phase_Error_Rms: float or bool: No parameter help available
 			- Phase_Error_Peak: float or bool: No parameter help available
-			- Iq_Offset: float or bool: I/Q origin offset
-			- Iq_Imbalance: float or bool: I/Q imbalance
+			- Iq_Offset: float or bool: I/Q origin offset.
+			- Iq_Imbalance: float or bool: I/Q imbalance.
 			- Carrier_Freq_Err: float or bool: No parameter help available
 			- Transmit_Time_Err: float or bool: No parameter help available
-			- Ue_Power: float or bool: User equipment power
-			- Power_Steps: float or bool: User equipment power step
-			- Phase_Disc: enums.ResultStatus2: Phase discontinuity"""
+			- Ue_Power: float or bool: User equipment power.
+			- Power_Steps: float or bool: User equipment power step.
+			- Phase_Disc: float or bool: Phase discontinuity."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Evm_Rms'),
 			ArgStruct.scalar_float_ext('Evm_Peak'),
 			ArgStruct.scalar_float_ext('Mag_Error_Rms'),
 			ArgStruct.scalar_float_ext('Mag_Error_Peak'),
 			ArgStruct.scalar_float_ext('Phase_Error_Rms'),
 			ArgStruct.scalar_float_ext('Phase_Error_Peak'),
 			ArgStruct.scalar_float_ext('Iq_Offset'),
 			ArgStruct.scalar_float_ext('Iq_Imbalance'),
 			ArgStruct.scalar_float_ext('Carrier_Freq_Err'),
 			ArgStruct.scalar_float_ext('Transmit_Time_Err'),
 			ArgStruct.scalar_float_ext('Ue_Power'),
 			ArgStruct.scalar_float_ext('Power_Steps'),
-			ArgStruct.scalar_enum('Phase_Disc', enums.ResultStatus2)]
+			ArgStruct.scalar_float_ext('Phase_Disc')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Evm_Rms: float or bool = None
 			self.Evm_Peak: float or bool = None
 			self.Mag_Error_Rms: float or bool = None
@@ -58,44 +57,44 @@
 			self.Phase_Error_Peak: float or bool = None
 			self.Iq_Offset: float or bool = None
 			self.Iq_Imbalance: float or bool = None
 			self.Carrier_Freq_Err: float or bool = None
 			self.Transmit_Time_Err: float or bool = None
 			self.Ue_Power: float or bool = None
 			self.Power_Steps: float or bool = None
-			self.Phase_Disc: enums.ResultStatus2 = None
+			self.Phase_Disc: float or bool = None
 
 	def calculate(self, carrier=repcap.Carrier.Default) -> CalculateStruct:
-		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:AVERage \n
-		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.average.calculate(carrier = repcap.Carrier.Default) \n
+		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:CURRent \n
+		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.current.calculate(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:AVERage?', self.__class__.CalculateStruct())
+		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:CURRent?', self.__class__.CalculateStruct())
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float: Error vector magnitude RMS and peak value
-			- Evm_Peak: float: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float: Magnitude error RMS value
-			- Mag_Error_Peak: float: Magnitude error peak value
+			- Evm_Rms: float: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float: Magnitude error RMS value.
+			- Mag_Error_Peak: float: Magnitude error peak value.
 			- Phase_Error_Rms: float: No parameter help available
 			- Phase_Error_Peak: float: No parameter help available
-			- Iq_Offset: float: I/Q origin offset
-			- Iq_Imbalance: float: I/Q imbalance
+			- Iq_Offset: float: I/Q origin offset.
+			- Iq_Imbalance: float: I/Q imbalance.
 			- Carrier_Freq_Err: float: No parameter help available
 			- Transmit_Time_Err: float: No parameter help available
-			- Ue_Power: float: User equipment power
-			- Power_Steps: float: User equipment power step
-			- Phase_Disc: float: Phase discontinuity
+			- Ue_Power: float: User equipment power.
+			- Power_Steps: float: User equipment power step.
+			- Phase_Disc: float: Phase discontinuity.
 			- Tx_Time_Alignment: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Evm_Rms'),
 			ArgStruct.scalar_float('Evm_Peak'),
 			ArgStruct.scalar_float('Mag_Error_Rms'),
 			ArgStruct.scalar_float('Mag_Error_Peak'),
@@ -124,28 +123,28 @@
 			self.Carrier_Freq_Err: float = None
 			self.Transmit_Time_Err: float = None
 			self.Ue_Power: float = None
 			self.Power_Steps: float = None
 			self.Phase_Disc: float = None
 			self.Tx_Time_Alignment: float = None
 
-	def fetch(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:AVERage \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.average.fetch(carrier = repcap.Carrier.Default) \n
+	def read(self, carrier=repcap.Carrier.Default) -> ResultData:
+		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:CURRent \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.current.read(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:AVERage?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:CURRent?', self.__class__.ResultData())
 
-	def read(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:AVERage \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.average.read(carrier = repcap.Carrier.Default) \n
+	def fetch(self, carrier=repcap.Carrier.Default) -> ResultData:
+		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:CURRent \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.current.fetch(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:AVERage?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:CURRent?', self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Maximum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
+from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class CurrentCls:
-	"""Current commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
+class MaximumCls:
+	"""Maximum commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("current", core, parent)
+		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value
-			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float or bool: Magnitude error RMS value
-			- Mag_Error_Peak: float or bool: Magnitude error peak value
+			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float or bool: Magnitude error RMS value.
+			- Mag_Error_Peak: float or bool: Magnitude error peak value.
 			- Phase_Error_Rms: float or bool: No parameter help available
 			- Phase_Error_Peak: float or bool: No parameter help available
-			- Iq_Offset: float or bool: I/Q origin offset
-			- Iq_Imbalance: float or bool: I/Q imbalance
+			- Iq_Offset: float or bool: I/Q origin offset.
+			- Iq_Imbalance: float or bool: I/Q imbalance.
 			- Carrier_Freq_Err: float or bool: No parameter help available
 			- Transmit_Time_Err: float or bool: No parameter help available
-			- Ue_Power: float or bool: User equipment power
-			- Power_Steps: float or bool: User equipment power step
-			- Phase_Disc: float or bool: Phase discontinuity"""
+			- Ue_Power: float or bool: User equipment power.
+			- Power_Steps: float or bool: User equipment power step.
+			- Phase_Disc: enums.ResultStatus2: Phase discontinuity."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Evm_Rms'),
 			ArgStruct.scalar_float_ext('Evm_Peak'),
 			ArgStruct.scalar_float_ext('Mag_Error_Rms'),
 			ArgStruct.scalar_float_ext('Mag_Error_Peak'),
 			ArgStruct.scalar_float_ext('Phase_Error_Rms'),
 			ArgStruct.scalar_float_ext('Phase_Error_Peak'),
 			ArgStruct.scalar_float_ext('Iq_Offset'),
 			ArgStruct.scalar_float_ext('Iq_Imbalance'),
 			ArgStruct.scalar_float_ext('Carrier_Freq_Err'),
 			ArgStruct.scalar_float_ext('Transmit_Time_Err'),
 			ArgStruct.scalar_float_ext('Ue_Power'),
 			ArgStruct.scalar_float_ext('Power_Steps'),
-			ArgStruct.scalar_float_ext('Phase_Disc')]
+			ArgStruct.scalar_enum('Phase_Disc', enums.ResultStatus2)]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Reliability: int = None
 			self.Evm_Rms: float or bool = None
 			self.Evm_Peak: float or bool = None
 			self.Mag_Error_Rms: float or bool = None
@@ -57,44 +58,44 @@
 			self.Phase_Error_Peak: float or bool = None
 			self.Iq_Offset: float or bool = None
 			self.Iq_Imbalance: float or bool = None
 			self.Carrier_Freq_Err: float or bool = None
 			self.Transmit_Time_Err: float or bool = None
 			self.Ue_Power: float or bool = None
 			self.Power_Steps: float or bool = None
-			self.Phase_Disc: float or bool = None
+			self.Phase_Disc: enums.ResultStatus2 = None
 
 	def calculate(self, carrier=repcap.Carrier.Default) -> CalculateStruct:
-		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:CURRent \n
-		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.current.calculate(carrier = repcap.Carrier.Default) \n
+		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:MAXimum \n
+		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.maximum.calculate(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:CURRent?', self.__class__.CalculateStruct())
+		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:MAXimum?', self.__class__.CalculateStruct())
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float: Error vector magnitude RMS and peak value
-			- Evm_Peak: float: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float: Magnitude error RMS value
-			- Mag_Error_Peak: float: Magnitude error peak value
+			- Evm_Rms: float: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float: Magnitude error RMS value.
+			- Mag_Error_Peak: float: Magnitude error peak value.
 			- Phase_Error_Rms: float: No parameter help available
 			- Phase_Error_Peak: float: No parameter help available
-			- Iq_Offset: float: I/Q origin offset
-			- Iq_Imbalance: float: I/Q imbalance
+			- Iq_Offset: float: I/Q origin offset.
+			- Iq_Imbalance: float: I/Q imbalance.
 			- Carrier_Freq_Err: float: No parameter help available
 			- Transmit_Time_Err: float: No parameter help available
-			- Ue_Power: float: User equipment power
-			- Power_Steps: float: User equipment power step
-			- Phase_Disc: float: Phase discontinuity
+			- Ue_Power: float: User equipment power.
+			- Power_Steps: float: User equipment power step.
+			- Phase_Disc: float: Phase discontinuity.
 			- Tx_Time_Alignment: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Evm_Rms'),
 			ArgStruct.scalar_float('Evm_Peak'),
 			ArgStruct.scalar_float('Mag_Error_Rms'),
 			ArgStruct.scalar_float('Mag_Error_Peak'),
@@ -124,27 +125,27 @@
 			self.Transmit_Time_Err: float = None
 			self.Ue_Power: float = None
 			self.Power_Steps: float = None
 			self.Phase_Disc: float = None
 			self.Tx_Time_Alignment: float = None
 
 	def read(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:CURRent \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.current.read(carrier = repcap.Carrier.Default) \n
+		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:MAXimum \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.maximum.read(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:CURRent?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:MAXimum?', self.__class__.ResultData())
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:CURRent \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.current.fetch(carrier = repcap.Carrier.Default) \n
+		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:MAXimum \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.maximum.fetch(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:CURRent?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:MAXimum?', self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/StandardDev.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class MaximumCls:
-	"""Maximum commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
+class StandardDevCls:
+	"""StandardDev commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("maximum", core, parent)
+		self._cmd_group = CommandsGroup("standardDev", core, parent)
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value
-			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float or bool: Magnitude error RMS value
-			- Mag_Error_Peak: float or bool: Magnitude error peak value
+			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float or bool: Magnitude error RMS value.
+			- Mag_Error_Peak: float or bool: Magnitude error peak value.
 			- Phase_Error_Rms: float or bool: No parameter help available
 			- Phase_Error_Peak: float or bool: No parameter help available
-			- Iq_Offset: float or bool: I/Q origin offset
-			- Iq_Imbalance: float or bool: I/Q imbalance
+			- Iq_Offset: float or bool: I/Q origin offset.
+			- Iq_Imbalance: float or bool: I/Q imbalance.
 			- Carrier_Freq_Err: float or bool: No parameter help available
 			- Transmit_Time_Err: float or bool: No parameter help available
-			- Ue_Power: float or bool: User equipment power
-			- Power_Steps: float or bool: User equipment power step
-			- Phase_Disc: enums.ResultStatus2: Phase discontinuity"""
+			- Ue_Power: float or bool: User equipment power.
+			- Power_Steps: float or bool: User equipment power step.
+			- Phase_Disc: enums.ResultStatus2: Phase discontinuity."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Evm_Rms'),
 			ArgStruct.scalar_float_ext('Evm_Peak'),
 			ArgStruct.scalar_float_ext('Mag_Error_Rms'),
 			ArgStruct.scalar_float_ext('Mag_Error_Peak'),
 			ArgStruct.scalar_float_ext('Phase_Error_Rms'),
@@ -61,41 +61,41 @@
 			self.Carrier_Freq_Err: float or bool = None
 			self.Transmit_Time_Err: float or bool = None
 			self.Ue_Power: float or bool = None
 			self.Power_Steps: float or bool = None
 			self.Phase_Disc: enums.ResultStatus2 = None
 
 	def calculate(self, carrier=repcap.Carrier.Default) -> CalculateStruct:
-		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:MAXimum \n
-		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.maximum.calculate(carrier = repcap.Carrier.Default) \n
+		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:SDEViation \n
+		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.standardDev.calculate(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:MAXimum?', self.__class__.CalculateStruct())
+		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:SDEViation?', self.__class__.CalculateStruct())
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float: Error vector magnitude RMS and peak value
-			- Evm_Peak: float: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float: Magnitude error RMS value
-			- Mag_Error_Peak: float: Magnitude error peak value
+			- Evm_Rms: float: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float: Magnitude error RMS value.
+			- Mag_Error_Peak: float: Magnitude error peak value.
 			- Phase_Error_Rms: float: No parameter help available
 			- Phase_Error_Peak: float: No parameter help available
-			- Iq_Offset: float: I/Q origin offset
-			- Iq_Imbalance: float: I/Q imbalance
+			- Iq_Offset: float: I/Q origin offset.
+			- Iq_Imbalance: float: I/Q imbalance.
 			- Carrier_Freq_Err: float: No parameter help available
 			- Transmit_Time_Err: float: No parameter help available
-			- Ue_Power: float: User equipment power
-			- Power_Steps: float: User equipment power step
-			- Phase_Disc: float: Phase discontinuity
+			- Ue_Power: float: User equipment power.
+			- Power_Steps: float: User equipment power step.
+			- Phase_Disc: float: Phase discontinuity.
 			- Tx_Time_Alignment: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Evm_Rms'),
 			ArgStruct.scalar_float('Evm_Peak'),
 			ArgStruct.scalar_float('Mag_Error_Rms'),
 			ArgStruct.scalar_float('Mag_Error_Peak'),
@@ -125,27 +125,27 @@
 			self.Transmit_Time_Err: float = None
 			self.Ue_Power: float = None
 			self.Power_Steps: float = None
 			self.Phase_Disc: float = None
 			self.Tx_Time_Alignment: float = None
 
 	def read(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:MAXimum \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.maximum.read(carrier = repcap.Carrier.Default) \n
+		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:SDEViation \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.standardDev.read(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:MAXimum?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:SDEViation?', self.__class__.ResultData())
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:MAXimum \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.maximum.fetch(carrier = repcap.Carrier.Default) \n
+		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:SDEViation \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.standardDev.fetch(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:MAXimum?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:SDEViation?', self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/Average.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from ......Internal.StructBase import StructBase
 from ......Internal.ArgStruct import ArgStruct
 from ...... import enums
 from ...... import repcap
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class StandardDevCls:
-	"""StandardDev commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
+class AverageCls:
+	"""Average commands group definition. 3 total commands, 0 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("standardDev", core, parent)
+		self._cmd_group = CommandsGroup("average", core, parent)
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value
-			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float or bool: Magnitude error RMS value
-			- Mag_Error_Peak: float or bool: Magnitude error peak value
+			- Evm_Rms: float or bool: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float or bool: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float or bool: Magnitude error RMS value.
+			- Mag_Error_Peak: float or bool: Magnitude error peak value.
 			- Phase_Error_Rms: float or bool: No parameter help available
 			- Phase_Error_Peak: float or bool: No parameter help available
-			- Iq_Offset: float or bool: I/Q origin offset
-			- Iq_Imbalance: float or bool: I/Q imbalance
+			- Iq_Offset: float or bool: I/Q origin offset.
+			- Iq_Imbalance: float or bool: I/Q imbalance.
 			- Carrier_Freq_Err: float or bool: No parameter help available
 			- Transmit_Time_Err: float or bool: No parameter help available
-			- Ue_Power: float or bool: User equipment power
-			- Power_Steps: float or bool: User equipment power step
-			- Phase_Disc: enums.ResultStatus2: Phase discontinuity"""
+			- Ue_Power: float or bool: User equipment power.
+			- Power_Steps: float or bool: User equipment power step.
+			- Phase_Disc: enums.ResultStatus2: Phase discontinuity."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Evm_Rms'),
 			ArgStruct.scalar_float_ext('Evm_Peak'),
 			ArgStruct.scalar_float_ext('Mag_Error_Rms'),
 			ArgStruct.scalar_float_ext('Mag_Error_Peak'),
 			ArgStruct.scalar_float_ext('Phase_Error_Rms'),
@@ -61,41 +61,41 @@
 			self.Carrier_Freq_Err: float or bool = None
 			self.Transmit_Time_Err: float or bool = None
 			self.Ue_Power: float or bool = None
 			self.Power_Steps: float or bool = None
 			self.Phase_Disc: enums.ResultStatus2 = None
 
 	def calculate(self, carrier=repcap.Carrier.Default) -> CalculateStruct:
-		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:SDEViation \n
-		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.standardDev.calculate(carrier = repcap.Carrier.Default) \n
+		"""SCPI: CALCulate:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:AVERage \n
+		Snippet: value: CalculateStruct = driver.wcdmaMeas.multiEval.carrier.modulation.average.calculate(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for CalculateStruct structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:SDEViation?', self.__class__.CalculateStruct())
+		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:AVERage?', self.__class__.CalculateStruct())
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Evm_Rms: float: Error vector magnitude RMS and peak value
-			- Evm_Peak: float: Error vector magnitude RMS and peak value
-			- Mag_Error_Rms: float: Magnitude error RMS value
-			- Mag_Error_Peak: float: Magnitude error peak value
+			- Evm_Rms: float: Error vector magnitude RMS and peak value.
+			- Evm_Peak: float: Error vector magnitude RMS and peak value.
+			- Mag_Error_Rms: float: Magnitude error RMS value.
+			- Mag_Error_Peak: float: Magnitude error peak value.
 			- Phase_Error_Rms: float: No parameter help available
 			- Phase_Error_Peak: float: No parameter help available
-			- Iq_Offset: float: I/Q origin offset
-			- Iq_Imbalance: float: I/Q imbalance
+			- Iq_Offset: float: I/Q origin offset.
+			- Iq_Imbalance: float: I/Q imbalance.
 			- Carrier_Freq_Err: float: No parameter help available
 			- Transmit_Time_Err: float: No parameter help available
-			- Ue_Power: float: User equipment power
-			- Power_Steps: float: User equipment power step
-			- Phase_Disc: float: Phase discontinuity
+			- Ue_Power: float: User equipment power.
+			- Power_Steps: float: User equipment power step.
+			- Phase_Disc: float: Phase discontinuity.
 			- Tx_Time_Alignment: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Evm_Rms'),
 			ArgStruct.scalar_float('Evm_Peak'),
 			ArgStruct.scalar_float('Mag_Error_Rms'),
 			ArgStruct.scalar_float('Mag_Error_Peak'),
@@ -124,28 +124,28 @@
 			self.Carrier_Freq_Err: float = None
 			self.Transmit_Time_Err: float = None
 			self.Ue_Power: float = None
 			self.Power_Steps: float = None
 			self.Phase_Disc: float = None
 			self.Tx_Time_Alignment: float = None
 
-	def read(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:SDEViation \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.standardDev.read(carrier = repcap.Carrier.Default) \n
+	def fetch(self, carrier=repcap.Carrier.Default) -> ResultData:
+		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:AVERage \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.average.fetch(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:SDEViation?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:AVERage?', self.__class__.ResultData())
 
-	def fetch(self, carrier=repcap.Carrier.Default) -> ResultData:
-		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:SDEViation \n
-		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.standardDev.fetch(carrier = repcap.Carrier.Default) \n
+	def read(self, carrier=repcap.Carrier.Default) -> ResultData:
+		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:MODulation:AVERage \n
+		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.carrier.modulation.average.read(carrier = repcap.Carrier.Default) \n
 		Return the current, average, maximum and standard deviation single value results. The return values described below are
 		returned by FETCh and READ commands. CALCulate commands return limit check results instead, one value for each of the
 		first 14 results listed below. The TX time alignment is only returned by FETCh and READ commands. \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
-		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:SDEViation?', self.__class__.ResultData())
+		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:MODulation:AVERage?', self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/OcInfo.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/OcInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("ocInfo", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- State: List[enums.State]: State of the channel OFF: Channel off since start of measurement VAR: Channel has been on and off ON: Channel on since start of measurement
-			- Spreading_Factor: List[enums.SpreadingFactorB]: Spreading factor of the channel 2 | 4 | 8 | 16 | 32 | 64 | 128 | 256: constant spreading factor V2 | V4 | V8 | V16 | V32 | V64 | V128 | V256: varying spreading factor, indicates smallest occurred value
-			- Modulation: List[enums.Modulation]: Modulation type of the channel BPSK: Constantly BPSK modulated 4PAM: Constantly 4PAM modulated 4PVar: BPSK and 4PAM occurred"""
+			- State: List[enums.State]: State of the channel OFF: Channel off since start of measurement VAR: The channel has been on and off. ON: Channel on since start of measurement
+			- Spreading_Factor: List[enums.SpreadingFactorB]: Spreading factor of the channel 2 | 4 | 8 | 16 | 32 | 64 | 128 | 256: constant spreading factor V2 | V4 | V8 | V16 | V32 | V64 | V128 | V256: varying spreading factor, indicates the smallest occurred value
+			- Modulation: List[enums.Modulation]: Modulation format of the channel BPSK: Constantly BPSK modulated 4PAM: Constantly 4PAM modulated 4PVar: BPSK and 4PAM occurred"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct('State', DataType.EnumList, enums.State, False, True, 1),
 			ArgStruct('Spreading_Factor', DataType.EnumList, enums.SpreadingFactorB, False, True, 1),
 			ArgStruct('Modulation', DataType.EnumList, enums.Modulation, False, True, 1)]
 
 		def __init__(self):
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Sf.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/Sf.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/RcdError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Average.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPCCh:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPCCh:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPCCh:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/StandardDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPCCh:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPCCh:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Average.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPDCh:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPDCh:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPDCh:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/StandardDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:DPDCh:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:DPDCh:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Dpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Average.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:EDPCch:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:EDPCch:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/Maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:EDPCch:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/StandardDev.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:EDPCch:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:EDPCch:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Edpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Average.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:HSDPcch:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:HSDPcch:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/Maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:HSDPcch:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/StandardDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDERror:HSDPcch:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDERror:HSDPcch:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/Hsdpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Dpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Average.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:EDPCch:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:EDPCch:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:EDPCch:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/Minimum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:MINimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:EDPCch:MINimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:MINimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/StandardDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:EDPCch:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: edpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:EDPCch:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Edpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Average.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:HSDPcch:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:HSDPcch:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:HSDPcch:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/Minimum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:MINimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:HSDPcch:MINimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:MINimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/StandardDev.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:CDPower:HSDPcch:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the RMS CDP vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, minimum, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: RMS CDP trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:CDPower:HSDPcch:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/Hsdpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/CdPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Sdeviaton.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/Sdeviaton.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Sdeviaton.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/Sdeviaton.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/EvMagnitude/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/FreqError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Merror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Perror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/Psteps/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Average.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPCCh:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPCCh:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPCCh:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/StandardDev.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:SDEViation?', suppressed)
 		return response
 
 	def read(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPCCh:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPCCh:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Average.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPDCh:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPDCh:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/Maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPDCh:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/StandardDev.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:DPDCh:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the DPCCH and the DPDCH. Each current value is averaged over a
 		half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.
 		Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.
 		WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can be
 		retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: dpdch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:DPDCh:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Dpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Average.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:EDPCch:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:EDPCch:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/Maximum.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:EDPCch:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/StandardDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:EDPCch:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: edpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:EDPCch:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Edpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Average.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:AVERage?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:HSDPcch:AVERage \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:AVERage?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Current.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:CURRent?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:HSDPcch:CURRent \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/Maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:MAXimum?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:HSDPcch:MAXimum \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:MAXimum?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/StandardDev.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:SDEViation?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:HSDPcch:SDEViation \n
@@ -37,12 +37,12 @@
 		Returns the values of the relative CDE vs slot traces for the HS-DPCCH and the E-DPCCH. Each current value is averaged
 		over a half-slot or a full-slot, depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.
 		MultiEval.Mperiod.modulation) . The number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.msCount) . The results of the current, average, maximum and standard deviation traces can
 		be retrieved. The standard deviation traces cannot be displayed at the GUI. \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot"""
+			:return: hsdpcch: Relative CDE trace results, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:HSDPcch:SDEViation?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Hsdpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpcch.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:DPCCh \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.dpcch.fetch(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the DPCCH and the DPDCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) .
 		The number of results depends on the measurement length (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Spreading factors, one result per measured slot or half-slot"""
+			:return: dpcch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:DPCCh?', suppressed)
 		return response
 
 	def read(self, carrier=repcap.Carrier.Default) -> List[int]:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:DPCCh \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.dpcch.read(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the DPCCH and the DPDCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) .
 		The number of results depends on the measurement length (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpcch: Spreading factors, one result per measured slot or half-slot"""
+			:return: dpcch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:DPCCh?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpdch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Dpdch.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:DPDCh \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.dpdch.read(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the DPCCH and the DPDCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) .
 		The number of results depends on the measurement length (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Spreading factors, one result per measured slot or half-slot"""
+			:return: dpdch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:DPDCh?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[int]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:DPDCh \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.dpdch.fetch(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the DPCCH and the DPDCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) .
 		The number of results depends on the measurement length (method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: dpdch: Spreading factors, one result per measured slot or half-slot"""
+			:return: dpdch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:DPDCh?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpcch.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:EDPCch \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.edpcch.read(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the E-DPCCH and the HS-DPCCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) . The
 		number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Spreading factors, one result per measured slot or half-slot"""
+			:return: edpcch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:EDPCch?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[int]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:EDPCch \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.edpcch.fetch(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the E-DPCCH and the HS-DPCCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) . The
 		number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: edpcch: Spreading factors, one result per measured slot or half-slot"""
+			:return: edpcch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:EDPCch?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpdch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Edpdch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Hsdpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/Hsdpcch.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:HSDPcch \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.hsdpcch.read(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the E-DPCCH and the HS-DPCCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) . The
 		number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Spreading factors, one result per measured slot or half-slot"""
+			:return: hsdpcch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:HSDPcch?', suppressed)
 		return response
 
 	def fetch(self, carrier=repcap.Carrier.Default) -> List[int]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:CARRier<carrier>:TRACe:RCDerror:SF:HSDPcch \n
 		Snippet: value: List[int] = driver.wcdmaMeas.multiEval.carrier.trace.rcdError.sf.hsdpcch.fetch(carrier = repcap.Carrier.Default) \n
 		Returns the current spreading factors for the E-DPCCH and the HS-DPCCH. Each value refers to a half-slot or a full-slot,
 		depending on the measurement period (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.Mperiod.modulation) . The
 		number of results depends on the measurement length (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.MultiEval.msCount) . \n
 		Suppressed linked return values: reliability \n
 			:param carrier: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Carrier')
-			:return: hsdpcch: Spreading factors, one result per measured slot or half-slot"""
+			:return: hsdpcch: Spreading factors, one result per measured slot or half-slot."""
 		carrier_cmd_val = self._cmd_group.get_repcap_cmd_value(carrier, repcap.Carrier)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_int_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:CARRier{carrier_cmd_val}:TRACe:RCDerror:SF:HSDPcch?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/Sf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/RcdError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Dpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Edpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Hsdpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Dpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Edpdch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Hsdpcch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/CdPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Evm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/FreqError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqImbalance/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/IqOffset/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Merror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/Perror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/TtError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Code/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Current.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		self._cmd_group = CommandsGroup("current", core, parent)
 
 	# noinspection PyTypeChecker
 	class FetchStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator' In list mode, a zero reliability indicator indicates that the results in all measured segments are valid. A non-zero value indicates that an error occurred in at least one of the measured segments.
 			- Return_Code: List[int]: Reliability indicator for the segment. The meaning of the returned values is the same as for the common reliability indicator, see previous parameter.
-			- Pcd_Error: List[float]: Peak code domain error
+			- Pcd_Error: List[float]: Peak code domain error.
 			- Pcd_Error_Phase: List[enums.PcdErrorPhase]: No parameter help available
 			- Pcd_Error_Code_Nr: List[int]: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct('Return_Code', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Pcd_Error', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Pcd_Error_Phase', DataType.EnumList, enums.PcdErrorPhase, False, True, 1),
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Error/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	# noinspection PyTypeChecker
 	class FetchStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator' In list mode, a zero reliability indicator indicates that the results in all measured segments are valid. A non-zero value indicates that an error occurred in at least one of the measured segments.
 			- Return_Code: List[int]: Reliability indicator for the segment. The meaning of the returned values is the same as for the common reliability indicator, see previous parameter.
-			- Pcd_Error: List[float]: Peak code domain error
+			- Pcd_Error: List[float]: Peak code domain error.
 			- Pcd_Error_Phase: List[enums.PcdErrorPhase]: No parameter help available
 			- Pcd_Error_Code_Nr: List[int]: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct('Return_Code', DataType.IntegerList, None, False, True, 1),
 			ArgStruct('Pcd_Error', DataType.FloatList, None, False, True, 1),
 			ArgStruct('Pcd_Error_Phase', DataType.EnumList, enums.PcdErrorPhase, False, True, 1),
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/Phase/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Pcde/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Phd/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/CdPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Pcde/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Phd/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Average.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,13 +82,13 @@
 			self.Emask_Margin_Had: float = None
 			self.Emask_Margin_Hda: float = None
 
 	def fetch(self, aclr_mode: enums.AclrMode = None, segment=repcap.Segment.Default) -> FetchStruct:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SEGMent<nr>:SPECtrum:AVERage \n
 		Snippet: value: FetchStruct = driver.wcdmaMeas.multiEval.listPy.segment.spectrum.average.fetch(aclr_mode = enums.AclrMode.ABSolute, segment = repcap.Segment.Default) \n
 		Returns the ACLR power and spectrum emission single value results for segment <no> in list mode. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 			:return: structure: for return value, see the help for FetchStruct structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:SPECtrum:AVERage? {param}'.rstrip(), self.__class__.FetchStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Current.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,13 @@
 			self.Emask_Margin_Had: float = None
 			self.Emask_Margin_Hda: float = None
 
 	def fetch(self, aclr_mode: enums.AclrMode = None, segment=repcap.Segment.Default) -> FetchStruct:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SEGMent<nr>:SPECtrum:CURRent \n
 		Snippet: value: FetchStruct = driver.wcdmaMeas.multiEval.listPy.segment.spectrum.current.fetch(aclr_mode = enums.AclrMode.ABSolute, segment = repcap.Segment.Default) \n
 		Returns the ACLR power and spectrum emission single value results for segment <no> in list mode. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 			:return: structure: for return value, see the help for FetchStruct structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:SPECtrum:CURRent? {param}'.rstrip(), self.__class__.FetchStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,13 +82,13 @@
 			self.Emask_Margin_Had: float = None
 			self.Emask_Margin_Hda: float = None
 
 	def fetch(self, aclr_mode: enums.AclrMode = None, segment=repcap.Segment.Default) -> FetchStruct:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SEGMent<nr>:SPECtrum:MAXimum \n
 		Snippet: value: FetchStruct = driver.wcdmaMeas.multiEval.listPy.segment.spectrum.maximum.fetch(aclr_mode = enums.AclrMode.ABSolute, segment = repcap.Segment.Default) \n
 		Returns the ACLR power and spectrum emission single value results for segment <no> in list mode. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param segment: optional repeated capability selector. Default value: Nr1 (settable in the interface 'Segment')
 			:return: structure: for return value, see the help for FetchStruct structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		segment_cmd_val = self._cmd_group.get_repcap_cmd_value(segment, repcap.Segment)
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SEGMent{segment_cmd_val}:SPECtrum:MAXimum? {param}'.rstrip(), self.__class__.FetchStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Segment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Average.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:ACLR:M<nr>:AVERage \n
 		Snippet: value: List[float] = driver.wcdmaMeas.multiEval.listPy.spectrum.aclr.m.average.fetch(aclr_mode = enums.AclrMode.ABSolute, minus = repcap.Minus.Default) \n
 		Return the power of the adjacent channels for all measured list mode segments.
 			INTRO_CMD_HELP: The adjacent channel selected via M<no>/P<no> is at the following frequency relative to the carrier frequency: \n
 			- M1 = -5 MHz, M2 = -10 MHz
 			- P1 = +5 MHz, P2 = +10 MHz  \n
 		Suppressed linked return values: reliability \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param minus: optional repeated capability selector. Default value: Ch1 (settable in the interface 'M')
 			:return: aclr: Comma-separated list of values, one per measured segment"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		minus_cmd_val = self._cmd_group.get_repcap_cmd_value(minus, repcap.Minus)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:ACLR:M{minus_cmd_val}:AVERage? {param}'.rstrip(), suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Current.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:ACLR:M<nr>:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.multiEval.listPy.spectrum.aclr.m.current.fetch(aclr_mode = enums.AclrMode.ABSolute, minus = repcap.Minus.Default) \n
 		Return the power of the adjacent channels for all measured list mode segments.
 			INTRO_CMD_HELP: The adjacent channel selected via M<no>/P<no> is at the following frequency relative to the carrier frequency: \n
 			- M1 = -5 MHz, M2 = -10 MHz
 			- P1 = +5 MHz, P2 = +10 MHz  \n
 		Suppressed linked return values: reliability \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param minus: optional repeated capability selector. Default value: Ch1 (settable in the interface 'M')
 			:return: aclr: Comma-separated list of values, one per measured segment"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		minus_cmd_val = self._cmd_group.get_repcap_cmd_value(minus, repcap.Minus)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:ACLR:M{minus_cmd_val}:CURRent? {param}'.rstrip(), suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:ACLR:M<nr>:MAXimum \n
 		Snippet: value: List[float] = driver.wcdmaMeas.multiEval.listPy.spectrum.aclr.m.maximum.fetch(aclr_mode = enums.AclrMode.ABSolute, minus = repcap.Minus.Default) \n
 		Return the power of the adjacent channels for all measured list mode segments.
 			INTRO_CMD_HELP: The adjacent channel selected via M<no>/P<no> is at the following frequency relative to the carrier frequency: \n
 			- M1 = -5 MHz, M2 = -10 MHz
 			- P1 = +5 MHz, P2 = +10 MHz  \n
 		Suppressed linked return values: reliability \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param minus: optional repeated capability selector. Default value: Ch1 (settable in the interface 'M')
 			:return: aclr: Comma-separated list of values, one per measured segment"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		minus_cmd_val = self._cmd_group.get_repcap_cmd_value(minus, repcap.Minus)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:ACLR:M{minus_cmd_val}:MAXimum? {param}'.rstrip(), suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/M/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Average.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:ACLR:P<nr>:AVERage \n
 		Snippet: value: List[float] = driver.wcdmaMeas.multiEval.listPy.spectrum.aclr.p.average.fetch(aclr_mode = enums.AclrMode.ABSolute, plus = repcap.Plus.Default) \n
 		Return the power of the adjacent channels for all measured list mode segments.
 			INTRO_CMD_HELP: The adjacent channel selected via M<no>/P<no> is at the following frequency relative to the carrier frequency: \n
 			- M1 = -5 MHz, M2 = -10 MHz
 			- P1 = +5 MHz, P2 = +10 MHz  \n
 		Suppressed linked return values: reliability \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param plus: optional repeated capability selector. Default value: Ch1 (settable in the interface 'P')
 			:return: aclr: Comma-separated list of values, one per measured segment"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		plus_cmd_val = self._cmd_group.get_repcap_cmd_value(plus, repcap.Plus)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:ACLR:P{plus_cmd_val}:AVERage? {param}'.rstrip(), suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Current.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:ACLR:P<nr>:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.multiEval.listPy.spectrum.aclr.p.current.fetch(aclr_mode = enums.AclrMode.ABSolute, plus = repcap.Plus.Default) \n
 		Return the power of the adjacent channels for all measured list mode segments.
 			INTRO_CMD_HELP: The adjacent channel selected via M<no>/P<no> is at the following frequency relative to the carrier frequency: \n
 			- M1 = -5 MHz, M2 = -10 MHz
 			- P1 = +5 MHz, P2 = +10 MHz  \n
 		Suppressed linked return values: reliability \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param plus: optional repeated capability selector. Default value: Ch1 (settable in the interface 'P')
 			:return: aclr: Comma-separated list of values, one per measured segment"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		plus_cmd_val = self._cmd_group.get_repcap_cmd_value(plus, repcap.Plus)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:ACLR:P{plus_cmd_val}:CURRent? {param}'.rstrip(), suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:ACLR:P<nr>:MAXimum \n
 		Snippet: value: List[float] = driver.wcdmaMeas.multiEval.listPy.spectrum.aclr.p.maximum.fetch(aclr_mode = enums.AclrMode.ABSolute, plus = repcap.Plus.Default) \n
 		Return the power of the adjacent channels for all measured list mode segments.
 			INTRO_CMD_HELP: The adjacent channel selected via M<no>/P<no> is at the following frequency relative to the carrier frequency: \n
 			- M1 = -5 MHz, M2 = -10 MHz
 			- P1 = +5 MHz, P2 = +10 MHz  \n
 		Suppressed linked return values: reliability \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:param plus: optional repeated capability selector. Default value: Ch1 (settable in the interface 'P')
 			:return: aclr: Comma-separated list of values, one per measured segment"""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		plus_cmd_val = self._cmd_group.get_repcap_cmd_value(plus, repcap.Plus)
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:ACLR:P{plus_cmd_val}:MAXimum? {param}'.rstrip(), suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/P/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Aclr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Average.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,11 +85,11 @@
 
 	def fetch(self, aclr_mode: enums.AclrMode = None) -> FetchStruct:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:AVERage \n
 		Snippet: value: FetchStruct = driver.wcdmaMeas.multiEval.listPy.spectrum.average.fetch(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results in list mode. The values listed below in curly brackets
 		{} are returned for the segments {...}seg 1, {...}seg 2, ..., {...}seg n, with n determined by method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.ListPy.count. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for FetchStruct structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:AVERage? {param}'.rstrip(), self.__class__.FetchStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Cpower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Current.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,11 +85,11 @@
 
 	def fetch(self, aclr_mode: enums.AclrMode = None) -> FetchStruct:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:CURRent \n
 		Snippet: value: FetchStruct = driver.wcdmaMeas.multiEval.listPy.spectrum.current.fetch(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results in list mode. The values listed below in curly brackets
 		{} are returned for the segments {...}seg 1, {...}seg 2, ..., {...}seg n, with n determined by method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.ListPy.count. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for FetchStruct structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:CURRent? {param}'.rstrip(), self.__class__.FetchStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ab/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ba/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Bc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Cd/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Dc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Ef/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Fe/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Had/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/Hda/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Emask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Maximum.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,11 +85,11 @@
 
 	def fetch(self, aclr_mode: enums.AclrMode = None) -> FetchStruct:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:LIST:SPECtrum:MAXimum \n
 		Snippet: value: FetchStruct = driver.wcdmaMeas.multiEval.listPy.spectrum.maximum.fetch(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results in list mode. The values listed below in curly brackets
 		{} are returned for the segments {...}seg 1, {...}seg 2, ..., {...}seg n, with n determined by method RsCMPX_WcdmaMeas.
 		Configure.WcdmaMeas.MultiEval.ListPy.count. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for FetchStruct structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:LIST:SPECtrum:MAXimum? {param}'.rstrip(), self.__class__.FetchStruct())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/Obw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Sreliability.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/Sreliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/PhDhsDpcch.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/PhDhsDpcch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/Uephd.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/Uephd.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 		self._cmd_group = CommandsGroup("uephd", core, parent)
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Overall_Max_Ph_D: float or bool: Overall maximum phase discontinuity
-			- Overall_Min_Dist: float or bool: Overall minimum slot distance between two results exceeding the dynamic limit
+			- Overall_Min_Dist: float or bool: The overall minimum slot distance between the two results exceeding the dynamic limit
 			- Count_Upper_Limit: float or bool: Number of results exceeding the upper limit
-			- Count_Dyn_Limit: float or bool: Number of results exceeding the dynamic limit"""
+			- Count_Dyn_Limit: float or bool: The number of results exceeding the dynamic limit"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Overall_Max_Ph_D'),
 			ArgStruct.scalar_float_ext('Overall_Min_Dist'),
 			ArgStruct.scalar_float_ext('Count_Upper_Limit'),
 			ArgStruct.scalar_float_ext('Count_Dyn_Limit')]
 
@@ -46,17 +46,17 @@
 		return self._core.io.query_struct(f'CALCulate:WCDMa:MEASurement<Instance>:MEValuation:MODulation:UEPHd?', self.__class__.CalculateStruct())
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Overall_Max_Ph_D: float: Overall maximum phase discontinuity
-			- Overall_Min_Dist: int: Overall minimum slot distance between two results exceeding the dynamic limit
+			- Overall_Min_Dist: int: The overall minimum slot distance between the two results exceeding the dynamic limit
 			- Count_Upper_Limit: int: Number of results exceeding the upper limit
-			- Count_Dyn_Limit: int: Number of results exceeding the dynamic limit"""
+			- Count_Dyn_Limit: int: The number of results exceeding the dynamic limit"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Overall_Max_Ph_D'),
 			ArgStruct.scalar_int('Overall_Min_Dist'),
 			ArgStruct.scalar_int('Count_Upper_Limit'),
 			ArgStruct.scalar_int('Count_Dyn_Limit')]
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Modulation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 		self._cmd_group = CommandsGroup("current", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Pcd_Error: float: Peak code domain error
-			- Pcd_Error_Phase: enums.PcdErrorPhase: Phase where the peak code domain error was measured IPHase: I-Signal QPHase: Q-Signal
-			- Pcd_Error_Code_Nr: int: Code number for which the PCDE was measured"""
+			- Pcd_Error_Phase: enums.PcdErrorPhase: Phase where the peak code domain error was measured. IPHase: I-Signal QPHase: Q-Signal
+			- Pcd_Error_Code_Nr: int: Code number for which the PCDE was measured."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Pcd_Error'),
 			ArgStruct.scalar_enum('Pcd_Error_Phase', enums.PcdErrorPhase),
 			ArgStruct.scalar_int('Pcd_Error_Code_Nr')]
 
 		def __init__(self):
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/Maximum.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Pcd_Error: float: Peak code domain error
-			- Pcd_Error_Phase: enums.PcdErrorPhase: Phase where the peak code domain error was measured IPHase: I-Signal QPHase: Q-Signal
-			- Pcd_Error_Code_Nr: int: Code number for which the PCDE was measured"""
+			- Pcd_Error_Phase: enums.PcdErrorPhase: Phase where the peak code domain error was measured. IPHase: I-Signal QPHase: Q-Signal
+			- Pcd_Error_Code_Nr: int: Code number for which the PCDE was measured."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Pcd_Error'),
 			ArgStruct.scalar_enum('Pcd_Error_Phase', enums.PcdErrorPhase),
 			ArgStruct.scalar_int('Pcd_Error_Code_Nr')]
 
 		def __init__(self):
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Pcde/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Average.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,23 +195,23 @@
 	def fetch(self, aclr_mode: enums.AclrMode = None) -> ResultData:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:SPECtrum:AVERage \n
 		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.spectrum.average.fetch(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results of the multi-evaluation measurement. The current,
 		average and maximum values can be retrieved. The return values described below are returned by FETCh and READ commands.
 		CALCulate commands return limit check results instead, one value for each of the results 1 to 18, 29 and 30 listed below.
 		The frequency positions are only returned by FETCh and READ commands. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:SPECtrum:AVERage? {param}'.rstrip(), self.__class__.ResultData())
 
 	def read(self, aclr_mode: enums.AclrMode = None) -> ResultData:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:SPECtrum:AVERage \n
 		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.spectrum.average.read(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results of the multi-evaluation measurement. The current,
 		average and maximum values can be retrieved. The return values described below are returned by FETCh and READ commands.
 		CALCulate commands return limit check results instead, one value for each of the results 1 to 18, 29 and 30 listed below.
 		The frequency positions are only returned by FETCh and READ commands. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:SPECtrum:AVERage? {param}'.rstrip(), self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,23 +195,23 @@
 	def fetch(self, aclr_mode: enums.AclrMode = None) -> ResultData:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:SPECtrum:CURRent \n
 		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.spectrum.current.fetch(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results of the multi-evaluation measurement. The current,
 		average and maximum values can be retrieved. The return values described below are returned by FETCh and READ commands.
 		CALCulate commands return limit check results instead, one value for each of the results 1 to 18, 29 and 30 listed below.
 		The frequency positions are only returned by FETCh and READ commands. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:SPECtrum:CURRent? {param}'.rstrip(), self.__class__.ResultData())
 
 	def read(self, aclr_mode: enums.AclrMode = None) -> ResultData:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:SPECtrum:CURRent \n
 		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.spectrum.current.read(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results of the multi-evaluation measurement. The current,
 		average and maximum values can be retrieved. The return values described below are returned by FETCh and READ commands.
 		CALCulate commands return limit check results instead, one value for each of the results 1 to 18, 29 and 30 listed below.
 		The frequency positions are only returned by FETCh and READ commands. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:SPECtrum:CURRent? {param}'.rstrip(), self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/Maximum.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,23 +195,23 @@
 	def fetch(self, aclr_mode: enums.AclrMode = None) -> ResultData:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:MEValuation:SPECtrum:MAXimum \n
 		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.spectrum.maximum.fetch(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results of the multi-evaluation measurement. The current,
 		average and maximum values can be retrieved. The return values described below are returned by FETCh and READ commands.
 		CALCulate commands return limit check results instead, one value for each of the results 1 to 18, 29 and 30 listed below.
 		The frequency positions are only returned by FETCh and READ commands. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:MEValuation:SPECtrum:MAXimum? {param}'.rstrip(), self.__class__.ResultData())
 
 	def read(self, aclr_mode: enums.AclrMode = None) -> ResultData:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:MEValuation:SPECtrum:MAXimum \n
 		Snippet: value: ResultData = driver.wcdmaMeas.multiEval.spectrum.maximum.read(aclr_mode = enums.AclrMode.ABSolute) \n
 		Returns the ACLR power and spectrum emission single value results of the multi-evaluation measurement. The current,
 		average and maximum values can be retrieved. The return values described below are returned by FETCh and READ commands.
 		CALCulate commands return limit check results instead, one value for each of the results 1 to 18, 29 and 30 listed below.
 		The frequency positions are only returned by FETCh and READ commands. \n
-			:param aclr_mode: ABSolute: ACLR power displayed in dBm as absolute value RELative: ACLR power displayed in dB relative to carrier power
+			:param aclr_mode: ABSolute: ACLR power is displayed in dBm as an absolute value. RELative: ACLR power is displayed in dB relative to carrier power.
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		param = ArgSingleList().compose_cmd_string(ArgSingle('aclr_mode', aclr_mode, DataType.Enum, enums.AclrMode, is_optional=True))
 		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:MEValuation:SPECtrum:MAXimum? {param}'.rstrip(), self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/All.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/Perror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Isignal/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/Qsignal/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdeMonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Isignal/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/Qsignal/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/CdpMonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfLeft/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/HkfRight/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/Kfilter/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfLeft/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/MfRight/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Emask/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/Chip/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/EvMagnitude/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Iq/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/Chip/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Merror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/Chip/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Perror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/Phd/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/MultiEval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,37 +73,37 @@
 			from .ListPy import ListPyCls
 			self._listPy = ListPyCls(self._core, self._cmd_group)
 		return self._listPy
 
 	def stop(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:WCDMa:MEASurement<instance>:MEValuation \n
 		Snippet: driver.wcdmaMeas.multiEval.stop() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'STOP:WCDMa:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
 	def abort(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:WCDMa:MEASurement<instance>:MEValuation \n
 		Snippet: driver.wcdmaMeas.multiEval.abort() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'ABORt:WCDMa:MEASurement<Instance>:MEValuation', opc_timeout_ms)
 
 	def initiate(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:WCDMa:MEASurement<instance>:MEValuation \n
 		Snippet: driver.wcdmaMeas.multiEval.initiate() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'INITiate:WCDMa:MEASurement<Instance>:MEValuation', opc_timeout_ms)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/Rup.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/Rup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/UepPower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/All.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OlpControl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/All.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/OoSync/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/OffPower.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/OffPower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/Current.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 		self._cmd_group = CommandsGroup("current", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
 			- Ue_Power: float: Mean preamble power
-			- Power_Steps: float: Mean preamble power minus mean power of previous preamble For first preamble NCAP is returned.
+			- Power_Steps: float: Mean preamble power minus mean power of previous preamble For the first preamble, NCAP is returned.
 			- Carrier_Freq_Err: float: Carrier frequency error
 			- Evm_Rms: float: Error vector magnitude RMS value
 			- Evm_Peak: float: Error vector magnitude peak value
 			- Mag_Error_Rms: float: Magnitude error RMS value
 			- Mag_Error_Peak: float: Magnitude error peak value
 			- Phase_Error_Rms: float: No parameter help available
 			- Phase_Error_Peak: float: No parameter help available
@@ -78,15 +78,15 @@
 		preamble_cmd_val = self._cmd_group.get_repcap_cmd_value(preamble, repcap.Preamble)
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:PRACh:PREamble{preamble_cmd_val}:CURRent?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Ue_Power: float or bool: Mean preamble power
-			- Power_Steps: float or bool: Mean preamble power minus mean power of previous preamble For first preamble NCAP is returned.
+			- Power_Steps: float or bool: Mean preamble power minus mean power of previous preamble For the first preamble, NCAP is returned.
 			- Carrier_Freq_Err: float or bool: Carrier frequency error
 			- Evm_Rms: float or bool: Error vector magnitude RMS value
 			- Evm_Peak: float or bool: Error vector magnitude peak value
 			- Mag_Error_Rms: float or bool: Magnitude error RMS value
 			- Mag_Error_Peak: float or bool: Magnitude error peak value
 			- Phase_Error_Rms: float or bool: No parameter help available
 			- Phase_Error_Peak: float or bool: No parameter help available
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Preamble/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/All.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Chip/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/EvMagnitude/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/Current.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("current", core, parent)
 
 	def read(self) -> List[float]:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:PRACh:TRACe:FERRor:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.prach.trace.freqError.current.read() \n
-		Return the values of the frequency error bar graph. \n
+		Return the bargraph values of the frequency error. \n
 		Suppressed linked return values: reliability \n
 			:return: frequency_error: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble)"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:PRACh:TRACe:FERRor:CURRent?', suppressed)
 		return response
 
 	def fetch(self) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:PRACh:TRACe:FERRor:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.prach.trace.freqError.current.fetch() \n
-		Return the values of the frequency error bar graph. \n
+		Return the bargraph values of the frequency error. \n
 		Suppressed linked return values: reliability \n
 			:return: frequency_error: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble)"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:PRACh:TRACe:FERRor:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/FreqError/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Iq/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Chip/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Merror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Chip/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Perror/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/Current.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("current", core, parent)
 
 	def read(self) -> List[float]:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:PRACh:TRACe:PSTeps:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.prach.trace.psteps.current.read() \n
-		Return the values of the power steps bar graph. \n
+		Return the bargraph values of the power steps. \n
 		Suppressed linked return values: reliability \n
-			:return: power_steps: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble) For the first preamble NCAP is returned."""
+			:return: power_steps: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble) For the first preamble, NCAP is returned."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:PRACh:TRACe:PSTeps:CURRent?', suppressed)
 		return response
 
 	def fetch(self) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:PRACh:TRACe:PSTeps:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.prach.trace.psteps.current.fetch() \n
-		Return the values of the power steps bar graph. \n
+		Return the bargraph values of the power steps. \n
 		Suppressed linked return values: reliability \n
-			:return: power_steps: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble) For the first preamble NCAP is returned."""
+			:return: power_steps: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble) For the first preamble, NCAP is returned."""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:PRACh:TRACe:PSTeps:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/Psteps/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Chip/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/Current.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("current", core, parent)
 
 	def read(self) -> List[float]:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:PRACh:TRACe:UEPower:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.prach.trace.uePower.current.read() \n
-		Return the values of the UE power bar graph. \n
+		Return the result values of the UE power bargraph. \n
 		Suppressed linked return values: reliability \n
 			:return: ue_power: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble)"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'READ:WCDMa:MEASurement<Instance>:PRACh:TRACe:UEPower:CURRent?', suppressed)
 		return response
 
 	def fetch(self) -> List[float]:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:PRACh:TRACe:UEPower:CURRent \n
 		Snippet: value: List[float] = driver.wcdmaMeas.prach.trace.uePower.current.fetch() \n
-		Return the values of the UE power bar graph. \n
+		Return the result values of the UE power bargraph. \n
 		Suppressed linked return values: reliability \n
 			:return: ue_power: Comma-separated list of values, one result per measured preamble (see method RsCMPX_WcdmaMeas.Configure.WcdmaMeas.Prach.mpreamble)"""
 		suppressed = ArgSingleSuppressed(0, DataType.Integer, False, 1, 'Reliability')
 		response = self._core.io.query_bin_or_ascii_float_list_suppressed(f'FETCh:WCDMa:MEASurement<Instance>:PRACh:TRACe:UEPower:CURRent?', suppressed)
 		return response
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Prach/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,37 +41,37 @@
 			from .Preamble import PreambleCls
 			self._preamble = PreambleCls(self._core, self._cmd_group)
 		return self._preamble
 
 	def stop(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:WCDMa:MEASurement<instance>:PRACh \n
 		Snippet: driver.wcdmaMeas.prach.stop() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'STOP:WCDMa:MEASurement<Instance>:PRACh', opc_timeout_ms)
 
 	def abort(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:WCDMa:MEASurement<instance>:PRACh \n
 		Snippet: driver.wcdmaMeas.prach.abort() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'ABORt:WCDMa:MEASurement<Instance>:PRACh', opc_timeout_ms)
 
 	def initiate(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:WCDMa:MEASurement<instance>:PRACh \n
 		Snippet: driver.wcdmaMeas.prach.initiate() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'INITiate:WCDMa:MEASurement<Instance>:PRACh', opc_timeout_ms)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Statistics.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/Statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 			- Pwr_Steps_B_1_Db: int: No parameter help available
 			- Pwr_Steps_Cm_1_Db: int: No parameter help available
 			- Pwr_Steps_Group_A: int: No parameter help available
 			- Pwr_Steps_Eg: int: No parameter help available
 			- Pwr_Steps_Fh: int: No parameter help available
 			- Pwr_Steps_Group_Eg: int: No parameter help available
 			- Pwr_Steps_Group_Fh: int: No parameter help available
-			- Pwr_Steps_Up: int: Power steps up result of Change of TFC mode
-			- Pwr_Steps_Down: int: Power steps down result of Change of TFC mode
-			- Rpwr_Steps: int: Recovery power steps result of UL Compressed Mode - pattern A
+			- Pwr_Steps_Up: int: Power steps up result of Change of TFC mode.
+			- Pwr_Steps_Down: int: Power steps down result of Change of TFC mode.
+			- Rpwr_Steps: int: Recovery power steps result of UL Compressed Mode - pattern A.
 			- Epwr_Steps_B_1_D_B: int: No parameter help available
 			- Epwr_Steps_Cm_1_D_B: int: No parameter help available
 			- Epwr_Steps_Eg: int: No parameter help available
 			- Epwr_Steps_Fh: int: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_int('Pwr_Steps_0_Db'),
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Psteps/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/Psteps/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Statistics.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/Statistics.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Carrier/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Average.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("average", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Carrier_Ch_Power: float: Level of the uplink carrier, where the UE transmits at the maximal output power
-			- Inband_Emission: float: Relative level of the other uplink carrier transmitting at minimal output power"""
+			- Carrier_Ch_Power: float: Level of the uplink carrier, where the UE transmits at the maximal output power.
+			- Inband_Emission: float: Relative level of the other uplink carrier transmitting at minimal output power."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Carrier_Ch_Power'),
 			ArgStruct.scalar_float('Inband_Emission')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
@@ -47,16 +47,16 @@
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:TPC:DHIB:AVERage?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Carrier_Ch_Power: float or bool: Level of the uplink carrier, where the UE transmits at the maximal output power
-			- Inband_Emission: float or bool: Relative level of the other uplink carrier transmitting at minimal output power"""
+			- Carrier_Ch_Power: float or bool: Level of the uplink carrier, where the UE transmits at the maximal output power.
+			- Inband_Emission: float or bool: Relative level of the other uplink carrier transmitting at minimal output power."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Carrier_Ch_Power'),
 			ArgStruct.scalar_float_ext('Inband_Emission')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Maximum.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("maximum", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Carrier_Ch_Power: float: Level of the uplink carrier, where the UE transmits at the maximal output power
-			- Inband_Emission: float: Relative level of the other uplink carrier transmitting at minimal output power"""
+			- Carrier_Ch_Power: float: Level of the uplink carrier, where the UE transmits at the maximal output power.
+			- Inband_Emission: float: Relative level of the other uplink carrier transmitting at minimal output power."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Carrier_Ch_Power'),
 			ArgStruct.scalar_float('Inband_Emission')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
@@ -47,16 +47,16 @@
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:TPC:DHIB:MAXimum?', self.__class__.ResultData())
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Carrier_Ch_Power: float or bool: Level of the uplink carrier, where the UE transmits at the maximal output power
-			- Inband_Emission: float or bool: Relative level of the other uplink carrier transmitting at minimal output power"""
+			- Carrier_Ch_Power: float or bool: Level of the uplink carrier, where the UE transmits at the maximal output power.
+			- Inband_Emission: float or bool: Relative level of the other uplink carrier transmitting at minimal output power."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Carrier_Ch_Power'),
 			ArgStruct.scalar_float_ext('Inband_Emission')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimum.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("minimum", core, parent)
 
 	# noinspection PyTypeChecker
 	class ResultData(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Carrier_Ch_Power: float: Level of the uplink carrier, where the UE transmits at the maximal output power
-			- Inband_Emission: float: Relative level of the other uplink carrier transmitting at minimal output power"""
+			- Carrier_Ch_Power: float: Level of the uplink carrier, where the UE transmits at the maximal output power.
+			- Inband_Emission: float: Relative level of the other uplink carrier transmitting at minimal output power."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float('Carrier_Ch_Power'),
 			ArgStruct.scalar_float('Inband_Emission')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimumc.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Minimumc.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("minimumc", core, parent)
 
 	# noinspection PyTypeChecker
 	class CalculateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Reliability: int: 'Reliability indicator'
-			- Carrier_Ch_Power: float or bool: Level of the uplink carrier, where the UE transmits at the maximal output power
-			- Inband_Emission: float or bool: Relative level of the other uplink carrier transmitting at minimal output power"""
+			- Carrier_Ch_Power: float or bool: Level of the uplink carrier, where the UE transmits at the maximal output power.
+			- Inband_Emission: float or bool: Relative level of the other uplink carrier transmitting at minimal output power."""
 		__meta_args_list = [
 			ArgStruct.scalar_int('Reliability', 'Reliability'),
 			ArgStruct.scalar_float_ext('Carrier_Ch_Power'),
 			ArgStruct.scalar_float_ext('Inband_Emission')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Statistics.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/Statistics.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Dhib/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/All.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/Current.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/Trace/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Average.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Average.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 			self.Reliability: int = None
 			self.Ue_Power: float = None
 			self.Max_Output_Power: float = None
 
 	def fetch(self) -> ResultData:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:TPC:TOTal:UEPower:AVERage \n
 		Snippet: value: ResultData = driver.wcdmaMeas.tpc.total.uePower.average.fetch() \n
-		Return the UE power and maximum output power single value results over all carriers. The minimum, maximum and average
+		Return the UE power and the maximum output power single value results over all carriers. The minimum, maximum and average
 		values of these results can be retrieved. \n
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:TPC:TOTal:UEPower:AVERage?', self.__class__.ResultData())
 
 	def read(self) -> ResultData:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:TPC:TOTal:UEPower:AVERage \n
 		Snippet: value: ResultData = driver.wcdmaMeas.tpc.total.uePower.average.read() \n
-		Return the UE power and maximum output power single value results over all carriers. The minimum, maximum and average
+		Return the UE power and the maximum output power single value results over all carriers. The minimum, maximum and average
 		values of these results can be retrieved. \n
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:TPC:TOTal:UEPower:AVERage?', self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Maximum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Maximum.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 			self.Reliability: int = None
 			self.Ue_Power: float = None
 			self.Max_Output_Power: float = None
 
 	def fetch(self) -> ResultData:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:TPC:TOTal:UEPower:MAXimum \n
 		Snippet: value: ResultData = driver.wcdmaMeas.tpc.total.uePower.maximum.fetch() \n
-		Return the UE power and maximum output power single value results over all carriers. The minimum, maximum and average
+		Return the UE power and the maximum output power single value results over all carriers. The minimum, maximum and average
 		values of these results can be retrieved. \n
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:TPC:TOTal:UEPower:MAXimum?', self.__class__.ResultData())
 
 	def read(self) -> ResultData:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:TPC:TOTal:UEPower:MAXimum \n
 		Snippet: value: ResultData = driver.wcdmaMeas.tpc.total.uePower.maximum.read() \n
-		Return the UE power and maximum output power single value results over all carriers. The minimum, maximum and average
+		Return the UE power and the maximum output power single value results over all carriers. The minimum, maximum and average
 		values of these results can be retrieved. \n
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:TPC:TOTal:UEPower:MAXimum?', self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Minimum.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Minimum.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 			self.Reliability: int = None
 			self.Ue_Power: float = None
 			self.Max_Output_Power: float = None
 
 	def fetch(self) -> ResultData:
 		"""SCPI: FETCh:WCDMa:MEASurement<instance>:TPC:TOTal:UEPower:MINimum \n
 		Snippet: value: ResultData = driver.wcdmaMeas.tpc.total.uePower.minimum.fetch() \n
-		Return the UE power and maximum output power single value results over all carriers. The minimum, maximum and average
+		Return the UE power and the maximum output power single value results over all carriers. The minimum, maximum and average
 		values of these results can be retrieved. \n
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'FETCh:WCDMa:MEASurement<Instance>:TPC:TOTal:UEPower:MINimum?', self.__class__.ResultData())
 
 	def read(self) -> ResultData:
 		"""SCPI: READ:WCDMa:MEASurement<instance>:TPC:TOTal:UEPower:MINimum \n
 		Snippet: value: ResultData = driver.wcdmaMeas.tpc.total.uePower.minimum.read() \n
-		Return the UE power and maximum output power single value results over all carriers. The minimum, maximum and average
+		Return the UE power and the maximum output power single value results over all carriers. The minimum, maximum and average
 		values of these results can be retrieved. \n
 			:return: structure: for return value, see the help for ResultData structure arguments."""
 		return self._core.io.query_struct(f'READ:WCDMa:MEASurement<Instance>:TPC:TOTal:UEPower:MINimum?', self.__class__.ResultData())
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Statistics.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/Statistics.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/UePower/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/Total/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/Tpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,37 +41,37 @@
 			from .State import StateCls
 			self._state = StateCls(self._core, self._cmd_group)
 		return self._state
 
 	def stop(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: STOP:WCDMa:MEASurement<instance>:TPC \n
 		Snippet: driver.wcdmaMeas.tpc.stop() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'STOP:WCDMa:MEASurement<Instance>:TPC', opc_timeout_ms)
 
 	def abort(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: ABORt:WCDMa:MEASurement<instance>:TPC \n
 		Snippet: driver.wcdmaMeas.tpc.abort() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'ABORt:WCDMa:MEASurement<Instance>:TPC', opc_timeout_ms)
 
 	def initiate(self, opc_timeout_ms: int = -1) -> None:
 		"""SCPI: INITiate:WCDMa:MEASurement<instance>:TPC \n
 		Snippet: driver.wcdmaMeas.tpc.initiate() \n
-			INTRO_CMD_HELP: Starts, stops, or aborts the measurement: \n
+			INTRO_CMD_HELP: Starts, stops or aborts the measurement: \n
 			- INITiate... starts or restarts the measurement. The measurement enters the RUN state.
 			- STOP... halts the measurement immediately. The measurement enters the RDY state. Measurement results are kept. The resources remain allocated to the measurement.
 			- ABORt... halts the measurement immediately. The measurement enters the OFF state. All measurement values are set to NAV. Allocated resources are released.
 		Use FETCh...STATe? to query the current measurement state. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
 		self._core.io.write_with_opc(f'INITiate:WCDMa:MEASurement<Instance>:TPC', opc_timeout_ms)
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Implementations/WcdmaMeas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgLinkedEventArgs.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgLinkedEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgSingle.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgSingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgSingleList.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgSingleList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgSingleSuppressed.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgSingleSuppressed.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStringComposer.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStringComposer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStruct.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStruct.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStructList.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStructList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ArgStructStringParser.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ArgStructStringParser.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/CommandsGroup.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/CommandsGroup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Conversions.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Conversions.py`

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
@@ -198,19 +199,20 @@
 
 
 number_plus_inf_lookup = frozenset(['Inf', 'INF', 'INFINITY', '+Inf', '+INF', '+inf', '+INFINITY', '+Infinity', '+infinity'])
 number_minus_inf_lookup = frozenset(['-Inf', '-INF', '-inf', '-INFINITY', '-Infinity', '-infinity'])
 number_nan_lookup = frozenset(['Nan', 'NAN', 'nan', 'NaN', 'NAV', 'NaV', 'NCAP', 'INV', 'NONE', 'none', 'None', 'DTX', 'UND', 'und'])
 number_max_lookup = frozenset(['OFL', 'ofl', 'Ofl'])
 number_min_lookup = frozenset(['UFL', 'ufl', 'Ufl'])
-number_si_suffix = {'pHz': 1E-12, 'MHz': 1E+6, 'kHz': 1E+3, 'GHz': 1E+9, 'mHz': 1E-3, 'uHz': 1E-6, 'µHz': 1E-6, 'THz': 1E+12, 'nHz': 1E-9, 'ns': 1E-9, 'fW': 1E-15,
-					'pW': 1E-12, 'nW': 1E-9, 'uW': 1E-6, 'µW': 1E-6, 'mW': 1E-3, 'kW': 1E3, 'MW': 1E6, 'GW': 1E9, 'MV': 1E+6, 'MA': 1E+6, 'ps': 1E-12, 'fs': 1E-15,
-					'km': 1E+3, 'kV': 1E+3, 'kA': 1E+3, 'pF': 1E-2, 'Hz': 1.0, 'mm': 1E-3, 'mA': 1E-3, 'mF': 1E-3, 'mV': 1E-3, 'pV': 1E-12, 'nF': 1E-9, 'nA': 1E-9,
-					'nV': 1E-9, 'nm': 1E-9, 'pm': 1E-12, 'us': 1E-6, 'µs': 1E-6, 'uF': 1E-6, 'µF': 1E-6, 'ms': 1E-3, 'uA': 1E-6, 'µA': 1E-6, 'uV': 1E-6, 'µV': 1E-6,
-					'um': 1E-6, 'µm': 1E-6, 'pA': 1E-12, 'V': 1, 'W': 1, 'A': 1, 'F': 1, 's': 1, 'm': 1}
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
@@ -362,15 +364,15 @@
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
@@ -480,15 +482,15 @@
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
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ConverterFromScpiString.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ConverterFromScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ConverterToScpiString.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ConverterToScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Core.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Core.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,40 @@
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
 		1.54.0 (27.06.2023)
 			- Added new options profile for ATS chambers.
 			- Added settings boolean token EachCmdAsQuery. Example: EachCmdAsQuery=True. Default: False
 
 		1.53.0 (18.10.2022)
 			- Improved mode where the instrument works with a session from another object.
 			- Silently ignoring invalid *IDN? string.
@@ -175,15 +187,15 @@
 			reset: bool = False,
 			driver_options: str = None,
 			user_options: str = None,
 			direct_session: object = None):
 		"""Initializes new driver session. For cleaner code, use the class methods: \n
 		- Core.from_existing_session() - initializes a new Core with an existing pyvisa session."""
 
-		self.core_version = '1.54.0'
+		self.core_version = '1.55.0'
 		self.resource_name = resource_name
 
 		# Typical settings for the Core
 		self._instrumentSettings = InstrumentSettings(
 			InstrViClearMode.execute_on_all,  # Instrument viClear mode
 			False,  # Full model name. True: SMW200A, False: SMW
 			0,  # Delay by each write
@@ -193,15 +205,17 @@
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
@@ -212,14 +226,15 @@
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
@@ -275,14 +290,20 @@
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

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/GlobalData.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/GlobalData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Instrument.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,34 @@
 
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
@@ -385,14 +398,24 @@
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
@@ -435,15 +458,16 @@
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
@@ -723,15 +747,16 @@
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
@@ -818,15 +843,16 @@
 
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
@@ -1047,15 +1073,16 @@
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
@@ -1130,15 +1157,16 @@
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

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InstrumentErrors.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InstrumentErrors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InstrumentOptions.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InstrumentOptions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InstrumentSettings.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InstrumentSettings.py`

 * *Files 9% similar despite different names*

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
@@ -75,16 +86,20 @@
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
 		self.each_cmd_as_query = False
 		self.instr_status_check = False
 		self.disable_opc_query = False
@@ -173,14 +188,15 @@
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
@@ -205,28 +221,39 @@
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
@@ -247,26 +274,40 @@
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
@@ -275,14 +316,15 @@
 		if value:
 			self.each_cmd_as_query = Conv.str_to_bool(value)
 
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
@@ -308,28 +350,29 @@
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
@@ -354,15 +397,15 @@
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
@@ -398,9 +441,44 @@
 				self.skip_status_system_setting = True
 				self.skip_clear_status = True
 				self.disable_opc_query = True
 				self.instrument_status_check = False
 				self.stb_in_error_check = False
 				self.each_cmd_as_query = True
 
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
-				raise ValueError(f"Unknown value in InitWithOptions string 'options', key 'Profile', value '{value}'. Valid values (case-insensitive): HM8123, CMQ, Minimal, ATS")
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

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/InternalLinker.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/InternalLinker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/IoTransferEventArgs.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/IoTransferEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/RepeatedCapability.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/RepeatedCapability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ScpiEnums.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ScpiEnums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/ScpiLogger.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/ScpiLogger.py`

 * *Files 1% similar despite different names*

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
@@ -366,14 +367,25 @@
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
@@ -469,15 +481,15 @@
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

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/StreamReader.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/StreamReader.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/StreamWriter.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/StreamWriter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/StructBase.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/StructBase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Types.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Types.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/Utilities.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/Utilities.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/VisaPluginSocketIo.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/VisaPluginSocketIo.py`

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

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/VisaSession.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/VisaSession.py`

 * *Files 4% similar despite different names*

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
 
 
@@ -74,14 +75,16 @@
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
@@ -189,14 +192,27 @@
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
@@ -328,15 +344,15 @@
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
@@ -364,41 +380,60 @@
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
@@ -658,16 +693,17 @@
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
@@ -683,21 +719,18 @@
 
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
@@ -711,21 +744,33 @@
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
@@ -788,20 +833,23 @@
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

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/Internal/VisaSessionSim.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/Internal/VisaSessionSim.py`

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

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/RsCMPX_WcdmaMeas.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/RsCMPX_WcdmaMeas.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from . import repcap
 from .Internal.RepeatedCapability import RepeatedCapability
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class RsCMPX_WcdmaMeas:
 	"""845 total commands, 4 Subgroups, 0 group commands"""
-	_driver_options = "SupportedInstrModels = CMW/CMP/CMX, SupportedIdnPatterns = CMW/CMP/CMX, SimulationIdnString = 'Rohde&Schwarz,CMP180,100001,4.0.186.0002'"
+	_driver_options = "SupportedInstrModels = CMW/CMP/CMX, SupportedIdnPatterns = CMW/CMP/CMX, SimulationIdnString = 'Rohde&Schwarz,CMP180,100001,5.0.40.0003'"
 	_global_logging_relative_timestamp: ClassVar[datetime] = None
 	_global_logging_target_stream: ClassVar = None
 
 	def __init__(self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsCMPX_WcdmaMeas session. \n
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
 			- ``LogToGlobalTarget = True`` - Sets the logging target to the class-property previously set with RsCMPX_WcdmaMeas.set_global_logging_target() Default: ``False``
 			- ``LoggingToConsole = True`` - Immediately starts logging to the console. Default: False
 			- ``LoggingToUdp = True`` - Immediately starts logging to the UDP port. Default: False
 			- ``LoggingUdpPort = 49200`` - UDP port to log to. Default: 49200
 		:param resource_name: VISA resource name, e.g. 'TCPIP::192.168.2.1::INSTR'
 		:param id_query: if True, the instrument's model name is verified against the models supported by the driver and eventually throws an exception.
 		:param reset: Resets the instrument (sends *RST command) and clears its status sybsystem.
 		:param options: string tokens alternating the driver settings.
 		:param direct_session: Another driver object or pyVisa object to reuse the session instead of opening a new session."""
 		self._core = Core(resource_name, id_query, reset, RsCMPX_WcdmaMeas._driver_options, options, direct_session)
-		self._core.driver_version = '4.0.186.0002'
+		self._core.driver_version = '5.0.40.0003'
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
-		curr_version_list = '4.0.186.0002'.split('.')
+		curr_version_list = '5.0.40.0003'.split('.')
 		count_min = len(min_version_list)
 		count_curr = len(curr_version_list)
 		count = count_min if count_min < count_curr else count_curr
 		for i in range(count):
 			minimum = int(min_version_list[i])
 			curr = int(curr_version_list[i])
 			if curr > minimum:
 				break
 			if curr < minimum:
-				raise RsInstrException(f"Assertion for minimum RsCMPX_WcdmaMeas version failed. Current version: '4.0.186.0002', minimum required version: '{min_version}'")
+				raise RsInstrException(f"Assertion for minimum RsCMPX_WcdmaMeas version failed. Current version: '5.0.40.0003', minimum required version: '{min_version}'")
 
 	@staticmethod
 	def list_resources(expression: str = '?*::INSTR', visa_select: str = None) -> List[str]:
 		"""Finds all the resources defined by the expression
 			- '?*' - matches all the available instruments
 			- 'USB::?*' - matches all the USB instruments
 			- 'TCPIP::192?*' - matches all the LAN instruments with the IP address starting with 192
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/__init__.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """RsCMPX_WcdmaMeas instrument driver
-	:version: 4.0.186.2
+	:version: 5.0.40.3
 	:copyright: 2023 by Rohde & Schwarz GMBH & Co. KG
 	:license: MIT, see LICENSE for more details.
 """
 
-__version__ = '4.0.186.2'
+__version__ = '5.0.40.3'
 
 # Main class
 from RsCMPX_WcdmaMeas.RsCMPX_WcdmaMeas import RsCMPX_WcdmaMeas
 
 # Bin data format
 from RsCMPX_WcdmaMeas.Internal.Conversions import BinIntFormat, BinFloatFormat
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/enums.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/enums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas/repcap.py` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas/repcap.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/PKG-INFO` & `RsCMPX_WcdmaMeas-5.0.40/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: RsCMPX-WcdmaMeas
-Version: 4.0.186
+Name: RsCMPX_WcdmaMeas
+Version: 5.0.40
 Summary: CMP180 WCDMA Measurement Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_WcdmaMeas
         ==================================
@@ -44,15 +44,18 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Fixed documentation
+        	Latest release notes summary: Update for FW 5.0.40
+        
+        	Version 5.0.40
+        		- Update for FW 5.0.40
         
         	Version 4.0.186
         		- Fixed documentation
         
         	Version 4.0.185
         		- First released version for FW 4.0.185
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/RsCMPX_WcdmaMeas.egg-info/SOURCES.txt` & `RsCMPX_WcdmaMeas-5.0.40/RsCMPX_WcdmaMeas.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -713,14 +713,15 @@
 RsCMPX_WcdmaMeas/Internal/GlobalData.py
 RsCMPX_WcdmaMeas/Internal/Instrument.py
 RsCMPX_WcdmaMeas/Internal/InstrumentErrors.py
 RsCMPX_WcdmaMeas/Internal/InstrumentOptions.py
 RsCMPX_WcdmaMeas/Internal/InstrumentSettings.py
 RsCMPX_WcdmaMeas/Internal/InternalLinker.py
 RsCMPX_WcdmaMeas/Internal/IoTransferEventArgs.py
+RsCMPX_WcdmaMeas/Internal/Properties.py
 RsCMPX_WcdmaMeas/Internal/RepeatedCapability.py
 RsCMPX_WcdmaMeas/Internal/ScpiEnums.py
 RsCMPX_WcdmaMeas/Internal/ScpiLogger.py
 RsCMPX_WcdmaMeas/Internal/StreamReader.py
 RsCMPX_WcdmaMeas/Internal/StreamWriter.py
 RsCMPX_WcdmaMeas/Internal/StructBase.py
 RsCMPX_WcdmaMeas/Internal/Types.py
```

### Comparing `RsCMPX_WcdmaMeas-4.0.186/setup.py` & `RsCMPX_WcdmaMeas-5.0.40/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.rst").read_text()
 
 # This call to setup() does all the work
 setup(
     name="RsCMPX_WcdmaMeas",
-    version="4.0.186",
+    version="5.0.40",
     description="CMP180 WCDMA Measurement Remote-control module",
     long_description=README,
     long_description_content_type="text/x-rst",
     author="Rohde & Schwarz GmbH & Co. KG",
     copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2022",
     license="MIT",
     classifiers=['License :: OSI Approved :: MIT License',
```

