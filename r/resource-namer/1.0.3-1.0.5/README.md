# Comparing `tmp/resource-namer-1.0.3.tar.gz` & `tmp/resource-namer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resource-namer-1.0.3.tar", last modified: Sat Jan  7 21:52:08 2023, max compression
+gzip compressed data, was "resource-namer-1.0.5.tar", last modified: Fri Apr 19 17:33:12 2024, max compression
```

## Comparing `resource-namer-1.0.3.tar` & `resource-namer-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2023-01-07 21:52:08.963665 resource-namer-1.0.3/
--rw-r--r--   0 drace      (501) staff       (20)    11357 2023-01-07 21:35:09.000000 resource-namer-1.0.3/LICENSE
--rw-r--r--   0 drace      (501) staff       (20)     1933 2023-01-07 21:52:08.963793 resource-namer-1.0.3/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)     1109 2023-01-07 21:48:27.000000 resource-namer-1.0.3/README.md
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2023-01-07 21:52:08.918656 resource-namer-1.0.3/resource_namer/
--rw-r--r--   0 drace      (501) staff       (20)     2125 2023-01-07 21:35:09.000000 resource-namer-1.0.3/resource_namer/__init__.py
--rw-r--r--   0 drace      (501) staff       (20)       36 2023-01-07 21:35:09.000000 resource-namer-1.0.3/resource_namer/__main__.py
--rw-r--r--   0 drace      (501) staff       (20)      290 2023-01-07 21:35:09.000000 resource-namer-1.0.3/resource_namer/__meta__.py
--rw-r--r--   0 drace      (501) staff       (20)    25687 2023-01-07 21:35:09.000000 resource-namer-1.0.3/resource_namer/word_lists.py
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2023-01-07 21:52:08.963338 resource-namer-1.0.3/resource_namer.egg-info/
--rw-r--r--   0 drace      (501) staff       (20)     1933 2023-01-07 21:52:08.000000 resource-namer-1.0.3/resource_namer.egg-info/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)      298 2023-01-07 21:52:08.000000 resource-namer-1.0.3/resource_namer.egg-info/SOURCES.txt
--rw-r--r--   0 drace      (501) staff       (20)        1 2023-01-07 21:52:08.000000 resource-namer-1.0.3/resource_namer.egg-info/dependency_links.txt
--rw-r--r--   0 drace      (501) staff       (20)       15 2023-01-07 21:52:08.000000 resource-namer-1.0.3/resource_namer.egg-info/top_level.txt
--rw-r--r--   0 drace      (501) staff       (20)     1079 2023-01-07 21:52:08.970681 resource-namer-1.0.3/setup.cfg
--rw-r--r--   0 drace      (501) staff       (20)     2087 2023-01-07 21:46:29.000000 resource-namer-1.0.3/setup.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:33:12.731579 resource-namer-1.0.5/
+-rw-r--r--   0 drace      (501) staff       (20)    11357 2023-01-07 21:35:09.000000 resource-namer-1.0.5/LICENSE
+-rw-r--r--   0 drace      (501) staff       (20)     1913 2024-04-19 17:33:12.731673 resource-namer-1.0.5/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)     1069 2023-01-09 21:32:06.000000 resource-namer-1.0.5/README.md
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:33:12.730546 resource-namer-1.0.5/resource_namer/
+-rw-r--r--   0 drace      (501) staff       (20)     2125 2023-01-07 21:35:09.000000 resource-namer-1.0.5/resource_namer/__init__.py
+-rw-r--r--   0 drace      (501) staff       (20)       36 2023-01-07 21:35:09.000000 resource-namer-1.0.5/resource_namer/__main__.py
+-rw-r--r--   0 drace      (501) staff       (20)      290 2024-04-19 17:32:49.000000 resource-namer-1.0.5/resource_namer/__meta__.py
+-rw-r--r--   0 drace      (501) staff       (20)    25726 2023-01-09 21:16:05.000000 resource-namer-1.0.5/resource_namer/word_lists.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:33:12.731414 resource-namer-1.0.5/resource_namer.egg-info/
+-rw-r--r--   0 drace      (501) staff       (20)     1913 2024-04-19 17:33:12.000000 resource-namer-1.0.5/resource_namer.egg-info/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)      298 2024-04-19 17:33:12.000000 resource-namer-1.0.5/resource_namer.egg-info/SOURCES.txt
+-rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-19 17:33:12.000000 resource-namer-1.0.5/resource_namer.egg-info/dependency_links.txt
+-rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-19 17:33:12.000000 resource-namer-1.0.5/resource_namer.egg-info/top_level.txt
+-rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-19 17:33:12.732041 resource-namer-1.0.5/setup.cfg
+-rw-r--r--   0 drace      (501) staff       (20)     2087 2023-01-07 21:46:29.000000 resource-namer-1.0.5/setup.py
```

### Comparing `resource-namer-1.0.3/LICENSE` & `resource-namer-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `resource-namer-1.0.3/PKG-INFO` & `resource-namer-1.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: resource-namer
-Version: 1.0.3
+Version: 1.0.5
 Summary: Generate names for things with phonetic alliteration - use with GUIDs for easy identification.
 Home-page: https://github.com/darenr/resource-namer
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: Apache License, Version 2.0, January 2004
 Keywords: random resource name generator
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# academic-avocado-namer
+# resource-namer
 
 [![License](https://img.shields.io/badge/license-Apache-blue.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0)
-[![PyPI Version](https://img.shields.io/pypi/v/academic-avocado-namer.svg?style=flat&color=blue)](https://pypi.org/project/academic-avocado-namer)
-[![Python Versions](https://img.shields.io/pypi/pyversions/academic-avocado-namer.svg?logo=python&logoColor=white&style=flat)](https://pypi.org/project/academic-avocado-namer)
+[![PyPI Version](https://img.shields.io/pypi/v/resource-namer.svg?style=flat&color=blue)](https://pypi.org/project/resource-namer)
+[![Python Versions](https://img.shields.io/pypi/pyversions/resource-namer.svg?logo=python&logoColor=white&style=flat)](https://pypi.org/project/resource-namer)
 
 
 Name things with better names than GUIDs, use in combination with
 GUIDs or datetimes.
 
 ## module main
 
@@ -67,7 +68,9 @@
 
 >>> generate_name(prefer_plants=True)
 'irritating-inkberry'
 
 ```
 
 https://pypi.org/project/resource-namer
