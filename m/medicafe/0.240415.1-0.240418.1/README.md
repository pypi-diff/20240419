# Comparing `tmp/medicafe-0.240415.1.tar.gz` & `tmp/medicafe-0.240418.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240415.1.tar", last modified: Tue Apr 16 04:05:43 2024, max compression
+gzip compressed data, was "medicafe-0.240418.1.tar", last modified: Fri Apr 19 03:53:32 2024, max compression
```

## Comparing `medicafe-0.240415.1.tar` & `medicafe-0.240418.1.tar`

### file list

```diff
@@ -1,13 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 04:05:43.591000 medicafe-0.240415.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240415.1/LICENSE
--rw-rw-rw-   0        0        0      827 2024-04-16 04:05:43.569000 medicafe-0.240415.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240415.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 04:05:43.556000 medicafe-0.240415.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      827 2024-04-16 04:05:43.000000 medicafe-0.240415.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-16 04:05:43.000000 medicafe-0.240415.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 04:05:43.000000 medicafe-0.240415.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240415.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2024-04-16 04:05:43.000000 medicafe-0.240415.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 04:05:43.000000 medicafe-0.240415.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 04:05:43.588000 medicafe-0.240415.1/setup.cfg
--rw-rw-rw-   0        0        0      984 2024-04-16 03:16:31.000000 medicafe-0.240415.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:53:32.732000 medicafe-0.240418.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240418.1/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-19 03:53:32.154000 medicafe-0.240418.1/MediBot/
+-rw-rw-rw-   0        0        0    15172 2024-04-19 03:46:30.000000 medicafe-0.240418.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240418.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    12503 2024-04-19 03:45:33.000000 medicafe-0.240418.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     9281 2024-04-19 03:05:07.000000 medicafe-0.240418.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6314 2024-04-19 03:00:07.000000 medicafe-0.240418.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240418.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240418.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240418.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240418.1/MediBot/update_json.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:53:32.526000 medicafe-0.240418.1/MediLink/
+-rw-rw-rw-   0        0        0    13842 2024-04-19 02:21:32.000000 medicafe-0.240418.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240418.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    22116 2024-04-19 00:09:39.000000 medicafe-0.240418.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    32894 2024-04-19 00:37:58.000000 medicafe-0.240418.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3070 2024-04-19 03:17:08.000000 medicafe-0.240418.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0     6838 2024-04-18 21:22:06.000000 medicafe-0.240418.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     8306 2024-04-19 00:12:45.000000 medicafe-0.240418.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8769 2024-04-19 00:19:03.000000 medicafe-0.240418.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0      133 2024-03-27 01:07:04.000000 medicafe-0.240418.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240418.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240418.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4409 2024-04-18 02:17:49.000000 medicafe-0.240418.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     6080 2024-04-18 21:27:03.000000 medicafe-0.240418.1/MediLink/MediLink_Up.py
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240418.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240418.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      827 2024-04-19 03:53:32.709000 medicafe-0.240418.1/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240418.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 03:53:32.696000 medicafe-0.240418.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      827 2024-04-19 03:53:31.000000 medicafe-0.240418.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-04-19 03:53:31.000000 medicafe-0.240418.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 03:53:31.000000 medicafe-0.240418.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240418.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2024-04-19 03:53:31.000000 medicafe-0.240418.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-19 03:53:31.000000 medicafe-0.240418.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 03:53:32.728000 medicafe-0.240418.1/setup.cfg
+-rw-rw-rw-   0        0        0      984 2024-04-19 03:50:48.000000 medicafe-0.240418.1/setup.py
```

### Comparing `medicafe-0.240415.1/LICENSE` & `medicafe-0.240418.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240415.1/PKG-INFO` & `medicafe-0.240418.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240415.1
+Version: 0.240418.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240415.1/README.md` & `medicafe-0.240418.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240415.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240418.1/medicafe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240415.1
+Version: 0.240418.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240415.1/setup.py` & `medicafe-0.240418.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version='0.240415.1',
+    version='0.240418.1',
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```

