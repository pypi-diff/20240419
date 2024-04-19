# Comparing `tmp/solvent_guide-0.4.4.tar.gz` & `tmp/solvent_guide-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\pczjh2\OneDrive - The University of Nottingham\PycharmProjects\solvent_guide\dist\.tmp-pz_b_aeh\solvent_guide-0.4.4.ta", last modified: Thu Feb 15 10:45:00 2024, max compression
+gzip compressed data, was "C:\Users\pczjh2\OneDrive - The University of Nottingham\PycharmProjects\solvent_guide\dist\.tmp-dlkpk0_w\solvent_guide-0.4.5.ta", last modified: Fri Apr 19 15:27:03 2024, max compression
```

## Comparing `solvent_guide-0.4.4.tar` & `solvent_guide-0.4.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 10:45:00.003951 solvent_guide-0.4.4/
--rw-rw-rw-   0        0        0    35163 2023-10-03 13:29:19.000000 solvent_guide-0.4.4/LICENSE
--rw-rw-rw-   0        0        0     9489 2024-02-15 10:45:00.002948 solvent_guide-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     8826 2023-10-17 16:29:20.000000 solvent_guide-0.4.4/README.md
--rw-rw-rw-   0        0        0      765 2024-02-15 10:44:45.000000 solvent_guide-0.4.4/pyproject.toml
--rw-rw-rw-   0        0        0      149 2024-02-15 10:45:00.011032 solvent_guide-0.4.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.837569 solvent_guide-0.4.4/src/
--rw-rw-rw-   0        0        0        0 2023-09-27 14:03:04.000000 solvent_guide-0.4.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.866565 solvent_guide-0.4.4/src/solvent_guide/
--rw-rw-rw-   0        0        0        0 2023-09-29 09:09:48.000000 solvent_guide-0.4.4/src/solvent_guide/__init__.py
--rw-rw-rw-   0        0        0     6594 2024-02-08 16:49:30.000000 solvent_guide-0.4.4/src/solvent_guide/add_solvent.py
--rw-rw-rw-   0        0        0     1116 2023-10-05 13:54:32.000000 solvent_guide-0.4.4/src/solvent_guide/remove_solvent.py
--rw-rw-rw-   0        0        0      544 2023-10-05 12:16:25.000000 solvent_guide-0.4.4/src/solvent_guide/reset_solvents.py
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.899706 solvent_guide-0.4.4/src/solvent_guide/sources/
--rw-rw-rw-   0        0        0      407 2023-10-03 15:45:26.000000 solvent_guide-0.4.4/src/solvent_guide/sources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.902703 solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/
--rw-rw-rw-   0        0        0        0 2023-09-07 12:55:19.000000 solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.933821 solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/solvent_guide/
--rw-rw-rw-   0        0        0   501509 2023-09-06 14:40:31.000000 solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
--rw-rw-rw-   0        0        0      112 2023-09-06 14:40:31.000000 solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
--rw-rw-rw-   0        0        0      231 2024-02-08 14:16:33.000000 solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
--rw-rw-rw-   0        0        0     4079 2024-02-08 14:32:56.000000 solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/solvent_guide/routes.py
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.813430 solvent_guide-0.4.4/src/solvent_guide/sources/static/
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.944821 solvent_guide-0.4.4/src/solvent_guide/sources/static/css/
--rw-rw-rw-   0        0        0      141 2023-10-06 08:46:41.000000 solvent_guide-0.4.4/src/solvent_guide/sources/static/css/hazard_colours.css
--rw-rw-rw-   0        0        0     1904 2023-09-27 09:44:06.000000 solvent_guide-0.4.4/src/solvent_guide/sources/static/css/pagestyle.css
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.952819 solvent_guide-0.4.4/src/solvent_guide/sources/static/js/
--rw-rw-rw-   0        0        0     2060 2023-10-06 09:47:54.000000 solvent_guide-0.4.4/src/solvent_guide/sources/static/js/custom_colours.js
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.991949 solvent_guide-0.4.4/src/solvent_guide/sources/templates/
--rw-rw-rw-   0        0        0    12967 2024-02-08 14:29:28.000000 solvent_guide-0.4.4/src/solvent_guide/sources/templates/accessibility.html
--rw-rw-rw-   0        0        0     2269 2024-02-08 10:48:28.000000 solvent_guide-0.4.4/src/solvent_guide/sources/templates/base.html
--rw-rw-rw-   0        0        0    17027 2024-02-08 10:51:23.000000 solvent_guide-0.4.4/src/solvent_guide/sources/templates/solvent_guide.html
--rw-rw-rw-   0        0        0     6067 2023-09-06 14:40:32.000000 solvent_guide-0.4.4/src/solvent_guide/sources/templates/solvent_guide_help.html
--rw-rw-rw-   0        0        0      520 2024-02-15 10:05:14.000000 solvent_guide-0.4.4/src/solvent_guide/webapp.py
-drwxrwxrwx   0        0        0        0 2024-02-15 10:44:59.998948 solvent_guide-0.4.4/src/solvent_guide.egg-info/
--rw-rw-rw-   0        0        0     9489 2024-02-15 10:44:59.000000 solvent_guide-0.4.4/src/solvent_guide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2024-02-15 10:44:59.000000 solvent_guide-0.4.4/src/solvent_guide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 10:44:59.000000 solvent_guide-0.4.4/src/solvent_guide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-02-15 10:44:59.000000 solvent_guide-0.4.4/src/solvent_guide.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.186120 solvent_guide-0.4.5/
+-rw-rw-rw-   0        0        0    35163 2023-10-03 13:29:19.000000 solvent_guide-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0     9489 2024-04-19 15:27:03.185119 solvent_guide-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8826 2024-04-19 09:51:44.000000 solvent_guide-0.4.5/README.md
+-rw-rw-rw-   0        0        0      765 2024-04-19 14:15:01.000000 solvent_guide-0.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0      325 2024-04-19 15:27:03.190240 solvent_guide-0.4.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.031785 solvent_guide-0.4.5/src/
+-rw-rw-rw-   0        0        0        0 2023-09-27 14:03:04.000000 solvent_guide-0.4.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.060813 solvent_guide-0.4.5/src/solvent_guide/
+-rw-rw-rw-   0        0        0        0 2023-09-29 09:09:48.000000 solvent_guide-0.4.5/src/solvent_guide/__init__.py
+-rw-rw-rw-   0        0        0     6594 2024-02-08 16:49:30.000000 solvent_guide-0.4.5/src/solvent_guide/add_solvent.py
+-rw-rw-rw-   0        0        0     1116 2023-10-05 13:54:32.000000 solvent_guide-0.4.5/src/solvent_guide/remove_solvent.py
+-rw-rw-rw-   0        0        0      544 2023-10-05 12:16:25.000000 solvent_guide-0.4.5/src/solvent_guide/reset_solvents.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.090209 solvent_guide-0.4.5/src/solvent_guide/sources/
+-rw-rw-rw-   0        0        0      407 2023-10-03 15:45:26.000000 solvent_guide-0.4.5/src/solvent_guide/sources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.093123 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/
+-rw-rw-rw-   0        0        0        0 2023-09-07 12:55:19.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.127122 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/
+-rw-rw-rw-   0        0        0   501509 2023-09-06 14:40:31.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
+-rw-rw-rw-   0        0        0      112 2023-09-06 14:40:31.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
+-rw-rw-rw-   0        0        0      231 2024-02-08 14:16:33.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
+-rw-rw-rw-   0        0        0     4079 2024-02-08 14:32:56.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/routes.py
+-rw-rw-rw-   0        0        0      232 2024-04-19 10:28:55.000000 solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/user_colours.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.008787 solvent_guide-0.4.5/src/solvent_guide/sources/static/
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.136177 solvent_guide-0.4.5/src/solvent_guide/sources/static/css/
+-rw-rw-rw-   0        0        0      141 2023-10-06 08:46:41.000000 solvent_guide-0.4.5/src/solvent_guide/sources/static/css/hazard_colours.css
+-rw-rw-rw-   0        0        0     1904 2023-09-27 09:44:06.000000 solvent_guide-0.4.5/src/solvent_guide/sources/static/css/pagestyle.css
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.144120 solvent_guide-0.4.5/src/solvent_guide/sources/static/js/
+-rw-rw-rw-   0        0        0     2060 2024-04-19 12:09:25.000000 solvent_guide-0.4.5/src/solvent_guide/sources/static/js/custom_colours.js
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.177119 solvent_guide-0.4.5/src/solvent_guide/sources/templates/
+-rw-rw-rw-   0        0        0    12967 2024-02-08 14:29:28.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/accessibility.html
+-rw-rw-rw-   0        0        0     2274 2024-04-19 12:53:45.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/base.html
+-rw-rw-rw-   0        0        0    17178 2024-04-19 13:59:02.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide.html
+-rw-rw-rw-   0        0        0     6067 2023-09-06 14:40:32.000000 solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide_help.html
+-rw-rw-rw-   0        0        0      519 2024-04-19 09:23:32.000000 solvent_guide-0.4.5/src/solvent_guide/webapp.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:27:03.182121 solvent_guide-0.4.5/src/solvent_guide.egg-info/
+-rw-rw-rw-   0        0        0     9489 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-19 15:27:02.000000 solvent_guide-0.4.5/src/solvent_guide.egg-info/top_level.txt
```

### Comparing `solvent_guide-0.4.4/LICENSE` & `solvent_guide-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/PKG-INFO` & `solvent_guide-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvent_guide
-Version: 0.4.4
+Version: 0.4.5
 Summary: Standalone version of the solvent guide as shown in the AI4Green ELN
 Author-email: Joe Heeley <joe.heeley@nottingham.ac.uk>, Samuel Boobier <samuel.boobier@googlemail.com>
 Project-URL: Homepage, https://github.com/JoeHeeley2/solvent_flashcards
 Project-URL: Bug Tracker, https://github.com/JoeHeeley2/solvent_flashcards/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -21,20 +21,20 @@
 Lab Notebook (ELN) that aims to facilitate greener choices at the laboratory level. It has been adapted as a standalone tool
 in the hope that it may be useful outside the ELN.
 
 ## Installation
 
 First, ensure you have installed the required dependencies:
 ```
-pip install numpy==1.26.0 pandas==1.4.1 blinker==1.6.2 flask==2.3.2 plotly==5.9.0 colorama==0.4.6 python-dateutil==2.8.2
+pip install numpy>=1.26.0 pandas>=1.4.1 blinker>=1.6.2 flask>=2.3.2 plotly>=5.9.0 colorama>=0.4.6 python-dateutil>=2.8.2
 ```
 
 Then, the package can be installed from pip using the following command:
 ```
-pip install solvent_guide
+pip install solvent-guide
 ```
 
 ## Run from command line
 
 Once installed, the Solvent Guide can be launched from the command line with:
 
 ```
```

