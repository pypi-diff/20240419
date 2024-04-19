# Comparing `tmp/apk-signer-1.1.2.tar.gz` & `tmp/apk_signer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apk-signer-1.1.2.tar", last modified: Sat Jul 22 11:13:17 2023, max compression
+gzip compressed data, was "apk_signer-1.1.3.tar", last modified: Fri Apr 19 13:34:30 2024, max compression
```

## Comparing `apk-signer-1.1.2.tar` & `apk_signer-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/
--rw-r--r--   0 ksg        (501) staff       (20)     5459 2023-07-22 11:13:17.000000 apk-signer-1.1.2/PKG-INFO
--rw-r--r--   0 ksg        (501) staff       (20)     4431 2023-07-22 11:12:31.000000 apk-signer-1.1.2/README.rst
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer/
--rw-r--r--   0 ksg        (501) staff       (20)       21 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/__init__.py
--rw-r--r--   0 ksg        (501) staff       (20)     2782 2023-07-22 10:33:59.000000 apk-signer-1.1.2/apk_signer/apksigner.py
--rw-r--r--   0 ksg        (501) staff       (20)      414 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/config.py
--rw-r--r--   0 ksg        (501) staff       (20)     2259 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/pyapksigner.jks
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer/scripts/
--rw-r--r--   0 ksg        (501) staff       (20)        0 2020-02-17 16:20:04.000000 apk-signer-1.1.2/apk_signer/scripts/__init__.py
--rw-r--r--   0 ksg        (501) staff       (20)     1528 2023-07-22 10:29:15.000000 apk-signer-1.1.2/apk_signer/scripts/launcher.py
-drwxr-xr-x   0 ksg        (501) staff       (20)        0 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/
--rw-r--r--   0 ksg        (501) staff       (20)     5459 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/PKG-INFO
--rw-r--r--   0 ksg        (501) staff       (20)      382 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/SOURCES.txt
--rw-r--r--   0 ksg        (501) staff       (20)        1 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/dependency_links.txt
--rw-r--r--   0 ksg        (501) staff       (20)       64 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/entry_points.txt
--rw-r--r--   0 ksg        (501) staff       (20)       17 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/requires.txt
--rw-r--r--   0 ksg        (501) staff       (20)       11 2023-07-22 11:13:17.000000 apk-signer-1.1.2/apk_signer.egg-info/top_level.txt
--rw-r--r--   0 ksg        (501) staff       (20)       38 2023-07-22 11:13:17.000000 apk-signer-1.1.2/setup.cfg
--rw-r--r--   0 ksg        (501) staff       (20)     1046 2023-07-22 11:13:14.000000 apk-signer-1.1.2/setup.py
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2024-04-19 13:34:30.015360 apk_signer-1.1.3/
+-rw-r--r--   0 ksg        (501) staff       (20)     1074 2024-04-19 13:18:33.000000 apk_signer-1.1.3/LICENSE
+-rw-r--r--   0 ksg        (501) staff       (20)     4874 2024-04-19 13:34:30.015185 apk_signer-1.1.3/PKG-INFO
+-rw-r--r--   0 ksg        (501) staff       (20)     4417 2024-04-19 13:18:33.000000 apk_signer-1.1.3/README.rst
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2024-04-19 13:34:30.014039 apk_signer-1.1.3/apk_signer/
+-rw-r--r--   0 ksg        (501) staff       (20)       21 2024-04-19 13:18:33.000000 apk_signer-1.1.3/apk_signer/__init__.py
+-rw-r--r--   0 ksg        (501) staff       (20)     2782 2024-04-19 13:18:33.000000 apk_signer-1.1.3/apk_signer/apksigner.py
+-rw-r--r--   0 ksg        (501) staff       (20)      414 2024-04-19 13:18:33.000000 apk_signer-1.1.3/apk_signer/config.py
+-rw-r--r--   0 ksg        (501) staff       (20)     2259 2024-04-19 13:18:33.000000 apk_signer-1.1.3/apk_signer/pyapksigner.jks
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2024-04-19 13:34:30.014827 apk_signer-1.1.3/apk_signer/scripts/
+-rw-r--r--   0 ksg        (501) staff       (20)        0 2024-04-19 13:18:33.000000 apk_signer-1.1.3/apk_signer/scripts/__init__.py
+-rw-r--r--   0 ksg        (501) staff       (20)     1529 2024-04-19 13:18:33.000000 apk_signer-1.1.3/apk_signer/scripts/launcher.py
+drwxr-xr-x   0 ksg        (501) staff       (20)        0 2024-04-19 13:34:30.014959 apk_signer-1.1.3/apk_signer.egg-info/
+-rw-r--r--   0 ksg        (501) staff       (20)     4874 2024-04-19 13:34:29.000000 apk_signer-1.1.3/apk_signer.egg-info/PKG-INFO
+-rw-r--r--   0 ksg        (501) staff       (20)      390 2024-04-19 13:34:29.000000 apk_signer-1.1.3/apk_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 ksg        (501) staff       (20)        1 2024-04-19 13:34:29.000000 apk_signer-1.1.3/apk_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       63 2024-04-19 13:34:29.000000 apk_signer-1.1.3/apk_signer.egg-info/entry_points.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       17 2024-04-19 13:34:29.000000 apk_signer-1.1.3/apk_signer.egg-info/requires.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       11 2024-04-19 13:34:29.000000 apk_signer-1.1.3/apk_signer.egg-info/top_level.txt
+-rw-r--r--   0 ksg        (501) staff       (20)       38 2024-04-19 13:34:30.015398 apk_signer-1.1.3/setup.cfg
+-rw-r--r--   0 ksg        (501) staff       (20)     1046 2024-04-19 13:18:49.000000 apk_signer-1.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apk-signer-1.1.2/PKG-INFO` & `apk_signer-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 Metadata-Version: 2.1
 Name: apk-signer
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sign the apk file
 Home-page: https://github.com/ksg97031/apk-signer
 Author: ksg97031
 Author-email: ksg97031@gmail.com
