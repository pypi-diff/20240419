# Comparing `tmp/more_captcha-0.5.0-py3-none-any.whl.zip` & `tmp/more_captcha-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 591998 bytes, number of entries: 102
--rw-r--r--  2.0 unx      378 b- defN 23-Oct-30 19:24 captcha/__init__.py
+Zip file size: 591973 bytes, number of entries: 102
+-rw-r--r--  2.0 unx      362 b- defN 24-Apr-19 17:58 captcha/__init__.py
 -rw-r--r--  2.0 unx     8013 b- defN 23-Oct-30 17:01 captcha/audio.py
--rw-r--r--  2.0 unx     7200 b- defN 23-Oct-30 17:01 captcha/image.py
+-rw-r--r--  2.0 unx     7200 b- defN 24-Apr-19 17:37 captcha/image.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Oct-30 17:01 captcha/py.typed
 -rw-r--r--  2.0 unx   117072 b- defN 23-Oct-30 17:01 captcha/data/DroidSansMono.ttf
 -rw-r--r--  2.0 unx      940 b- defN 23-Oct-30 17:01 captcha/data/beep.wav
 -rw-r--r--  2.0 unx    10120 b- defN 23-Oct-30 19:13 captcha/data/ /default.wav
 -rw-r--r--  2.0 unx    22902 b- defN 23-Oct-30 19:13 captcha/data/!/default.wav
 -rw-r--r--  2.0 unx    19054 b- defN 23-Oct-30 19:13 captcha/data/"/default.wav
 -rw-r--r--  2.0 unx    12960 b- defN 23-Oct-30 19:13 captcha/data/#/default.wav
@@ -92,13 +92,13 @@
 -rw-r--r--  2.0 unx    10704 b- defN 23-Oct-30 17:29 captcha/data/w/default.wav
 -rw-r--r--  2.0 unx     9610 b- defN 23-Oct-30 17:29 captcha/data/x/default.wav
 -rw-r--r--  2.0 unx     9326 b- defN 23-Oct-30 17:29 captcha/data/y/default.wav
 -rw-r--r--  2.0 unx     9804 b- defN 23-Oct-30 17:29 captcha/data/z/default.wav
 -rw-r--r--  2.0 unx    22710 b- defN 23-Oct-30 19:13 captcha/data/{/default.wav
 -rw-r--r--  2.0 unx    22876 b- defN 23-Oct-30 19:13 captcha/data/}/default.wav
 -rw-r--r--  2.0 unx    13990 b- defN 23-Oct-30 19:13 captcha/data/~/default.wav
--rw-r--r--  2.0 unx     1475 b- defN 23-Oct-30 19:27 more_captcha-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2330 b- defN 23-Oct-30 19:27 more_captcha-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-30 19:27 more_captcha-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Oct-30 19:27 more_captcha-0.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8460 b- defN 23-Oct-30 19:27 more_captcha-0.5.0.dist-info/RECORD
-102 files, 1172241 bytes uncompressed, 578888 bytes compressed:  50.6%
+-rw-r--r--  2.0 unx     1475 b- defN 24-Apr-19 18:00 more_captcha-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2316 b- defN 24-Apr-19 18:00 more_captcha-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 18:00 more_captcha-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 18:00 more_captcha-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8460 b- defN 24-Apr-19 18:00 more_captcha-1.0.0.dist-info/RECORD
+102 files, 1172211 bytes uncompressed, 578863 bytes compressed:  50.6%
```

## zipnote {}

```diff
@@ -285,23 +285,23 @@
 
 Filename: captcha/data/}/default.wav
 Comment: 
 
 Filename: captcha/data/~/default.wav
 Comment: 
 
-Filename: more_captcha-0.5.0.dist-info/LICENSE
+Filename: more_captcha-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: more_captcha-0.5.0.dist-info/METADATA
+Filename: more_captcha-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: more_captcha-0.5.0.dist-info/WHEEL
+Filename: more_captcha-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: more_captcha-0.5.0.dist-info/top_level.txt
+Filename: more_captcha-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: more_captcha-0.5.0.dist-info/RECORD
+Filename: more_captcha-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## captcha/__init__.py

```diff
@@ -6,11 +6,11 @@
 
     A captcha library that generates audio and image CAPTCHAs.
 
     :copyright: (c) 2014 by Hsiaoming Yang.
     :license: BSD, see LICENSE for more details.
 """
 
-__version__ = '0.5.0'
+__version__ = '1.0.0'
 __author__ = 'Hsiaoming Yang <me@lepture.com>'
-__co_author__ = 'Ari Archer <ari.web.xyz@gmail.com>'
-__homepage__ = 'https://ari-web.xyz/gh/captcha'
+__co_author__ = 'Ari Archer <ari@ari.lt>'
+__homepage__ = 'https://ari.lt/gh/captcha'
```