### Comparing `solvent_guide-0.4.4/README.md` & `solvent_guide-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 Lab Notebook (ELN) that aims to facilitate greener choices at the laboratory level. It has been adapted as a standalone tool
 in the hope that it may be useful outside the ELN.
 
 ## Installation
 
 First, ensure you have installed the required dependencies:
 ```
-pip install numpy==1.26.0 pandas==1.4.1 blinker==1.6.2 flask==2.3.2 plotly==5.9.0 colorama==0.4.6 python-dateutil==2.8.2
+pip install numpy>=1.26.0 pandas>=1.4.1 blinker>=1.6.2 flask>=2.3.2 plotly>=5.9.0 colorama>=0.4.6 python-dateutil>=2.8.2
 ```
 
 Then, the package can be installed from pip using the following command:
 ```
-pip install solvent_guide
+pip install solvent-guide
 ```
 
 ## Run from command line
 
 Once installed, the Solvent Guide can be launched from the command line with:
 
 ```
```

### Comparing `solvent_guide-0.4.4/pyproject.toml` & `solvent_guide-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "solvent_guide"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   {name="Joe Heeley", email="joe.heeley@nottingham.ac.uk"},
     { name="Samuel Boobier", email="samuel.boobier@googlemail.com" }
 ]
 description = "Standalone version of the solvent guide as shown in the AI4Green ELN"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `solvent_guide-0.4.4/src/solvent_guide/add_solvent.py` & `solvent_guide-0.4.5/src/solvent_guide/add_solvent.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/remove_solvent.py` & `solvent_guide-0.4.5/src/solvent_guide/remove_solvent.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/reset_solvents.py` & `solvent_guide-0.4.5/src/solvent_guide/reset_solvents.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv` & `solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/blueprints/solvent_guide/routes.py` & `solvent_guide-0.4.5/src/solvent_guide/sources/blueprints/solvent_guide/routes.py`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/static/css/pagestyle.css` & `solvent_guide-0.4.5/src/solvent_guide/sources/static/css/pagestyle.css`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/static/js/custom_colours.js` & `solvent_guide-0.4.5/src/solvent_guide/sources/static/js/custom_colours.js`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/templates/accessibility.html` & `solvent_guide-0.4.5/src/solvent_guide/sources/templates/accessibility.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/templates/base.html` & `solvent_guide-0.4.5/src/solvent_guide/sources/templates/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+<!DOCTYPE html>
 <html>
 
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
 <!--    External JavaScript + libraries-->
     <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
