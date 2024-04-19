# Comparing `tmp/jsp_vis-1.0.2.tar.gz` & `tmp/jsp_vis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsp_vis-1.0.2.tar", last modified: Thu Apr 18 15:10:52 2024, max compression
+gzip compressed data, was "jsp_vis-1.0.3.tar", last modified: Thu Apr 18 15:12:30 2024, max compression
```

## Comparing `jsp_vis-1.0.2.tar` & `jsp_vis-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.843762 jsp_vis-1.0.2/
--rw-r--r--   0 qwerty     (501) staff       (20)     1072 2024-04-11 16:16:44.000000 jsp_vis-1.0.2/LICENSE
--rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-12-26 19:19:03.000000 jsp_vis-1.0.2/MANIFEST.in
--rw-r--r--   0 qwerty     (501) staff       (20)     6534 2024-04-18 15:10:52.843697 jsp_vis-1.0.2/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)     4321 2024-04-18 15:10:27.000000 jsp_vis-1.0.2/README.md
--rw-r--r--   0 qwerty     (501) staff       (20)      994 2024-04-18 15:10:50.000000 jsp_vis-1.0.2/pyproject.toml
--rw-r--r--   0 qwerty     (501) staff       (20)      402 2024-04-18 15:10:52.844000 jsp_vis-1.0.2/setup.cfg
--rw-r--r--   0 qwerty     (501) staff       (20)       69 2023-12-26 19:19:03.000000 jsp_vis-1.0.2/setup.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.840985 jsp_vis-1.0.2/src/
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.842111 jsp_vis-1.0.2/src/jsp_vis/
--rw-r--r--   0 qwerty     (501) staff       (20)        0 2024-04-11 16:14:58.000000 jsp_vis-1.0.2/src/jsp_vis/__init__.py
--rw-r--r--   0 qwerty     (501) staff       (20)     7864 2024-04-16 19:04:18.000000 jsp_vis-1.0.2/src/jsp_vis/console.py
--rw-r--r--   0 qwerty     (501) staff       (20)     2686 2024-04-16 19:04:18.000000 jsp_vis-1.0.2/src/jsp_vis/cv2_window.py
--rw-r--r--   0 qwerty     (501) staff       (20)     1725 2024-04-16 17:22:15.000000 jsp_vis-1.0.2/src/jsp_vis/rgb_array.py
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.843222 jsp_vis-1.0.2/src/jsp_vis.egg-info/
--rw-r--r--   0 qwerty     (501) staff       (20)     6534 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/PKG-INFO
--rw-r--r--   0 qwerty     (501) staff       (20)      461 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/SOURCES.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/dependency_links.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-11 16:22:28.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/not-zip-safe
--rw-r--r--   0 qwerty     (501) staff       (20)       98 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/requires.txt
--rw-r--r--   0 qwerty     (501) staff       (20)        8 2024-04-18 15:10:52.000000 jsp_vis-1.0.2/src/jsp_vis.egg-info/top_level.txt
-drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:10:52.843065 jsp_vis-1.0.2/tests/
--rw-r--r--   0 qwerty     (501) staff       (20)      682 2024-04-16 18:50:13.000000 jsp_vis-1.0.2/tests/test_render_console.py
--rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-16 19:07:53.000000 jsp_vis-1.0.2/tests/test_render_cv2_window.py
--rw-r--r--   0 qwerty     (501) staff       (20)      574 2024-04-16 18:52:00.000000 jsp_vis-1.0.2/tests/test_render_rgb_array.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:12:30.896551 jsp_vis-1.0.3/
+-rw-r--r--   0 qwerty     (501) staff       (20)     1072 2024-04-11 16:16:44.000000 jsp_vis-1.0.3/LICENSE
+-rw-r--r--   0 qwerty     (501) staff       (20)       14 2023-12-26 19:19:03.000000 jsp_vis-1.0.3/MANIFEST.in
+-rw-r--r--   0 qwerty     (501) staff       (20)     6505 2024-04-18 15:12:30.896465 jsp_vis-1.0.3/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)     4321 2024-04-18 15:10:27.000000 jsp_vis-1.0.3/README.md
+-rw-r--r--   0 qwerty     (501) staff       (20)      965 2024-04-18 15:12:27.000000 jsp_vis-1.0.3/pyproject.toml
+-rw-r--r--   0 qwerty     (501) staff       (20)      402 2024-04-18 15:12:30.896800 jsp_vis-1.0.3/setup.cfg
+-rw-r--r--   0 qwerty     (501) staff       (20)       69 2023-12-26 19:19:03.000000 jsp_vis-1.0.3/setup.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:12:30.893636 jsp_vis-1.0.3/src/
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:12:30.894801 jsp_vis-1.0.3/src/jsp_vis/
+-rw-r--r--   0 qwerty     (501) staff       (20)        0 2024-04-11 16:14:58.000000 jsp_vis-1.0.3/src/jsp_vis/__init__.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     7864 2024-04-16 19:04:18.000000 jsp_vis-1.0.3/src/jsp_vis/console.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     2686 2024-04-16 19:04:18.000000 jsp_vis-1.0.3/src/jsp_vis/cv2_window.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     1725 2024-04-16 17:22:15.000000 jsp_vis-1.0.3/src/jsp_vis/rgb_array.py
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:12:30.895972 jsp_vis-1.0.3/src/jsp_vis.egg-info/
+-rw-r--r--   0 qwerty     (501) staff       (20)     6505 2024-04-18 15:12:30.000000 jsp_vis-1.0.3/src/jsp_vis.egg-info/PKG-INFO
+-rw-r--r--   0 qwerty     (501) staff       (20)      461 2024-04-18 15:12:30.000000 jsp_vis-1.0.3/src/jsp_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-18 15:12:30.000000 jsp_vis-1.0.3/src/jsp_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        1 2024-04-11 16:22:28.000000 jsp_vis-1.0.3/src/jsp_vis.egg-info/not-zip-safe
+-rw-r--r--   0 qwerty     (501) staff       (20)       98 2024-04-18 15:12:30.000000 jsp_vis-1.0.3/src/jsp_vis.egg-info/requires.txt
+-rw-r--r--   0 qwerty     (501) staff       (20)        8 2024-04-18 15:12:30.000000 jsp_vis-1.0.3/src/jsp_vis.egg-info/top_level.txt
+drwxr-xr-x   0 qwerty     (501) staff       (20)        0 2024-04-18 15:12:30.895825 jsp_vis-1.0.3/tests/
+-rw-r--r--   0 qwerty     (501) staff       (20)      682 2024-04-16 18:50:13.000000 jsp_vis-1.0.3/tests/test_render_console.py
+-rw-r--r--   0 qwerty     (501) staff       (20)     1190 2024-04-16 19:07:53.000000 jsp_vis-1.0.3/tests/test_render_cv2_window.py
+-rw-r--r--   0 qwerty     (501) staff       (20)      574 2024-04-16 18:52:00.000000 jsp_vis-1.0.3/tests/test_render_rgb_array.py
```

### Comparing `jsp_vis-1.0.2/LICENSE` & `jsp_vis-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.2/PKG-INFO` & `jsp_vis-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jsp-vis
-Version: 1.0.2
-Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
+Version: 1.0.3
+Summary: A visualization tool for job shop scheduling problems.
 Author: Alexander Nasuta
 Author-email: Alexander Nasuta <alexander.nasuta@wzl-iqs.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2024 Alexander Nasuta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.2 Summary: A flexible