+
+
```

### Comparing `resource-namer-1.0.3/README.md` & `resource-namer-1.0.5/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# academic-avocado-namer
+# resource-namer
 
 [![License](https://img.shields.io/badge/license-Apache-blue.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0)
-[![PyPI Version](https://img.shields.io/pypi/v/academic-avocado-namer.svg?style=flat&color=blue)](https://pypi.org/project/academic-avocado-namer)
-[![Python Versions](https://img.shields.io/pypi/pyversions/academic-avocado-namer.svg?logo=python&logoColor=white&style=flat)](https://pypi.org/project/academic-avocado-namer)
+[![PyPI Version](https://img.shields.io/pypi/v/resource-namer.svg?style=flat&color=blue)](https://pypi.org/project/resource-namer)
+[![Python Versions](https://img.shields.io/pypi/pyversions/resource-namer.svg?logo=python&logoColor=white&style=flat)](https://pypi.org/project/resource-namer)
 
 
 Name things with better names than GUIDs, use in combination with
 GUIDs or datetimes.
 
 ## module main
```

### Comparing `resource-namer-1.0.3/resource_namer/__init__.py` & `resource-namer-1.0.5/resource_namer/__init__.py`

 * *Files identical despite different names*

### Comparing `resource-namer-1.0.3/resource_namer/word_lists.py` & `resource-namer-1.0.5/resource_namer/word_lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -1415,14 +1415,15 @@
     "hornet",
     "horse",
     "human",
     "hummingbird",
     "hyena",
     "ibex",
     "ibis",
+    "iguana",
     "jackal",
     "jaguar",
     "jay",
     "jellyfish",
     "kangaroo",
     "kingfisher",
     "koala",
@@ -1497,14 +1498,15 @@
     "scorpion",
     "seahorse",
     "seal",
     "shark",
     "sheep",
     "shrew",
     "skunk",
+    "sloth",
     "snail",
     "snake",
     "sparrow",
     "spider",
     "spoonbill",
     "squid",
     "squirrel",
@@ -1539,14 +1541,15 @@
     "wombat",
     "woodcock",
     "woodpecker",
     "worm",
     "wren",
     "yak",
     "zebra",
+    "zebu",
     "zombie",
 ]
 
 plants = [
     "alder",
     "almond",
     "ambrosia",
```

### Comparing `resource-namer-1.0.3/resource_namer.egg-info/PKG-INFO` & `resource-namer-1.0.5/resource_namer.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: resource-namer
-Version: 1.0.3
+Version: 1.0.5
 Summary: Generate names for things with phonetic alliteration - use with GUIDs for easy identification.
 Home-page: https://github.com/darenr/resource-namer
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: Apache License, Version 2.0, January 2004
 Keywords: random resource name generator
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# academic-avocado-namer
+# resource-namer
 
 [![License](https://img.shields.io/badge/license-Apache-blue.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0)
-[![PyPI Version](https://img.shields.io/pypi/v/academic-avocado-namer.svg?style=flat&color=blue)](https://pypi.org/project/academic-avocado-namer)
-[![Python Versions](https://img.shields.io/pypi/pyversions/academic-avocado-namer.svg?logo=python&logoColor=white&style=flat)](https://pypi.org/project/academic-avocado-namer)
+[![PyPI Version](https://img.shields.io/pypi/v/resource-namer.svg?style=flat&color=blue)](https://pypi.org/project/resource-namer)
+[![Python Versions](https://img.shields.io/pypi/pyversions/resource-namer.svg?logo=python&logoColor=white&style=flat)](https://pypi.org/project/resource-namer)
 
 
 Name things with better names than GUIDs, use in combination with
 GUIDs or datetimes.
 
 ## module main
 
@@ -67,7 +68,9 @@
 
 >>> generate_name(prefer_plants=True)
 'irritating-inkberry'
 
 ```
 
 https://pypi.org/project/resource-namer
+
+
```

### Comparing `resource-namer-1.0.3/setup.cfg` & `resource-namer-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `resource-namer-1.0.3/setup.py` & `resource-namer-1.0.5/setup.py`

 * *Files identical despite different names*