@@ -30,15 +31,14 @@
     </div>
 
 </body>
 
 
 <footer class="bg-light text-center text-lg-start fixed-bottom footer-at-bottom">
 
-    </div>
     <!--Utility Links-->
     <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2);">
         <table>
             <tr></tr>
             <tr>
                 <a class="text-dark" href="https://twitter.com/ai4green" target="_blank">Twitter</a> |
                 <a class="text-dark" href="https://github.com/AI4Green/solvent_flashcards" target="_blank">GitHub</a>
```

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/templates/solvent_guide.html` & `solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 {% extends "base.html" %}
 {% block content %}
-<head>
-    <script type="text/javascript" src="{{ url_for('static', filename='js/custom_colours.js') }}"></script>
-</head>
 
 <div class="container-fluid">
     <h2>Solvent Guide</h2>
     <p><a class="btn btn-primary" href="{{ url_for('solvent_guide.solvent_guide_help') }}">About the Solvent Guide &#10097;</a>
     <a class="btn btn-secondary" href="{{ url_for('solvent_guide.accessibility') }}">Colour Preferences &#10097;</a></p>
     <p>Choose up to two solvents from the classes below to compare them!</p>
-    <div class="row">
-      <div class="col-2">
+    <div class="row nav">
+      <div class="col-2" style="overflow-y:scroll; max-height:400px; direction:rtl">
         {% for family in families %}
         <a id="family{{ loop.index }}" style="color: black; border: none" class="my-0 py-1 list-group-item" data-toggle="collapse" href="#collapse{{ loop.index }}" role="button" aria-expanded="false" aria-controls="collapseExample">
           <b>{{ family }}</b>
         </a>
         <div class="collapse" id="collapse{{ loop.index }}">
           {% for solvent in solvents %}
           {% if solvent["Family"] == family %}
@@ -212,17 +209,14 @@
           </div>
           {% endfor %}
         </div>
       </div>
     </div>
 </div>
 
-
-
-
 <script>
   $(document).ready(function(){
   $('[data-toggle="tooltip"]').tooltip();
    setColours();
 });
   let iteration = 0;
   function showTab(sol, sub){
@@ -249,33 +243,40 @@
       $(sol).tab('show');
       if(iteration % 2 === 0){
         iteration = iteration + 1
       }
       return
     }
     if(iteration % 2 === 0){
-      sol = '[href="#list2-' + sol + '"]';
+      if(sub != "sub1" && sub != "sub2") {
+        sol = '[href="#list2-' + sol + '"]';
+      }
       $(sol).tab('show');
     }
-    else{
-      sol = '[href="#list-' + sol + '"]';
+    else {
+      if(sub != "sub1" && sub != "sub2") {
+        sol = '[href="#list-' + sol + '"]';
+      }
       $(sol).tab('show');
     }
   }
 </script>
 <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
+<script type="text/javascript" src="{{ url_for('static', filename='js/custom_colours.js') }}"></script>
 {% for solvent in solvents %}
 <script>
   var graph = {{ solvent["graph"] | safe}}
   Plotly.newPlot('chart{{ solvent["Number"] }}', graph, {});
   Plotly.newPlot('chart2_{{ solvent["Number"] }}', graph, {});
 </script>
 {% endfor %}
 {% if sol %}
 <script>
+
   $(document).ready(function(){
     showTab({{ sol }}, 'no');
     showTab({{ sol2 }}, 'no');
   });
 </script>
 {% endif %}
+
 {% endblock %}
```

