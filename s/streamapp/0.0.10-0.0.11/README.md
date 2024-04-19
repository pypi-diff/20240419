# Comparing `tmp/streamapp-0.0.10.tar.gz` & `tmp/streamapp-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamapp-0.0.10.tar", last modified: Tue Apr 16 23:17:36 2024, max compression
+gzip compressed data, was "streamapp-0.0.11.tar", last modified: Fri Apr 19 00:34:53 2024, max compression
```

## Comparing `streamapp-0.0.10.tar` & `streamapp-0.0.11.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 23:17:36.097663 streamapp-0.0.10/
--rw-rw-rw-   0        0        0     1086 2024-04-12 00:49:21.000000 streamapp-0.0.10/LICENSE
--rw-rw-rw-   0        0        0     2102 2024-04-16 23:17:36.097663 streamapp-0.0.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 23:17:36.058000 streamapp-0.0.10/scr/
-drwxrwxrwx   0        0        0        0 2024-04-16 23:17:36.088953 streamapp-0.0.10/scr/streamapp/
--rw-rw-rw-   0        0        0     1096 2024-04-14 14:05:21.000000 streamapp-0.0.10/scr/streamapp/__init__.py
--rw-rw-rw-   0        0        0     3809 2024-04-12 00:49:21.000000 streamapp-0.0.10/scr/streamapp/authenticator.py
--rw-rw-rw-   0        0        0     2834 2024-04-14 15:09:59.000000 streamapp-0.0.10/scr/streamapp/cards.py
--rw-rw-rw-   0        0        0     5394 2024-04-14 00:56:10.000000 streamapp-0.0.10/scr/streamapp/enviroment_selector.py
--rw-rw-rw-   0        0        0     7410 2024-04-12 00:49:21.000000 streamapp-0.0.10/scr/streamapp/report_generator.py
--rw-rw-rw-   0        0        0     7768 2024-04-15 03:19:40.000000 streamapp-0.0.10/scr/streamapp/requests.py
--rw-rw-rw-   0        0        0     2062 2024-04-14 02:29:37.000000 streamapp-0.0.10/scr/streamapp/roles.py
--rw-rw-rw-   0        0        0    10733 2024-04-14 01:00:39.000000 streamapp-0.0.10/scr/streamapp/snow_class.py
--rw-rw-rw-   0        0        0     3077 2024-04-14 16:11:09.000000 streamapp-0.0.10/scr/streamapp/subpages.py
--rw-rw-rw-   0        0        0     2211 2024-04-12 00:49:21.000000 streamapp-0.0.10/scr/streamapp/utils.py
--rw-rw-rw-   0        0        0     2702 2024-04-12 00:49:21.000000 streamapp-0.0.10/scr/streamapp/validators.py
-drwxrwxrwx   0        0        0        0 2024-04-16 23:17:36.091520 streamapp-0.0.10/scr/streamapp.egg-info/
--rw-rw-rw-   0        0        0     2102 2024-04-16 23:17:35.000000 streamapp-0.0.10/scr/streamapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2024-04-16 23:17:35.000000 streamapp-0.0.10/scr/streamapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 23:17:35.000000 streamapp-0.0.10/scr/streamapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2024-04-16 23:17:35.000000 streamapp-0.0.10/scr/streamapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 23:17:35.000000 streamapp-0.0.10/scr/streamapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 23:17:36.098676 streamapp-0.0.10/setup.cfg
--rw-rw-rw-   0        0        0     1043 2024-04-16 23:00:29.000000 streamapp-0.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 00:34:53.223415 streamapp-0.0.11/
+-rw-rw-rw-   0        0        0     1086 2024-04-12 00:49:21.000000 streamapp-0.0.11/LICENSE
+-rw-rw-rw-   0        0        0     2163 2024-04-19 00:34:53.223415 streamapp-0.0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 00:34:53.182592 streamapp-0.0.11/scr/
+drwxrwxrwx   0        0        0        0 2024-04-19 00:34:53.211324 streamapp-0.0.11/scr/streamapp/
+-rw-rw-rw-   0        0        0     1096 2024-04-14 14:05:21.000000 streamapp-0.0.11/scr/streamapp/__init__.py
+-rw-rw-rw-   0        0        0     3809 2024-04-12 00:49:21.000000 streamapp-0.0.11/scr/streamapp/authenticator.py
+-rw-rw-rw-   0        0        0     2834 2024-04-14 15:09:59.000000 streamapp-0.0.11/scr/streamapp/cards.py
+-rw-rw-rw-   0        0        0     5394 2024-04-14 00:56:10.000000 streamapp-0.0.11/scr/streamapp/enviroment_selector.py
+-rw-rw-rw-   0        0        0     7410 2024-04-12 00:49:21.000000 streamapp-0.0.11/scr/streamapp/report_generator.py
+-rw-rw-rw-   0        0        0     7768 2024-04-15 03:19:40.000000 streamapp-0.0.11/scr/streamapp/requests.py
+-rw-rw-rw-   0        0        0     2062 2024-04-14 02:29:37.000000 streamapp-0.0.11/scr/streamapp/roles.py
+-rw-rw-rw-   0        0        0    10660 2024-04-19 00:17:19.000000 streamapp-0.0.11/scr/streamapp/snow_class.py
+-rw-rw-rw-   0        0        0     3077 2024-04-14 16:11:09.000000 streamapp-0.0.11/scr/streamapp/subpages.py
+-rw-rw-rw-   0        0        0     2211 2024-04-12 00:49:21.000000 streamapp-0.0.11/scr/streamapp/utils.py
+-rw-rw-rw-   0        0        0     2796 2024-04-19 00:23:32.000000 streamapp-0.0.11/scr/streamapp/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-19 00:34:53.220416 streamapp-0.0.11/scr/streamapp.egg-info/
+-rw-rw-rw-   0        0        0     2163 2024-04-19 00:34:52.000000 streamapp-0.0.11/scr/streamapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2024-04-19 00:34:52.000000 streamapp-0.0.11/scr/streamapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 00:34:52.000000 streamapp-0.0.11/scr/streamapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2024-04-19 00:34:52.000000 streamapp-0.0.11/scr/streamapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-19 00:34:52.000000 streamapp-0.0.11/scr/streamapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 00:34:53.224506 streamapp-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-19 00:30:19.000000 streamapp-0.0.11/setup.py
```

### Comparing `streamapp-0.0.10/LICENSE` & `streamapp-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/PKG-INFO` & `streamapp-0.0.11/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: streamapp
-Version: 0.0.10
+Version: 0.0.11
 Summary: Base modules to use in a Streamlit basic project
 Home-page: https://github.com/nmrls/streamapp_utils
 Author: nmrls
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # streamapp
 
 Base modules to use in a Streamlit project.
 
