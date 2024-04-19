# Comparing `tmp/pandas-wizard-0.0.1.dev0.tar.gz` & `tmp/pandas-wizard-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-wizard-0.0.1.dev0.tar", last modified: Sun Apr 14 14:39:45 2024, max compression
+gzip compressed data, was "pandas-wizard-1.0.0.dev0.tar", last modified: Fri Apr 19 15:52:53 2024, max compression
```

## Comparing `pandas-wizard-0.0.1.dev0.tar` & `pandas-wizard-1.0.0.dev0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 14:39:45.083506 pandas-wizard-0.0.1.dev0/
--rw-rw-rw-   0        0        0     1561 2024-04-14 14:25:43.000000 pandas-wizard-0.0.1.dev0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2024-04-11 18:59:27.000000 pandas-wizard-0.0.1.dev0/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-11 18:59:27.000000 pandas-wizard-0.0.1.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     2177 2024-04-14 14:39:45.081517 pandas-wizard-0.0.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0      736 2024-04-14 14:34:45.000000 pandas-wizard-0.0.1.dev0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 14:39:45.079507 pandas-wizard-0.0.1.dev0/pandas_wizard.egg-info/
--rw-rw-rw-   0        0        0     2177 2024-04-14 14:39:44.000000 pandas-wizard-0.0.1.dev0/pandas_wizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-14 14:39:44.000000 pandas-wizard-0.0.1.dev0/pandas_wizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 14:39:44.000000 pandas-wizard-0.0.1.dev0/pandas_wizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-14 14:39:44.000000 pandas-wizard-0.0.1.dev0/pandas_wizard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-14 14:39:45.080507 pandas-wizard-0.0.1.dev0/pandaswizard/
--rw-rw-rw-   0        0        0      462 2024-04-14 14:26:21.000000 pandas-wizard-0.0.1.dev0/pandaswizard/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-14 14:39:45.083506 pandas-wizard-0.0.1.dev0/setup.cfg
--rw-rw-rw-   0        0        0     1928 2024-04-14 14:24:50.000000 pandas-wizard-0.0.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:52:53.586762 pandas-wizard-1.0.0.dev0/
+-rw-rw-rw-   0        0        0     2739 2024-04-19 15:49:36.000000 pandas-wizard-1.0.0.dev0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2024-04-19 13:29:01.000000 pandas-wizard-1.0.0.dev0/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-19 13:29:01.000000 pandas-wizard-1.0.0.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3296 2024-04-19 15:52:53.585757 pandas-wizard-1.0.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     1788 2024-04-19 13:59:54.000000 pandas-wizard-1.0.0.dev0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 15:52:53.584758 pandas-wizard-1.0.0.dev0/pandas_wizard.egg-info/
+-rw-rw-rw-   0        0        0     3296 2024-04-19 15:52:53.000000 pandas-wizard-1.0.0.dev0/pandas_wizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-04-19 15:52:53.000000 pandas-wizard-1.0.0.dev0/pandas_wizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:52:53.000000 pandas-wizard-1.0.0.dev0/pandas_wizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 15:52:53.000000 pandas-wizard-1.0.0.dev0/pandas_wizard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:52:53.583757 pandas-wizard-1.0.0.dev0/pandaswizard/
+-rw-rw-rw-   0        0        0      565 2024-04-19 15:19:29.000000 pandas-wizard-1.0.0.dev0/pandaswizard/__init__.py
+-rw-rw-rw-   0        0        0     5037 2024-04-19 15:17:56.000000 pandas-wizard-1.0.0.dev0/pandaswizard/aggregate.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:52:53.586762 pandas-wizard-1.0.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     2045 2024-04-19 15:50:53.000000 pandas-wizard-1.0.0.dev0/setup.py
```

### Comparing `pandas-wizard-0.0.1.dev0/LICENSE` & `pandas-wizard-1.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-wizard-0.0.1.dev0/PKG-INFO` & `pandas-wizard-1.0.0.dev0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pandas-wizard
-Version: 0.0.1.dev0
+Version: 1.0.0.dev0
 Summary: Utility Functions, Wrappers for pandas Module
 Home-page: https://github.com/sharkutilities/pandas-wizard
 Author: shark-utilities developers
 Author-email: neuralNOD@outlook.com
 Project-URL: Issue Tracker, https://github.com/sharkutilities/pandas-wizard/issues