-License: UNKNOWN
-Description: apk-signer
-        ============
-        
-        Easy signing with apk-signer
-        
-        Installation
-        ------------
-        
-        |Py-Versions| |PyPI-Downloads|
-        
-        .. code:: sh
-        
-            pip install apk-signer
-            
-        Prerequirement
-        ----------------
-        | Download: `Android SDK <https://developer.android.com/studio/releases/platform-tools?hl=ko>`_
-        
-        Usage
-        ------------
-        
-        .. code:: sh
-        
-            $ apk-signer {APK_PATH}
-               
-        
-        .. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/apk-signer/master?logo=coveralls
-           :target: https://coveralls.io/github/ksg97031/apk-signer
-        .. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/apk-signer/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/ksg97031/apk-signer
-        .. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
-           :target: https://www.codacy.com/gh/ksg97031/apk-signer/dashboard
-        .. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
-           :target: https://bestpractices.coreinfrastructure.org/projects/3264
-        .. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/apk-signer.svg?maxAge=86400&logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/releases
-        .. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/network
-        .. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/stargazers
-        .. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/apk-signer.svg?logo=git&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/graphs/commit-activity
-        .. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/issues?q=
-        .. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/pulls
-        .. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/graphs/contributors
-        .. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/apk-signer/master.svg?logo=github&logoColor=white&label=pushed
-           :target: https://github.com/ksg97031/apk-signer/pulse
-        .. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
-           :target: https://cdcl.ml/sponsor
-        .. |PyPI-Downloads| image:: https://static.pepy.tech/badge/apk-signer
-           :target: https://pepy.tech/project/apk-signer
-        .. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/apk-signer
-           :target: https://pypi.org/project/apk-signer
-        .. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/apk-signer.svg?label=conda-forge&logo=conda-forge
-           :target: https://anaconda.org/conda-forge/apk-signer
-        .. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/pkgs/container/apk-signer
-        .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/apk-signer.svg?logo=koding&logoColor=white
-           :target: https://libraries.io/pypi/apk-signer
-        .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/apk-signer.svg?logo=koding&logoColor=white
-            :target: https://github.com/ksg97031/apk-signer/network/dependents
-        .. |OpenHub-Status| image:: https://www.openhub.net/p/apk-signer/widgets/project_thin_badge?format=gif
-           :target: https://www.openhub.net/p/apk-signer?ref=Thin+badge
-        .. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
-           :target: https://github.com/vinta/awesome-python
-        .. |LICENCE| image:: https://img.shields.io/pypi/l/apk-signer.svg
-           :target: https://raw.githubusercontent.com/ksg97031/apk-signer/master/LICENCE
-        .. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
-           :target: https://doi.org/10.5281/zenodo.595120
-        .. |binder-demo| image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/ksg97031/apk-signer/master?filepath=DEMO.ipynb
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: androguard
+
+apk-signer
+============
+
+Easy signing with apk-signer
+
+Installation
+------------
+
+|PyPI-Downloads|
+
+.. code:: sh
+
+    pip install apk-signer
+    
+Prerequirement
+----------------
+| Download: `Android SDK <https://developer.android.com/studio/releases/platform-tools?hl=ko>`_
+
+Usage
+------------
+
+.. code:: sh
+
+    $ apk-signer {APK_PATH}
+       
+
+.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/apk-signer/master?logo=coveralls
+   :target: https://coveralls.io/github/ksg97031/apk-signer
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/apk-signer/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/ksg97031/apk-signer
+.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
+   :target: https://www.codacy.com/gh/ksg97031/apk-signer/dashboard
+.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
+   :target: https://bestpractices.coreinfrastructure.org/projects/3264
+.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/apk-signer.svg?maxAge=86400&logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/releases
+.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/network
+.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/stargazers
+.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/apk-signer.svg?logo=git&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/graphs/commit-activity
+.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/issues?q=
+.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/pulls
+.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/graphs/contributors
+.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/apk-signer/master.svg?logo=github&logoColor=white&label=pushed
+   :target: https://github.com/ksg97031/apk-signer/pulse
+.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
+   :target: https://cdcl.ml/sponsor
+.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/apk-signer
+   :target: https://pepy.tech/project/apk-signer
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/apk-signer
+   :target: https://pypi.org/project/apk-signer
+.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/apk-signer.svg?label=conda-forge&logo=conda-forge
+   :target: https://anaconda.org/conda-forge/apk-signer
+.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/pkgs/container/apk-signer
+.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/apk-signer.svg?logo=koding&logoColor=white
+   :target: https://libraries.io/pypi/apk-signer
+.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/apk-signer.svg?logo=koding&logoColor=white
+    :target: https://github.com/ksg97031/apk-signer/network/dependents
+.. |OpenHub-Status| image:: https://www.openhub.net/p/apk-signer/widgets/project_thin_badge?format=gif
+   :target: https://www.openhub.net/p/apk-signer?ref=Thin+badge
+.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
+   :target: https://github.com/vinta/awesome-python
+.. |LICENCE| image:: https://img.shields.io/pypi/l/apk-signer.svg
+   :target: https://raw.githubusercontent.com/ksg97031/apk-signer/master/LICENCE
+.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
+   :target: https://doi.org/10.5281/zenodo.595120
+.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/ksg97031/apk-signer/master?filepath=DEMO.ipynb
```

### Comparing `apk-signer-1.1.2/README.rst` & `apk_signer-1.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ============
 
 Easy signing with apk-signer
 
 Installation
 ------------
 