@@ -36,15 +36,16 @@
 openpyxl==3.1.2
 pydantic>=2.5.3
 ```
 
 # Secrets file
 ```
 # environment variables
-key = key for hased passwords with Fernet
+key = streamlit cookies key for auth module
+snow_key = key for hased snowflake password with Fernet
 queries_path = 'static/queries'  # your folder queries path
 utils_files = 'static/consume'  # your static files path
 admin_contact = 'admin@admin.com'  # show contact if something went wrong 
 
 # snowflake credentials
 # see snowflake documentation
 [SNOW_SERVER]
```

### Comparing `streamapp-0.0.10/scr/streamapp/__init__.py` & `streamapp-0.0.11/scr/streamapp/__init__.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/authenticator.py` & `streamapp-0.0.11/scr/streamapp/authenticator.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/cards.py` & `streamapp-0.0.11/scr/streamapp/cards.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/enviroment_selector.py` & `streamapp-0.0.11/scr/streamapp/enviroment_selector.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/report_generator.py` & `streamapp-0.0.11/scr/streamapp/report_generator.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/requests.py` & `streamapp-0.0.11/scr/streamapp/requests.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/roles.py` & `streamapp-0.0.11/scr/streamapp/roles.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/snow_class.py` & `streamapp-0.0.11/scr/streamapp/snow_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,15 @@
         Args:
             credentials: The Snowflake credential from .secrets/toml
 
         Returns:
             A dict with the credentials checked
         """
         try:
-            if secrets.get('key') and \
-                    not credentials.get('authenticator') == 'externalbrowser':
+            if secrets.get('snow_key', False):
                 token = Fernet(secrets.key.encode()).decrypt(
                     credentials.get('password', '').encode()
                 ).decode()
                 credentials.pop('password')
                 credentials.update(password=token)
         except Exception:
             credentials.pop('user')
```

### Comparing `streamapp-0.0.10/scr/streamapp/subpages.py` & `streamapp-0.0.11/scr/streamapp/subpages.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/utils.py` & `streamapp-0.0.11/scr/streamapp/utils.py`

 * *Files identical despite different names*

### Comparing `streamapp-0.0.10/scr/streamapp/validators.py` & `streamapp-0.0.11/scr/streamapp/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,8 +77,10 @@
                 'table': table,
                 'where': where,
                 'group_by': group_by
             },
             template=False,
             succes_confirmation=succes_confirmation
         )
+        if set(result).difference(columns):
+            result = DataFrame(columns=columns)
         return result
```

### Comparing `streamapp-0.0.10/scr/streamapp.egg-info/PKG-INFO` & `streamapp-0.0.11/scr/streamapp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: streamapp
-Version: 0.0.10
+Version: 0.0.11
 Summary: Base modules to use in a Streamlit basic project
 Home-page: https://github.com/nmrls/streamapp_utils
 Author: nmrls
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # streamapp
 
 Base modules to use in a Streamlit project.
 
@@ -36,15 +36,16 @@
 openpyxl==3.1.2
 pydantic>=2.5.3
 ```
 
 # Secrets file
 ```
 # environment variables
-key = key for hased passwords with Fernet
+key = streamlit cookies key for auth module
+snow_key = key for hased snowflake password with Fernet
 queries_path = 'static/queries'  # your folder queries path
 utils_files = 'static/consume'  # your static files path
 admin_contact = 'admin@admin.com'  # show contact if something went wrong 
 
 # snowflake credentials
 # see snowflake documentation
 [SNOW_SERVER]
```

### Comparing `streamapp-0.0.10/setup.py` & `streamapp-0.0.11/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('scr/README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='streamapp',
-    version='0.0.10',
+    version='0.0.11',
     author='nmrls',
     description='Base modules to use in a Streamlit basic project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nmrls/streamapp_utils',
     package_dir={'': 'scr'},
     packages=find_packages(where='scr'),
@@ -17,15 +17,15 @@
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3'
     ],
-    python_requires='>=3.10',
+    python_requires='>=3.10.0',
     install_requires=[
         'streamlit>=1.30.0',
         'pydantic>=2.5.3',
         'openpyxl==3.1.2',
         'snowflake-connector-python>=3.0.4',
         'streamlit-authenticator==0.2.2',
         'twine>=4.0.2'
```

