# Comparing `tmp/report_creator-1.0.4.tar.gz` & `tmp/report_creator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report_creator-1.0.4.tar", last modified: Fri Apr 19 17:39:07 2024, max compression
+gzip compressed data, was "report_creator-1.0.5.tar", last modified: Fri Apr 19 17:46:09 2024, max compression
```

## Comparing `report_creator-1.0.4.tar` & `report_creator-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:39:07.727113 report_creator-1.0.4/
--rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-19 17:26:07.000000 report_creator-1.0.4/LICENSE
--rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 17:18:24.000000 report_creator-1.0.4/MANIFEST.in
--rw-r--r--   0 drace      (501) staff       (20)     4052 2024-04-19 17:39:07.727015 report_creator-1.0.4/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)     3259 2024-04-19 17:18:24.000000 report_creator-1.0.4/README.md
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:39:07.725267 report_creator-1.0.4/report_creator/
--rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 17:18:24.000000 report_creator-1.0.4/report_creator/__init__.py
--rw-r--r--   0 drace      (501) staff       (20)      182 2024-04-19 17:38:59.000000 report_creator-1.0.4/report_creator/__meta__.py
--rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 17:18:24.000000 report_creator-1.0.4/report_creator/report_creator.py
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:39:07.726224 report_creator-1.0.4/report_creator/templates/
--rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 17:18:24.000000 report_creator-1.0.4/report_creator/templates/default.html
-drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:39:07.726699 report_creator-1.0.4/report_creator.egg-info/
--rw-r--r--   0 drace      (501) staff       (20)     4052 2024-04-19 17:39:07.000000 report_creator-1.0.4/report_creator.egg-info/PKG-INFO
--rw-r--r--   0 drace      (501) staff       (20)      325 2024-04-19 17:39:07.000000 report_creator-1.0.4/report_creator.egg-info/SOURCES.txt
--rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-19 17:39:07.000000 report_creator-1.0.4/report_creator.egg-info/dependency_links.txt
--rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-19 17:39:07.000000 report_creator-1.0.4/report_creator.egg-info/top_level.txt
--rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-19 17:39:07.727450 report_creator-1.0.4/setup.cfg
--rw-r--r--   0 drace      (501) staff       (20)     2122 2024-04-19 17:18:24.000000 report_creator-1.0.4/setup.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:46:09.355753 report_creator-1.0.5/
+-rw-r--r--   0 drace      (501) staff       (20)     1066 2024-04-19 17:26:07.000000 report_creator-1.0.5/LICENSE
+-rw-r--r--   0 drace      (501) staff       (20)       69 2024-04-19 17:18:24.000000 report_creator-1.0.5/MANIFEST.in
+-rw-r--r--   0 drace      (501) staff       (20)     4093 2024-04-19 17:46:09.355675 report_creator-1.0.5/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)     3300 2024-04-19 17:44:05.000000 report_creator-1.0.5/README.md
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:46:09.354062 report_creator-1.0.5/report_creator/
+-rw-r--r--   0 drace      (501) staff       (20)      478 2024-04-19 17:18:24.000000 report_creator-1.0.5/report_creator/__init__.py
+-rw-r--r--   0 drace      (501) staff       (20)      182 2024-04-19 17:44:39.000000 report_creator-1.0.5/report_creator/__meta__.py
+-rw-r--r--   0 drace      (501) staff       (20)    45428 2024-04-19 17:18:24.000000 report_creator-1.0.5/report_creator/report_creator.py
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:46:09.354941 report_creator-1.0.5/report_creator/templates/
+-rw-r--r--   0 drace      (501) staff       (20)    10528 2024-04-19 17:18:24.000000 report_creator-1.0.5/report_creator/templates/default.html
+drwxr-xr-x   0 drace      (501) staff       (20)        0 2024-04-19 17:46:09.355400 report_creator-1.0.5/report_creator.egg-info/
+-rw-r--r--   0 drace      (501) staff       (20)     4093 2024-04-19 17:46:09.000000 report_creator-1.0.5/report_creator.egg-info/PKG-INFO
+-rw-r--r--   0 drace      (501) staff       (20)      325 2024-04-19 17:46:09.000000 report_creator-1.0.5/report_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 drace      (501) staff       (20)        1 2024-04-19 17:46:09.000000 report_creator-1.0.5/report_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 drace      (501) staff       (20)       15 2024-04-19 17:46:09.000000 report_creator-1.0.5/report_creator.egg-info/top_level.txt
+-rw-r--r--   0 drace      (501) staff       (20)     1079 2024-04-19 17:46:09.356095 report_creator-1.0.5/setup.cfg
+-rw-r--r--   0 drace      (501) staff       (20)     2122 2024-04-19 17:18:24.000000 report_creator-1.0.5/setup.py
```

### Comparing `report_creator-1.0.4/LICENSE` & `report_creator-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.4/PKG-INFO` & `report_creator-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT License
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Report Creator
 