### Comparing `solvent_guide-0.4.4/src/solvent_guide/sources/templates/solvent_guide_help.html` & `solvent_guide-0.4.5/src/solvent_guide/sources/templates/solvent_guide_help.html`

 * *Files identical despite different names*

### Comparing `solvent_guide-0.4.4/src/solvent_guide/webapp.py` & `solvent_guide-0.4.5/src/solvent_guide/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # !/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from .sources import create_app
+from sources import create_app
 from threading import Timer
 import webbrowser
 import os
 
 app = create_app()
 
 port = os.getenv("FLASK_RUN_PORT")
```

### Comparing `solvent_guide-0.4.4/src/solvent_guide.egg-info/PKG-INFO` & `solvent_guide-0.4.5/src/solvent_guide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvent_guide
-Version: 0.4.4
+Version: 0.4.5
 Summary: Standalone version of the solvent guide as shown in the AI4Green ELN
 Author-email: Joe Heeley <joe.heeley@nottingham.ac.uk>, Samuel Boobier <samuel.boobier@googlemail.com>
 Project-URL: Homepage, https://github.com/JoeHeeley2/solvent_flashcards
 Project-URL: Bug Tracker, https://github.com/JoeHeeley2/solvent_flashcards/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -21,20 +21,20 @@
 Lab Notebook (ELN) that aims to facilitate greener choices at the laboratory level. It has been adapted as a standalone tool
 in the hope that it may be useful outside the ELN.
 
 ## Installation
 
 First, ensure you have installed the required dependencies:
 ```
-pip install numpy==1.26.0 pandas==1.4.1 blinker==1.6.2 flask==2.3.2 plotly==5.9.0 colorama==0.4.6 python-dateutil==2.8.2
+pip install numpy>=1.26.0 pandas>=1.4.1 blinker>=1.6.2 flask>=2.3.2 plotly>=5.9.0 colorama>=0.4.6 python-dateutil>=2.8.2
 ```
 
 Then, the package can be installed from pip using the following command:
 ```
-pip install solvent_guide
+pip install solvent-guide
 ```
 
 ## Run from command line
 
 Once installed, the Solvent Guide can be launched from the command line with:
 
 ```
```

### Comparing `solvent_guide-0.4.4/src/solvent_guide.egg-info/SOURCES.txt` & `solvent_guide-0.4.5/src/solvent_guide.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/solvent_guide.egg-info/top_level.txt
 src/solvent_guide/sources/__init__.py
 src/solvent_guide/sources/blueprints/__init__.py
 src/solvent_guide/sources/blueprints/solvent_guide/CHEM21_full.csv
 src/solvent_guide/sources/blueprints/solvent_guide/__init__.py
 src/solvent_guide/sources/blueprints/solvent_guide/default_colours.txt
 src/solvent_guide/sources/blueprints/solvent_guide/routes.py
+src/solvent_guide/sources/blueprints/solvent_guide/user_colours.txt
 src/solvent_guide/sources/static/css/hazard_colours.css
 src/solvent_guide/sources/static/css/pagestyle.css
 src/solvent_guide/sources/static/js/custom_colours.js
 src/solvent_guide/sources/templates/accessibility.html
 src/solvent_guide/sources/templates/base.html
 src/solvent_guide/sources/templates/solvent_guide.html
 src/solvent_guide/sources/templates/solvent_guide_help.html
```