## Comparing `more_captcha-0.5.0.dist-info/LICENSE` & `more_captcha-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `more_captcha-0.5.0.dist-info/METADATA` & `more_captcha-1.0.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: more-captcha
-Version: 0.5.0
+Version: 1.0.0
 Summary: A captcha library that generates audio and image CAPTCHAs.
-Author-email: Hsiaoming Yang <me@lepture.com>, Ari Archer <ari.web.xyz@gmail.com>
+Author-email: Hsiaoming Yang <me@lepture.com>, Ari Archer <ari@ari.lt>
 License: BSD-3-Clause
 Project-URL: Documentation, https://captcha.lepture.com/
-Project-URL: Source, https://ari-web.xyz/gh/captcha
+Project-URL: Source, https://ari.lt/gh/captcha
 Project-URL: Original, https://github.com/lepture/captcha
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `more_captcha-0.5.0.dist-info/RECORD` & `more_captcha-1.0.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-captcha/__init__.py,sha256=fLotCQOfxpY-WMPJKyzUxJrKFsJPUHFPPR0K_E8FIr8,378
+captcha/__init__.py,sha256=fWPCUhhTX8W6xo8PcknXWnA-i9FVjMKXTGItPzcRgiY,362
 captcha/audio.py,sha256=EQrkUPC3TZiQaYpcjJUw41adAu9nI1URanK4u0AL10U,8013
 captcha/image.py,sha256=SUj7Gv9UlsM9WcQr_DBCxEIu2PfwnDMjWVGzxLDC6xg,7200
 captcha/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 captcha/data/DroidSansMono.ttf,sha256=MFEurbRgSOPfrwSL4ODCdtER_B3pc3EZcQSfQl6_-mc,117072
 captcha/data/beep.wav,sha256=GejO1Bo36Lfoj2RGr6aTs9mG4X3O4xuxb8xWmMnLd_0,940
 captcha/data/ /default.wav,sha256=f9_BsLUMbNi_E_-fzJ5VoWCEHLJNAIpDQL4Yok_D_Hw,10120
 captcha/data/!/default.wav,sha256=Ll9rck-OdsRC5j8Pa-yPsiJTBx9fmAKUdGl-vl0W2ek,22902
@@ -91,12 +91,12 @@
 captcha/data/w/default.wav,sha256=6FkVXADzIswD_2GTtD_biOjS-c_WhXDvfYWaq_dUdXk,10704
 captcha/data/x/default.wav,sha256=bScZjhLHy3epX-sfXhPy6V9DH4wsNQp7yVGQiaf3vBY,9610
 captcha/data/y/default.wav,sha256=xSArDeaP6Mzpi_BSm9pJRy05CpaISBYrJ28jTJ4vKg0,9326
 captcha/data/z/default.wav,sha256=RhyAQff1zD6f047NmAD8h6pGFQxfY5PnorME5ALrWik,9804
 captcha/data/{/default.wav,sha256=t6ePcc_dUCuP4NWPXEBj-Rgwf_gU43XKc5Fs6ci2_zI,22710
 captcha/data/}/default.wav,sha256=QkES3WqlAXG2GfISabMth9wrFwMqDqPJ1_vwgQV56Mo,22876
 captcha/data/~/default.wav,sha256=Zf4h8B_wRETY0L9HlFELSCm9bY-H80-c_lHheCB5cMk,13990
-more_captcha-0.5.0.dist-info/LICENSE,sha256=U5AT_Y4Z90T4vw4npTK7_1TNaJ7O96gA9Wrl3IJL6HA,1475
-more_captcha-0.5.0.dist-info/METADATA,sha256=EAMVrjeqXHw67Fj7HqW67-oygjZfSzQFiYcNhm3xT0c,2330
-more_captcha-0.5.0.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-more_captcha-0.5.0.dist-info/top_level.txt,sha256=krw23fzzUC0oTgsEakKehDWjBfNzFYPTtC0hVpktXyQ,8
-more_captcha-0.5.0.dist-info/RECORD,,
+more_captcha-1.0.0.dist-info/LICENSE,sha256=U5AT_Y4Z90T4vw4npTK7_1TNaJ7O96gA9Wrl3IJL6HA,1475
+more_captcha-1.0.0.dist-info/METADATA,sha256=e75OH9Xq8Jb6FF1eTY4gKewKkWjrzYzbSifxYUXyfME,2316
+more_captcha-1.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+more_captcha-1.0.0.dist-info/top_level.txt,sha256=krw23fzzUC0oTgsEakKehDWjBfNzFYPTtC0hVpktXyQ,8
+more_captcha-1.0.0.dist-info/RECORD,,
```