-[![License](https://img.shields.io/badge/license-Apache-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI Version](https://img.shields.io/pypi/v/report_creator.svg?style=for-the-badge&color=blue)](https://pypi.org/project/report_creator)
 [![Python Versions](https://img.shields.io/pypi/pyversions/report_creator.svg?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/report_creator)
 
 Library to assemble reports in HTML from various components using python
 
 ## Features
 
@@ -94,15 +94,20 @@
 # optionally for pretty html generation
 pip install beautifulsoup4 lxml
 
 # recommended installs for code hygiene
 pip install ruff
 
 # build "kitchen_sink" example
+
 make
+
+# install local package
+pip install -e .
+
 ```
 
 ## Dev Notes
 
 * **4/18/24 - no breaking changes**, all changes should go through standard deprecation policies
 * The Blocks/Groups use css [flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).
   * Blocks flow vertically (columns)
```

### Comparing `report_creator-1.0.4/README.md` & `report_creator-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Report Creator
 
-[![License](https://img.shields.io/badge/license-Apache-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI Version](https://img.shields.io/pypi/v/report_creator.svg?style=for-the-badge&color=blue)](https://pypi.org/project/report_creator)
 [![Python Versions](https://img.shields.io/pypi/pyversions/report_creator.svg?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/report_creator)
 
 Library to assemble reports in HTML from various components using python
 
 ## Features
 
@@ -75,15 +75,20 @@
 # optionally for pretty html generation
 pip install beautifulsoup4 lxml
 
 # recommended installs for code hygiene
 pip install ruff
 
 # build "kitchen_sink" example
+
 make
+
+# install local package
+pip install -e .
+
 ```
 
 ## Dev Notes
 
 * **4/18/24 - no breaking changes**, all changes should go through standard deprecation policies
 * The Blocks/Groups use css [flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).
   * Blocks flow vertically (columns)
```

### Comparing `report_creator-1.0.4/report_creator/report_creator.py` & `report_creator-1.0.5/report_creator/report_creator.py`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.4/report_creator/templates/default.html` & `report_creator-1.0.5/report_creator/templates/default.html`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.4/report_creator.egg-info/PKG-INFO` & `report_creator-1.0.5/report_creator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report_creator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Produce self-contained HTML reports from Python
 Home-page: https://github.com/darenr/report_creator
 Author: Daren Race
 Author-email: daren.race@gmail.com
 License: MIT License
 Keywords: python,html,reports,report,creator,generator,markdown,yaml,plot,chart,table
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Report Creator
 
-[![License](https://img.shields.io/badge/license-Apache-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI Version](https://img.shields.io/pypi/v/report_creator.svg?style=for-the-badge&color=blue)](https://pypi.org/project/report_creator)
 [![Python Versions](https://img.shields.io/pypi/pyversions/report_creator.svg?logo=python&logoColor=white&style=for-the-badge)](https://pypi.org/project/report_creator)
 
 Library to assemble reports in HTML from various components using python
 
 ## Features
 
@@ -94,15 +94,20 @@
 # optionally for pretty html generation
 pip install beautifulsoup4 lxml
 
 # recommended installs for code hygiene
 pip install ruff
 
 # build "kitchen_sink" example
+
 make
+
+# install local package
+pip install -e .
+
 ```
 
 ## Dev Notes
 
 * **4/18/24 - no breaking changes**, all changes should go through standard deprecation policies
 * The Blocks/Groups use css [flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/).
   * Blocks flow vertically (columns)
```

### Comparing `report_creator-1.0.4/setup.cfg` & `report_creator-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `report_creator-1.0.4/setup.py` & `report_creator-1.0.5/setup.py`

 * *Files identical despite different names*

