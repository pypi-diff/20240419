# Comparing `tmp/ldap2jira-1.2.3.tar.gz` & `tmp/ldap2jira-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldap2jira-1.2.3.tar", last modified: Wed Aug 23 12:31:22 2023, max compression
+gzip compressed data, was "ldap2jira-1.2.4.tar", last modified: Fri Apr 19 12:53:24 2024, max compression
```

## Comparing `ldap2jira-1.2.3.tar` & `ldap2jira-1.2.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:22.751388 ldap2jira-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/.github/workflows/pypi-upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/ldap2jira/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/ldap2jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/ldap2jira/ldap_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/ldap2jira/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-23 12:31:22.000000 ldap2jira-1.2.3/ldap2jira/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/ldap2jira.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-23 12:31:22.000000 ldap2jira-1.2.3/ldap2jira.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-23 12:31:22.000000 ldap2jira-1.2.3/ldap2jira.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 12:31:22.000000 ldap2jira-1.2.3/ldap2jira.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-23 12:31:22.000000 ldap2jira-1.2.3/ldap2jira.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-23 12:31:22.000000 ldap2jira-1.2.3/ldap2jira.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:22.755388 ldap2jira-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/tests/test_ldap2jira.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/tests/test_map.csv
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/tests/test_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-23 12:31:05.000000 ldap2jira-1.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:24.848942 ldap2jira-1.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:24.840942 ldap2jira-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:24.844941 ldap2jira-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/.github/workflows/pypi-upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-19 12:53:24.848942 ldap2jira-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:24.844941 ldap2jira-1.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:24.844941 ldap2jira-1.2.4/ldap2jira/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/ldap2jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/ldap2jira/ldap_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/ldap2jira/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 12:53:24.000000 ldap2jira-1.2.4/ldap2jira/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:24.848942 ldap2jira-1.2.4/ldap2jira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-19 12:53:24.000000 ldap2jira-1.2.4/ldap2jira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 12:53:24.000000 ldap2jira-1.2.4/ldap2jira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:53:24.000000 ldap2jira-1.2.4/ldap2jira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 12:53:24.000000 ldap2jira-1.2.4/ldap2jira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 12:53:24.000000 ldap2jira-1.2.4/ldap2jira.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-19 12:53:24.848942 ldap2jira-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:24.848942 ldap2jira-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/tests/test_ldap2jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/tests/test_map.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/tests/test_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 12:53:13.000000 ldap2jira-1.2.4/tox.ini
```

### Comparing `ldap2jira-1.2.3/.github/workflows/pypi-upload.yml` & `ldap2jira-1.2.4/.github/workflows/pypi-upload.yml`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/.github/workflows/test.yml` & `ldap2jira-1.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/LICENSE` & `ldap2jira-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/PKG-INFO` & `ldap2jira-1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ldap2jira
-Version: 1.2.3
+Version: 1.2.4
 Summary: Set of utilities for finding jira accounts with LDAP check and optional file map
 Home-page: https://github.com/RedHat-Eng-PGM/python-ldap2jira
 Author: RH PLM
 Author-email: pp-dev-list@redhat.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/RedHat-Eng-PGM/python-ldap2jira/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jira
+Requires-Dist: python-ldap
 
 # python-ldap2jira
 
 Set of utilities for finding jira accounts with LDAP check and optional file map.
 
 [![Test](https://github.com/RedHat-Eng-PGM/python-ldap2jira/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/RedHat-Eng-PGM/python-ldap2jira/actions/workflows/test.yml)
 [![Coverage](https://codecov.io/gh/RedHat-Eng-PGM/python-ldap2jira/branch/master/graph/badge.svg?token=WCXC71LMUA)](https://codecov.io/gh/RedHat-Eng-PGM/python-ldap2jira)
```

### Comparing `ldap2jira-1.2.3/README.md` & `ldap2jira-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/docs/Makefile` & `ldap2jira-1.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/docs/conf.py` & `ldap2jira-1.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/docs/index.rst` & `ldap2jira-1.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/docs/make.bat` & `ldap2jira-1.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/ldap2jira/ldap_lookup.py` & `ldap2jira-1.2.4/ldap2jira/ldap_lookup.py`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/ldap2jira/map.py` & `ldap2jira-1.2.4/ldap2jira/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,19 +357,20 @@
 
             self._update_user(
                 user_dict, username, 'ambiguous',
                 'Possible matches: ' + ', '.join(user_dict['jira-results']))
 
         return user_dict
 
-    def find_jira_accounts(self, usernames: List[str]) -> dict:
+    def find_jira_accounts(self, usernames: List[str], max_workers: int = None) -> dict:
         """ Finds matching JIRA account for given user names
 
         Args:
             usernames: List of user names
+            max_workers: The maximum number of threads
 
         Returns:
             A dict with user names as keys and match results dict as values
 
             Possible match result keys:
                 status:
                     found: Found good match in JIRA
@@ -400,15 +401,15 @@
 
             }
         """
         users = {}
 
         self.map.update(self.load_map(self.map_file))
 
-        with ThreadPoolExecutor(thread_name_prefix='W') as executor:
+        with ThreadPoolExecutor(thread_name_prefix='W', max_workers=max_workers) as executor:
 
             f_users_d = {executor.submit(self._process_username, username)
                          for username in usernames}
 
             for f_user_d in as_completed(f_users_d):
                 user_d = f_user_d.result()
```

### Comparing `ldap2jira-1.2.3/ldap2jira.egg-info/PKG-INFO` & `ldap2jira-1.2.4/ldap2jira.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ldap2jira
-Version: 1.2.3
+Version: 1.2.4
 Summary: Set of utilities for finding jira accounts with LDAP check and optional file map
 Home-page: https://github.com/RedHat-Eng-PGM/python-ldap2jira
 Author: RH PLM
 Author-email: pp-dev-list@redhat.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/RedHat-Eng-PGM/python-ldap2jira/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jira
+Requires-Dist: python-ldap
 
 # python-ldap2jira
 
 Set of utilities for finding jira accounts with LDAP check and optional file map.
 
 [![Test](https://github.com/RedHat-Eng-PGM/python-ldap2jira/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/RedHat-Eng-PGM/python-ldap2jira/actions/workflows/test.yml)
 [![Coverage](https://codecov.io/gh/RedHat-Eng-PGM/python-ldap2jira/branch/master/graph/badge.svg?token=WCXC71LMUA)](https://codecov.io/gh/RedHat-Eng-PGM/python-ldap2jira)
```

### Comparing `ldap2jira-1.2.3/ldap2jira.egg-info/SOURCES.txt` & `ldap2jira-1.2.4/ldap2jira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/setup.cfg` & `ldap2jira-1.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ldap2jira-1.2.3/tests/test_ldap2jira.py` & `ldap2jira-1.2.4/tests/test_ldap2jira.py`

 * *Files identical despite different names*

