# Comparing `tmp/pynocaptcha-1.8.7.tar.gz` & `tmp/pynocaptcha-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynocaptcha-1.8.7.tar", last modified: Mon Apr  8 01:17:52 2024, max compression
+gzip compressed data, was "pynocaptcha-1.8.8.tar", last modified: Fri Apr 19 10:27:05 2024, max compression
```

## Comparing `pynocaptcha-1.8.7.tar` & `pynocaptcha-1.8.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.072888 pynocaptcha-1.8.7/
--rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.8.7/LICENSE
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-08 01:17:52.072744 pynocaptcha-1.8.7/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.8.7/README.md
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.071203 pynocaptcha-1.8.7/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)     1095 2024-03-28 09:20:29.000000 pynocaptcha-1.8.7/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.072589 pynocaptcha-1.8.7/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/akamai.py
--rw-r--r--   0 esbiya     (501) staff       (20)      668 2024-04-04 15:59:57.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/aws.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5116 2024-04-08 01:16:56.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/discord.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-03-30 04:01:26.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/perimeterx.py
--rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.8.7/pynocaptcha/crackers/tls.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-08 01:17:52.071698 pynocaptcha-1.8.7/pynocaptcha.egg-info/
--rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/PKG-INFO
--rw-r--r--   0 esbiya     (501) staff       (20)      577 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/not-zip-safe
--rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/requires.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-04-08 01:17:52.000000 pynocaptcha-1.8.7/pynocaptcha.egg-info/top_level.txt
--rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-04-08 01:17:52.072917 pynocaptcha-1.8.7/setup.cfg
--rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-04-08 01:16:25.000000 pynocaptcha-1.8.7/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-19 10:27:05.988473 pynocaptcha-1.8.8/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1074 2023-03-15 06:31:13.000000 pynocaptcha-1.8.8/LICENSE
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-19 10:27:05.988297 pynocaptcha-1.8.8/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2023-03-15 09:37:56.000000 pynocaptcha-1.8.8/README.md
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-19 10:27:05.986110 pynocaptcha-1.8.8/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1199 2024-04-19 10:26:57.000000 pynocaptcha-1.8.8/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-19 10:27:05.987820 pynocaptcha-1.8.8/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     1054 2023-11-15 10:37:10.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/akamai.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      668 2024-04-04 15:59:57.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/aws.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5116 2024-04-08 01:16:56.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1061 2024-02-27 06:17:10.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      744 2023-08-14 02:01:08.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/discord.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1221 2023-07-03 06:08:01.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2088 2024-01-15 06:49:23.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1413 2024-04-19 10:26:30.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/kasada.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1559 2024-03-30 04:01:26.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/perimeterx.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     3077 2023-12-13 01:23:55.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1639 2023-06-15 08:25:19.000000 pynocaptcha-1.8.8/pynocaptcha/crackers/tls.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2024-04-19 10:27:05.986619 pynocaptcha-1.8.8/pynocaptcha.egg-info/
+-rw-r--r--   0 esbiya     (501) staff       (20)      564 2024-04-19 10:27:05.000000 pynocaptcha-1.8.8/pynocaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 esbiya     (501) staff       (20)      608 2024-04-19 10:27:05.000000 pynocaptcha-1.8.8/pynocaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-19 10:27:05.000000 pynocaptcha-1.8.8/pynocaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)        1 2024-04-19 10:27:05.000000 pynocaptcha-1.8.8/pynocaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 esbiya     (501) staff       (20)       15 2024-04-19 10:27:05.000000 pynocaptcha-1.8.8/pynocaptcha.egg-info/requires.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       33 2024-04-19 10:27:05.000000 pynocaptcha-1.8.8/pynocaptcha.egg-info/top_level.txt
+-rw-r--r--   0 esbiya     (501) staff       (20)       38 2024-04-19 10:27:05.988507 pynocaptcha-1.8.8/setup.cfg
+-rw-r--r--   0 esbiya     (501) staff       (20)      845 2024-04-19 10:27:02.000000 pynocaptcha-1.8.8/setup.py
```

### Comparing `pynocaptcha-1.8.7/LICENSE` & `pynocaptcha-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/PKG-INFO` & `pynocaptcha-1.8.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynocaptcha
-Version: 1.8.7
+Version: 1.8.8
 Summary: nocaptcha.io api
 License: MIT
 Keywords: nocaptcha
 Platform: all
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pynocaptcha-1.8.7/pynocaptcha/__init__.py` & `pynocaptcha-1.8.8/pynocaptcha/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from .crackers.aws import AwsUniversalCracker
 from .crackers.cloudflare import CloudFlareCracker
 from .crackers.discord import DiscordCracker
 from .crackers.hcaptcha import HcaptchaCracker
 from .crackers.incapsula import (IncapsulaRbzidCracker,
                                  IncapsulaReese84Cracker,
                                  IncapsulaUtmvcCracker)
+from .crackers.kasada import KasadaCdCracker, KasadaCtCracker
 from .crackers.perimeterx import PerimeterxCracker
 from .crackers.recaptcha import (ReCaptchaAppCracker,
                                  ReCaptchaEnterpriseCracker,
                                  ReCaptchaSteamCracker,
                                  ReCaptchaUniversalCracker)
 from .crackers.tls import TlsV1Cracker
 
 __all__ = [
     'pynocaptcha', 
     'CloudFlareCracker', 'IncapsulaReese84Cracker', 'IncapsulaUtmvcCracker', 'IncapsulaRbzidCracker', 'HcaptchaCracker', 
     'AkamaiV2Cracker', 'ReCaptchaUniversalCracker', 'ReCaptchaEnterpriseCracker', 'ReCaptchaSteamCracker',
-    'TlsV1Cracker', 'DiscordCracker', 'ReCaptchaAppCracker', 'AwsUniversalCracker', 'PerimeterxCracker'
+    'TlsV1Cracker', 'DiscordCracker', 'ReCaptchaAppCracker', 'AwsUniversalCracker', 'PerimeterxCracker',
+    'KasadaCtCracker', 'KasadaCdCracker'
 ]
```

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/akamai.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/akamai.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/aws.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/aws.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/base.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/base.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/discord.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/discord.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/perimeterx.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/perimeterx.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha/crackers/tls.py` & `pynocaptcha-1.8.8/pynocaptcha/crackers/tls.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.8.7/pynocaptcha.egg-info/PKG-INFO` & `pynocaptcha-1.8.8/pynocaptcha.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynocaptcha
-Version: 1.8.7
+Version: 1.8.8
 Summary: nocaptcha.io api
 License: MIT
 Keywords: nocaptcha
 Platform: all
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pynocaptcha-1.8.7/pynocaptcha.egg-info/SOURCES.txt` & `pynocaptcha-1.8.8/pynocaptcha.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 pynocaptcha/crackers/akamai.py
 pynocaptcha/crackers/aws.py
 pynocaptcha/crackers/base.py
 pynocaptcha/crackers/cloudflare.py
 pynocaptcha/crackers/discord.py
 pynocaptcha/crackers/hcaptcha.py
 pynocaptcha/crackers/incapsula.py
+pynocaptcha/crackers/kasada.py
 pynocaptcha/crackers/perimeterx.py
 pynocaptcha/crackers/recaptcha.py
 pynocaptcha/crackers/tls.py
```

### Comparing `pynocaptcha-1.8.7/setup.py` & `pynocaptcha-1.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 setup(
     name='pynocaptcha',
-    version='1.8.7',
+    version='1.8.8',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