-enviorment for job shop scheduling using the disjunctive graph apporach.
-Author: Alexander Nasuta Author-email: Alexander Nasuta
+Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.3 Summary: A visualization
+tool for job shop scheduling problems. Author: Alexander Nasuta Author-email:
+Alexander Nasuta
 wzl-iqs.rwth-aachen.de> License: MIT License Copyright (c) 2024 Alexander
 Nasuta Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
```

### Comparing `jsp_vis-1.0.2/README.md` & `jsp_vis-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.2/pyproject.toml` & `jsp_vis-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsp-vis"
-version = "1.0.2"
-description = "A flexible enviorment for job shop scheduling using the disjunctive graph apporach."
+version = "1.0.3"
+description = "A visualization tool for job shop scheduling problems."
 readme = "README.md"
 authors = [{ name = "Alexander Nasuta", email = "alexander.nasuta@wzl-iqs.rwth-aachen.de" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `jsp_vis-1.0.2/src/jsp_vis/console.py` & `jsp_vis-1.0.3/src/jsp_vis/console.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.2/src/jsp_vis/cv2_window.py` & `jsp_vis-1.0.3/src/jsp_vis/cv2_window.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.2/src/jsp_vis/rgb_array.py` & `jsp_vis-1.0.3/src/jsp_vis/rgb_array.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.2/src/jsp_vis.egg-info/PKG-INFO` & `jsp_vis-1.0.3/src/jsp_vis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jsp-vis
-Version: 1.0.2
-Summary: A flexible enviorment for job shop scheduling using the disjunctive graph apporach.
+Version: 1.0.3
+Summary: A visualization tool for job shop scheduling problems.
 Author: Alexander Nasuta
 Author-email: Alexander Nasuta <alexander.nasuta@wzl-iqs.rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2024 Alexander Nasuta
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.2 Summary: A flexible
-enviorment for job shop scheduling using the disjunctive graph apporach.
-Author: Alexander Nasuta Author-email: Alexander Nasuta
+Metadata-Version: 2.1 Name: jsp-vis Version: 1.0.3 Summary: A visualization
+tool for job shop scheduling problems. Author: Alexander Nasuta Author-email:
+Alexander Nasuta
 wzl-iqs.rwth-aachen.de> License: MIT License Copyright (c) 2024 Alexander
 Nasuta Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
```

### Comparing `jsp_vis-1.0.2/tests/test_render_console.py` & `jsp_vis-1.0.3/tests/test_render_console.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.2/tests/test_render_cv2_window.py` & `jsp_vis-1.0.3/tests/test_render_cv2_window.py`

 * *Files identical despite different names*

### Comparing `jsp_vis-1.0.2/tests/test_render_rgb_array.py` & `jsp_vis-1.0.3/tests/test_render_rgb_array.py`

 * *Files identical despite different names*