-|Py-Versions| |PyPI-Downloads|
+|PyPI-Downloads|
 
 .. code:: sh
 
     pip install apk-signer
     
 Prerequirement
 ----------------
```

### Comparing `apk-signer-1.1.2/apk_signer/apksigner.py` & `apk_signer-1.1.3/apk_signer/apksigner.py`

 * *Files identical despite different names*

### Comparing `apk-signer-1.1.2/apk_signer/pyapksigner.jks` & `apk_signer-1.1.3/apk_signer/pyapksigner.jks`

 * *Files identical despite different names*

### Comparing `apk-signer-1.1.2/apk_signer/scripts/launcher.py` & `apk_signer-1.1.3/apk_signer/scripts/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @click.option('--key_path', default='pyapksigner.jks')
 @click.argument('apk')
 def cli(apk: str, default: bool, key_path: str, key_alias: str, key_pass: str, ks_pass: str, run: bool, run_only: bool):
     apk_path = apk
     if not run_only:
         if key_path == 'pyapksigner.jks':
             if not default:
-                print("Warning: Pass the --key_path, --key_alias, --key_pass, and --ks_pass parameters if you want to use your own keystore."
+                print("Warning: Pass the --key_path, --key_alias, --key_pass, and --ks_pass parameters if you want to use your own keystore.")
             key_path = str(config.ROOT_DIR.joinpath(key_path).resolve())
 
         apk_path = launcher(apk, key_path, key_alias, key_pass, ks_pass)
 
     if run or run_only:
        apk = APK(apk_path)
```

### Comparing `apk-signer-1.1.2/apk_signer.egg-info/PKG-INFO` & `apk_signer-1.1.3/apk_signer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 Metadata-Version: 2.1
 Name: apk-signer
-Version: 1.1.2
+Version: 1.1.3
 Summary: Sign the apk file
 Home-page: https://github.com/ksg97031/apk-signer
 Author: ksg97031
 Author-email: ksg97031@gmail.com
-License: UNKNOWN
-Description: apk-signer
-        ============
-        
-        Easy signing with apk-signer
-        
-        Installation
-        ------------
-        
-        |Py-Versions| |PyPI-Downloads|
-        
-        .. code:: sh
-        
-            pip install apk-signer
-            
-        Prerequirement
-        ----------------
-        | Download: `Android SDK <https://developer.android.com/studio/releases/platform-tools?hl=ko>`_
-        
-        Usage
-        ------------
-        
-        .. code:: sh
-        
-            $ apk-signer {APK_PATH}
-               
-        
-        .. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/apk-signer/master?logo=coveralls
-           :target: https://coveralls.io/github/ksg97031/apk-signer
-        .. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/apk-signer/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/ksg97031/apk-signer
-        .. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
-           :target: https://www.codacy.com/gh/ksg97031/apk-signer/dashboard
-        .. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
-           :target: https://bestpractices.coreinfrastructure.org/projects/3264
-        .. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/apk-signer.svg?maxAge=86400&logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/releases
-        .. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/network
-        .. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/stargazers
-        .. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/apk-signer.svg?logo=git&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/graphs/commit-activity
-        .. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/issues?q=
-        .. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/pulls
-        .. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/apk-signer.svg?logo=github&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/graphs/contributors
-        .. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/apk-signer/master.svg?logo=github&logoColor=white&label=pushed
-           :target: https://github.com/ksg97031/apk-signer/pulse
-        .. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
-           :target: https://cdcl.ml/sponsor
-        .. |PyPI-Downloads| image:: https://static.pepy.tech/badge/apk-signer
-           :target: https://pepy.tech/project/apk-signer
-        .. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/apk-signer
-           :target: https://pypi.org/project/apk-signer
-        .. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/apk-signer.svg?label=conda-forge&logo=conda-forge
-           :target: https://anaconda.org/conda-forge/apk-signer
-        .. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
-           :target: https://github.com/ksg97031/apk-signer/pkgs/container/apk-signer
-        .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/apk-signer.svg?logo=koding&logoColor=white
-           :target: https://libraries.io/pypi/apk-signer
-        .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/apk-signer.svg?logo=koding&logoColor=white
-            :target: https://github.com/ksg97031/apk-signer/network/dependents
-        .. |OpenHub-Status| image:: https://www.openhub.net/p/apk-signer/widgets/project_thin_badge?format=gif
-           :target: https://www.openhub.net/p/apk-signer?ref=Thin+badge
-        .. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
-           :target: https://github.com/vinta/awesome-python
-        .. |LICENCE| image:: https://img.shields.io/pypi/l/apk-signer.svg
-           :target: https://raw.githubusercontent.com/ksg97031/apk-signer/master/LICENCE
-        .. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
-           :target: https://doi.org/10.5281/zenodo.595120
-        .. |binder-demo| image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/ksg97031/apk-signer/master?filepath=DEMO.ipynb
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: androguard
+
+apk-signer
+============
+
+Easy signing with apk-signer
+
+Installation
+------------
+
+|PyPI-Downloads|
+
+.. code:: sh
+
+    pip install apk-signer
+    
+Prerequirement
+----------------
+| Download: `Android SDK <https://developer.android.com/studio/releases/platform-tools?hl=ko>`_
+
+Usage
+------------
+
+.. code:: sh
+
+    $ apk-signer {APK_PATH}
+       
+
+.. |Coverage-Status| image:: https://img.shields.io/coveralls/github/ksg97031/apk-signer/master?logo=coveralls
+   :target: https://coveralls.io/github/ksg97031/apk-signer
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/ksg97031/apk-signer/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/ksg97031/apk-signer
+.. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/3f965571598f44549c7818f29cdcf177
+   :target: https://www.codacy.com/gh/ksg97031/apk-signer/dashboard
+.. |CII Best Practices| image:: https://bestpractices.coreinfrastructure.org/projects/3264/badge
+   :target: https://bestpractices.coreinfrastructure.org/projects/3264
+.. |GitHub-Status| image:: https://img.shields.io/github/tag/ksg97031/apk-signer.svg?maxAge=86400&logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/releases
+.. |GitHub-Forks| image:: https://img.shields.io/github/forks/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/network
+.. |GitHub-Stars| image:: https://img.shields.io/github/stars/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/stargazers
+.. |GitHub-Commits| image:: https://img.shields.io/github/commit-activity/y/ksg97031/apk-signer.svg?logo=git&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/graphs/commit-activity
+.. |GitHub-Issues| image:: https://img.shields.io/github/issues-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/issues?q=
+.. |GitHub-PRs| image:: https://img.shields.io/github/issues-pr-closed/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/pulls
+.. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/ksg97031/apk-signer.svg?logo=github&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/graphs/contributors
+.. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/ksg97031/apk-signer/master.svg?logo=github&logoColor=white&label=pushed
+   :target: https://github.com/ksg97031/apk-signer/pulse
+.. |Gift-Casper| image:: https://img.shields.io/badge/dynamic/json.svg?color=ff69b4&label=gifts%20received&prefix=%C2%A3&query=%24..sum&url=https%3A%2F%2Fcaspersci.uk.to%2Fgifts.json
+   :target: https://cdcl.ml/sponsor
+.. |PyPI-Downloads| image:: https://static.pepy.tech/badge/apk-signer
+   :target: https://pepy.tech/project/apk-signer
+.. |Py-Versions| image:: https://img.shields.io/pypi/pyversions/apk-signer
+   :target: https://pypi.org/project/apk-signer
+.. |Conda-Forge-Status| image:: https://img.shields.io/conda/v/conda-forge/apk-signer.svg?label=conda-forge&logo=conda-forge
+   :target: https://anaconda.org/conda-forge/apk-signer
+.. |Docker| image:: https://img.shields.io/badge/docker-pull-blue.svg?logo=docker&logoColor=white
+   :target: https://github.com/ksg97031/apk-signer/pkgs/container/apk-signer
+.. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/apk-signer.svg?logo=koding&logoColor=white
+   :target: https://libraries.io/pypi/apk-signer
+.. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/apk-signer.svg?logo=koding&logoColor=white
+    :target: https://github.com/ksg97031/apk-signer/network/dependents
+.. |OpenHub-Status| image:: https://www.openhub.net/p/apk-signer/widgets/project_thin_badge?format=gif
+   :target: https://www.openhub.net/p/apk-signer?ref=Thin+badge
+.. |awesome-python| image:: https://awesome.re/mentioned-badge.svg
+   :target: https://github.com/vinta/awesome-python
+.. |LICENCE| image:: https://img.shields.io/pypi/l/apk-signer.svg
+   :target: https://raw.githubusercontent.com/ksg97031/apk-signer/master/LICENCE
+.. |DOI| image:: https://img.shields.io/badge/DOI-10.5281/zenodo.595120-blue.svg
+   :target: https://doi.org/10.5281/zenodo.595120
+.. |binder-demo| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/ksg97031/apk-signer/master?filepath=DEMO.ipynb
```

### Comparing `apk-signer-1.1.2/setup.py` & `apk_signer-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apk-signer",
     python_requires='>=3.5',
-    version="1.1.2",
+    version="1.1.3",
     author="ksg97031",
     author_email="ksg97031@gmail.com",
     description="Sign the apk file",
     install_requires=['click', 'androguard'],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/ksg97031/apk-signer",
```