-Keywords: pandas,utility,utilities,util,utils,wrappers,data science,data analysis,data scientist,data analyst
+Keywords: pandas,utility,utilities,util,utils,wrappers,data science,data analysis,data scientist,data analyst,statistics,percentile,quantile,probability
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
@@ -38,8 +38,32 @@
 unless needed to enhance performance.
 
 This is a relatively new repository, and if you find any performance or improvement scope please check the
 [contributing guidelines](https://github.com/sharkutilities/.github/blob/master/.github/CONTRIBUTING.md) for the organization.
 All help and criticism are appreciated. If you find any additional use cases please create a pull request or submit for a
 new feature.
 
+## Getting Started
+
+The source code is currently hosted at GitHub: [**sharkutilities/pandas-wizard**](https://github.com/sharkutilities/pandas-wizard).
+The binary installers for the latest release are available at the [Python Package Index (PyPI)](https://pypi.org/project/pandas-wizard/).
+
+```bash
+pip install -U pandas-wizard
+```
+
+The list of changes between each release is available [here](./CHANGELOG.md).
+
+The purpose of the below guide is to illustrate the main features of **pandas-wizard** and assume the working knowledge of
+the [`pandas`](https://pypi.org/project/pandas/) module and use cases. The below example calculates the percentile of
+`pandas.DataFrameGroupBy` object using [`np.percentile`](https://numpy.org/doc/stable/reference/generated/numpy.percentile.html).
+
+```python
+import pandaswizard as pdw
+
+percentiles = df.groupby("group").agg({"A" : pdw.percentile(0.05)})
+percentiles.head()
+```
+
+The above function calculates the 0.05, i.e., 5th percentile of the feature "A" based on the grouped column "group" from the data frame.
+
 </div>
```

### Comparing `pandas-wizard-0.0.1.dev0/pandas_wizard.egg-info/PKG-INFO` & `pandas-wizard-1.0.0.dev0/pandas_wizard.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pandas-wizard
-Version: 0.0.1.dev0
+Version: 1.0.0.dev0
 Summary: Utility Functions, Wrappers for pandas Module
 Home-page: https://github.com/sharkutilities/pandas-wizard
 Author: shark-utilities developers
 Author-email: neuralNOD@outlook.com
 Project-URL: Issue Tracker, https://github.com/sharkutilities/pandas-wizard/issues
-Keywords: pandas,utility,utilities,util,utils,wrappers,data science,data analysis,data scientist,data analyst
+Keywords: pandas,utility,utilities,util,utils,wrappers,data science,data analysis,data scientist,data analyst,statistics,percentile,quantile,probability
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
@@ -38,8 +38,32 @@
 unless needed to enhance performance.
 
 This is a relatively new repository, and if you find any performance or improvement scope please check the
 [contributing guidelines](https://github.com/sharkutilities/.github/blob/master/.github/CONTRIBUTING.md) for the organization.
 All help and criticism are appreciated. If you find any additional use cases please create a pull request or submit for a
 new feature.
 
+## Getting Started
+
+The source code is currently hosted at GitHub: [**sharkutilities/pandas-wizard**](https://github.com/sharkutilities/pandas-wizard).
+The binary installers for the latest release are available at the [Python Package Index (PyPI)](https://pypi.org/project/pandas-wizard/).
+
+```bash
+pip install -U pandas-wizard
+```
+
+The list of changes between each release is available [here](./CHANGELOG.md).
+
+The purpose of the below guide is to illustrate the main features of **pandas-wizard** and assume the working knowledge of
+the [`pandas`](https://pypi.org/project/pandas/) module and use cases. The below example calculates the percentile of
+`pandas.DataFrameGroupBy` object using [`np.percentile`](https://numpy.org/doc/stable/reference/generated/numpy.percentile.html).
+
+```python
+import pandaswizard as pdw
+
+percentiles = df.groupby("group").agg({"A" : pdw.percentile(0.05)})
+percentiles.head()
+```
+
+The above function calculates the 0.05, i.e., 5th percentile of the feature "A" based on the grouped column "group" from the data frame.
+
 </div>
```

### Comparing `pandas-wizard-0.0.1.dev0/setup.py` & `pandas-wizard-1.0.0.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,11 +41,13 @@
     project_urls = {
         "Issue Tracker" : "https://github.com/sharkutilities/pandas-wizard/issues"
     },
     keywords = [
         # keywords for finding the package::
         "pandas", "utility", "utilities", "util", "utils",
         # keywords for finding the package relevant to usecases::
-        "wrappers", "data science", "data analysis", "data scientist", "data analyst"
+        "wrappers", "data science", "data analysis", "data scientist", "data analyst",
+        # keywords as per available functionalities::
+        "statistics", "percentile", "quantile", "probability"
     ],
     python_requires = ">=3.8"
 )
```

