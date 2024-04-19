# Comparing `tmp/solvent_guide-0.4.6.tar.gz` & `tmp/solvent_guide-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\pczjh2\OneDrive - The University of Nottingham\PycharmProjects\solvent_guide\dist\.tmp-5x0xtfnr\solvent_guide-0.4.6.ta", last modified: Fri Apr 19 15:34:31 2024, max compression
+gzip compressed data, was "C:\Users\pczjh2\OneDrive - The University of Nottingham\PycharmProjects\solvent_guide\dist\.tmp-nzqraqe1\solvent_guide-0.4.7.ta", last modified: Fri Apr 19 15:40:47 2024, max compression
```

## Comparing `solvent_guide-0.4.6.tar` & `solvent_guide-0.4.7.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.489588 solvent_guide-0.4.6/
--rw-rw-rw-   0        0        0    35163 2023-10-03 13:29:19.000000 solvent_guide-0.4.6/LICENSE
--rw-rw-rw-   0        0        0     9489 2024-04-19 15:34:31.488585 solvent_guide-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     8826 2024-04-19 09:51:44.000000 solvent_guide-0.4.6/README.md
--rw-rw-rw-   0        0        0      765 2024-04-19 15:34:16.000000 solvent_guide-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0      325 2024-04-19 15:34:31.493607 solvent_guide-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0       37 2024-04-19 15:34:16.000000 solvent_guide-0.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.385788 solvent_guide-0.4.6/src/
--rw-rw-rw-   0        0        0        0 2023-09-27 14:03:04.000000 solvent_guide-0.4.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.403018 solvent_guide-0.4.6/src/solvent_guide/
--rw-rw-rw-   0        0        0        0 2023-09-29 09:09:48.000000 solvent_guide-0.4.6/src/solvent_guide/__init__.py
--rw-rw-rw-   0        0        0     6594 2024-02-08 16:49:30.000000 solvent_guide-0.4.6/src/solvent_guide/add_solvent.py
--rw-rw-rw-   0        0        0     1116 2023-10-05 13:54:32.000000 solvent_guide-0.4.6/src/solvent_guide/remove_solvent.py
--rw-rw-rw-   0        0        0      544 2023-10-05 12:16:25.000000 solvent_guide-0.4.6/src/solvent_guide/reset_solvents.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.429985 solvent_guide-0.4.6/src/solvent_guide/sources/
--rw-rw-rw-   0        0        0      407 2023-10-03 15:45:26.000000 solvent_guide-0.4.6/src/solvent_guide/sources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.432986 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/
--rw-rw-rw-   0        0        0        0 2023-09-07 12:55:19.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.451629 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/
--rw-rw-rw-   0        0        0   501509 2023-09-06 14:40:31.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
--rw-rw-rw-   0        0        0      112 2023-09-06 14:40:31.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
--rw-rw-rw-   0        0        0      231 2024-02-08 14:16:33.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
--rw-rw-rw-   0        0        0     4079 2024-02-08 14:32:56.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/routes.py
--rw-rw-rw-   0        0        0      232 2024-04-19 10:28:55.000000 solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/user_colours.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.365788 solvent_guide-0.4.6/src/solvent_guide/sources/static/
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.460582 solvent_guide-0.4.6/src/solvent_guide/sources/static/css/
--rw-rw-rw-   0        0        0      141 2023-10-06 08:46:41.000000 solvent_guide-0.4.6/src/solvent_guide/sources/static/css/hazard_colours.css
--rw-rw-rw-   0        0        0     1904 2023-09-27 09:44:06.000000 solvent_guide-0.4.6/src/solvent_guide/sources/static/css/pagestyle.css
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.463585 solvent_guide-0.4.6/src/solvent_guide/sources/static/js/
--rw-rw-rw-   0        0        0     2060 2024-04-19 12:09:25.000000 solvent_guide-0.4.6/src/solvent_guide/sources/static/js/custom_colours.js
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.480583 solvent_guide-0.4.6/src/solvent_guide/sources/templates/
--rw-rw-rw-   0        0        0    12967 2024-02-08 14:29:28.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/accessibility.html
--rw-rw-rw-   0        0        0     2274 2024-04-19 12:53:45.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/base.html
--rw-rw-rw-   0        0        0    17178 2024-04-19 13:59:02.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide.html
--rw-rw-rw-   0        0        0     6067 2023-09-06 14:40:32.000000 solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide_help.html
--rw-rw-rw-   0        0        0      520 2024-04-19 15:31:48.000000 solvent_guide-0.4.6/src/solvent_guide/webapp.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:34:31.485586 solvent_guide-0.4.6/src/solvent_guide.egg-info/
--rw-rw-rw-   0        0        0     9489 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1188 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-04-19 15:34:31.000000 solvent_guide-0.4.6/src/solvent_guide.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.797750 solvent_guide-0.4.7/
+-rw-rw-rw-   0        0        0    35163 2023-10-03 13:29:19.000000 solvent_guide-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0     9710 2024-04-19 15:40:47.796750 solvent_guide-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8826 2024-04-19 09:51:44.000000 solvent_guide-0.4.7/README.md
+-rw-rw-rw-   0        0        0      950 2024-04-19 15:40:33.000000 solvent_guide-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0      325 2024-04-19 15:40:47.801748 solvent_guide-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0       37 2024-04-19 15:34:16.000000 solvent_guide-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.695688 solvent_guide-0.4.7/src/
+-rw-rw-rw-   0        0        0        0 2023-09-27 14:03:04.000000 solvent_guide-0.4.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.710689 solvent_guide-0.4.7/src/solvent_guide/
+-rw-rw-rw-   0        0        0        0 2023-09-29 09:09:48.000000 solvent_guide-0.4.7/src/solvent_guide/__init__.py
+-rw-rw-rw-   0        0        0     6594 2024-02-08 16:49:30.000000 solvent_guide-0.4.7/src/solvent_guide/add_solvent.py
+-rw-rw-rw-   0        0        0     1116 2023-10-05 13:54:32.000000 solvent_guide-0.4.7/src/solvent_guide/remove_solvent.py
+-rw-rw-rw-   0        0        0      544 2023-10-05 12:16:25.000000 solvent_guide-0.4.7/src/solvent_guide/reset_solvents.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.740718 solvent_guide-0.4.7/src/solvent_guide/sources/
+-rw-rw-rw-   0        0        0      407 2023-10-03 15:45:26.000000 solvent_guide-0.4.7/src/solvent_guide/sources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.743719 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/
+-rw-rw-rw-   0        0        0        0 2023-09-07 12:55:19.000000 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.759907 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/
+-rw-rw-rw-   0        0        0   501509 2023-09-06 14:40:31.000000 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
+-rw-rw-rw-   0        0        0      112 2023-09-06 14:40:31.000000 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
+-rw-rw-rw-   0        0        0      231 2024-02-08 14:16:33.000000 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
+-rw-rw-rw-   0        0        0     4079 2024-02-08 14:32:56.000000 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/routes.py
+-rw-rw-rw-   0        0        0      232 2024-04-19 10:28:55.000000 solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/user_colours.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.676688 solvent_guide-0.4.7/src/solvent_guide/sources/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.765750 solvent_guide-0.4.7/src/solvent_guide/sources/static/css/
+-rw-rw-rw-   0        0        0      141 2023-10-06 08:46:41.000000 solvent_guide-0.4.7/src/solvent_guide/sources/static/css/hazard_colours.css
+-rw-rw-rw-   0        0        0     1904 2023-09-27 09:44:06.000000 solvent_guide-0.4.7/src/solvent_guide/sources/static/css/pagestyle.css
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.768749 solvent_guide-0.4.7/src/solvent_guide/sources/static/js/
+-rw-rw-rw-   0        0        0     2060 2024-04-19 12:09:25.000000 solvent_guide-0.4.7/src/solvent_guide/sources/static/js/custom_colours.js
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.784752 solvent_guide-0.4.7/src/solvent_guide/sources/templates/
+-rw-rw-rw-   0        0        0    12967 2024-02-08 14:29:28.000000 solvent_guide-0.4.7/src/solvent_guide/sources/templates/accessibility.html
+-rw-rw-rw-   0        0        0     2274 2024-04-19 12:53:45.000000 solvent_guide-0.4.7/src/solvent_guide/sources/templates/base.html
+-rw-rw-rw-   0        0        0    17178 2024-04-19 13:59:02.000000 solvent_guide-0.4.7/src/solvent_guide/sources/templates/solvent_guide.html
+-rw-rw-rw-   0        0        0     6067 2023-09-06 14:40:32.000000 solvent_guide-0.4.7/src/solvent_guide/sources/templates/solvent_guide_help.html
+-rw-rw-rw-   0        0        0      520 2024-04-19 15:31:48.000000 solvent_guide-0.4.7/src/solvent_guide/webapp.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:40:47.794749 solvent_guide-0.4.7/src/solvent_guide.egg-info/
+-rw-rw-rw-   0        0        0     9710 2024-04-19 15:40:47.000000 solvent_guide-0.4.7/src/solvent_guide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1228 2024-04-19 15:40:47.000000 solvent_guide-0.4.7/src/solvent_guide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:40:47.000000 solvent_guide-0.4.7/src/solvent_guide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-04-19 15:40:47.000000 solvent_guide-0.4.7/src/solvent_guide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-19 15:40:47.000000 solvent_guide-0.4.7/src/solvent_guide.egg-info/top_level.txt
```

### Comparing `solvent_guide-0.4.6/LICENSE` & `solvent_guide-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/PKG-INFO` & `solvent_guide-0.4.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: solvent_guide
-Version: 0.4.6
-Summary: Standalone version of the solvent guide as shown in the AI4Green ELN
-Author-email: Joe Heeley <joe.heeley@nottingham.ac.uk>, Samuel Boobier <samuel.boobier@googlemail.com>
-Project-URL: Homepage, https://github.com/JoeHeeley2/solvent_flashcards
-Project-URL: Bug Tracker, https://github.com/JoeHeeley2/solvent_flashcards/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Solvent Guide
 The solvent guide provides a visual interface for the comparison of
 common laboratory solvents to encourage greener decision-making during reaction design. The data for each solvent was collected
 from the [CHEM21 solvent guide](https://pubs.rsc.org/en/content/articlelanding/2016/gc/c5gc01008j) and is provided via a simple visual interface.
 
 This software was first developed as part of [AI4Green](https://pubs.acs.org/doi/10.1021/acs.jcim.3c00306), a Machine-Learning powered Electronic 
 Lab Notebook (ELN) that aims to facilitate greener choices at the laboratory level. It has been adapted as a standalone tool
```

### Comparing `solvent_guide-0.4.6/README.md` & `solvent_guide-0.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: solvent_guide
+Version: 0.4.7
+Summary: Standalone version of the solvent guide as shown in the AI4Green ELN
+Author-email: Joe Heeley <joe.heeley@nottingham.ac.uk>, Samuel Boobier <samuel.boobier@googlemail.com>
+Project-URL: Homepage, https://github.com/JoeHeeley2/solvent_flashcards
+Project-URL: Bug Tracker, https://github.com/JoeHeeley2/solvent_flashcards/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pandas>=1.4.1
+Requires-Dist: blinker>=1.6.2
+Requires-Dist: flask>=2.3.2
+Requires-Dist: plotly>=5.9.0
+Requires-Dist: colorama>=0.4.6
+Requires-Dist: python-dateutil>=2.8.2
+
 # Solvent Guide
 The solvent guide provides a visual interface for the comparison of
 common laboratory solvents to encourage greener decision-making during reaction design. The data for each solvent was collected
 from the [CHEM21 solvent guide](https://pubs.rsc.org/en/content/articlelanding/2016/gc/c5gc01008j) and is provided via a simple visual interface.
 
 This software was first developed as part of [AI4Green](https://pubs.acs.org/doi/10.1021/acs.jcim.3c00306), a Machine-Learning powered Electronic 
 Lab Notebook (ELN) that aims to facilitate greener choices at the laboratory level. It has been adapted as a standalone tool
```

### Comparing `solvent_guide-0.4.6/pyproject.toml` & `solvent_guide-0.4.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "solvent_guide"
-version = "0.4.6"
+version = "0.4.7"
 authors = [
   {name="Joe Heeley", email="joe.heeley@nottingham.ac.uk"},
     { name="Samuel Boobier", email="samuel.boobier@googlemail.com" }
 ]
 description = "Standalone version of the solvent guide as shown in the AI4Green ELN"
 readme = "README.md"
 requires-python = ">=3.9"
+dependencies = [
+    "numpy>=1.26.0",
+    "pandas>=1.4.1",
+    "blinker>=1.6.2",
+    "flask>=2.3.2",
+    "plotly>=5.9.0",
+    "colorama>=0.4.6",
+    "python-dateutil>=2.8.2"
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `solvent_guide-0.4.6/src/solvent_guide/add_solvent.py` & `solvent_guide-0.4.7/src/solvent_guide/add_solvent.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/remove_solvent.py` & `solvent_guide-0.4.7/src/solvent_guide/remove_solvent.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/reset_solvents.py` & `solvent_guide-0.4.7/src/solvent_guide/reset_solvents.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv` & `solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/blueprints/solvent_guide/routes.py` & `solvent_guide-0.4.7/src/solvent_guide/sources/blueprints/solvent_guide/routes.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/static/css/pagestyle.css` & `solvent_guide-0.4.7/src/solvent_guide/sources/static/css/pagestyle.css`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/static/js/custom_colours.js` & `solvent_guide-0.4.7/src/solvent_guide/sources/static/js/custom_colours.js`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/templates/accessibility.html` & `solvent_guide-0.4.7/src/solvent_guide/sources/templates/accessibility.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/templates/base.html` & `solvent_guide-0.4.7/src/solvent_guide/sources/templates/base.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide.html` & `solvent_guide-0.4.7/src/solvent_guide/sources/templates/solvent_guide.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/sources/templates/solvent_guide_help.html` & `solvent_guide-0.4.7/src/solvent_guide/sources/templates/solvent_guide_help.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide/webapp.py` & `solvent_guide-0.4.7/src/solvent_guide/webapp.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.6/src/solvent_guide.egg-info/PKG-INFO` & `solvent_guide-0.4.7/src/solvent_guide.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: solvent_guide
-Version: 0.4.6
+Version: 0.4.7
 Summary: Standalone version of the solvent guide as shown in the AI4Green ELN
 Author-email: Joe Heeley <joe.heeley@nottingham.ac.uk>, Samuel Boobier <samuel.boobier@googlemail.com>
 Project-URL: Homepage, https://github.com/JoeHeeley2/solvent_flashcards
 Project-URL: Bug Tracker, https://github.com/JoeHeeley2/solvent_flashcards/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.26.0
+Requires-Dist: pandas>=1.4.1
+Requires-Dist: blinker>=1.6.2
+Requires-Dist: flask>=2.3.2
+Requires-Dist: plotly>=5.9.0
+Requires-Dist: colorama>=0.4.6
+Requires-Dist: python-dateutil>=2.8.2
 
 # Solvent Guide
 The solvent guide provides a visual interface for the comparison of
 common laboratory solvents to encourage greener decision-making during reaction design. The data for each solvent was collected
 from the [CHEM21 solvent guide](https://pubs.rsc.org/en/content/articlelanding/2016/gc/c5gc01008j) and is provided via a simple visual interface.
 
 This software was first developed as part of [AI4Green](https://pubs.acs.org/doi/10.1021/acs.jcim.3c00306), a Machine-Learning powered Electronic
```

### Comparing `solvent_guide-0.4.6/src/solvent_guide.egg-info/SOURCES.txt` & `solvent_guide-0.4.7/src/solvent_guide.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/solvent_guide/add_solvent.py
 src/solvent_guide/remove_solvent.py
 src/solvent_guide/reset_solvents.py
 src/solvent_guide/webapp.py
 src/solvent_guide.egg-info/PKG-INFO
 src/solvent_guide.egg-info/SOURCES.txt
 src/solvent_guide.egg-info/dependency_links.txt
+src/solvent_guide.egg-info/requires.txt
 src/solvent_guide.egg-info/top_level.txt
 src/solvent_guide/sources/__init__.py
 src/solvent_guide/sources/blueprints/__init__.py
 src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
 src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
 src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
 src/solvent_guide/sources/blueprints/solvent_guide/routes.py
```

