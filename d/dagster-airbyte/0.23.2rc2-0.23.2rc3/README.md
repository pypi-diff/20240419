# Comparing `tmp/dagster-airbyte-0.23.2rc2.tar.gz` & `tmp/dagster-airbyte-0.23.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.23.2rc2.tar", last modified: Tue Apr 16 20:38:04 2024, max compression
+gzip compressed data, was "dagster-airbyte-0.23.2rc3.tar", last modified: Thu Apr 18 21:21:32 2024, max compression
```

## Comparing `dagster-airbyte-0.23.2rc2.tar` & `dagster-airbyte-0.23.2rc3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.484281 dagster-airbyte-0.23.2rc2/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 20:38:04.484281 dagster-airbyte-0.23.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.476281 dagster-airbyte-0.23.2rc2/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48304 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.480281 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.480281 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    34862 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14588 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    27040 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2823 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:38:04.476281 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 20:38:04.000000 dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-16 20:38:04.484281 dagster-airbyte-0.23.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1642 2024-04-16 20:26:55.000000 dagster-airbyte-0.23.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:21:32.783730 dagster-airbyte-0.23.2rc3/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-18 21:21:32.783730 dagster-airbyte-0.23.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:21:32.771730 dagster-airbyte-0.23.2rc3/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48304 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:21:32.775730 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:21:32.779730 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119751 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282772 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    34862 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14588 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    27040 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:21:32.775730 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-18 21:21:32.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2024-04-18 21:21:32.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:21:32.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-18 21:21:32.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:21:32.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-18 21:21:32.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-18 21:21:32.000000 dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-18 21:21:32.783730 dagster-airbyte-0.23.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-04-18 21:10:09.000000 dagster-airbyte-0.23.2rc3/setup.py
```

### Comparing `dagster-airbyte-0.23.2rc2/LICENSE` & `dagster-airbyte-0.23.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/PKG-INFO` & `dagster-airbyte-0.23.2rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/__init__.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

```diff
@@ -1159,15 +1159,15 @@
 
         Args:
             name (str): The name of the destination.
             credentials (Union[GoogleAnalyticsV4Source.AuthenticateViaGoogleOauth, GoogleAnalyticsV4Source.ServiceAccountKeyAuthentication]): Credentials for the service
             start_date (str): The date in the format YYYY-MM-DD. Any data before this date will not be replicated.
             view_id (str): The ID for the Google Analytics View you want to fetch data from. This can be found from the Google Analytics Account Explorer.
             custom_reports (Optional[str]): A JSON array describing the custom reports you want to sync from Google Analytics. See the docs for more information about the exact format you can use to fill out this field.
-            window_in_days (Optional[int]): The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the the docs. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364.
+            window_in_days (Optional[int]): The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the docs. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364.
         """
         self.credentials = check.inst_param(
             credentials,
             "credentials",
             (
                 GoogleAnalyticsV4Source.AuthenticateViaGoogleOauth,
                 GoogleAnalyticsV4Source.ServiceAccountKeyAuthentication,
@@ -4720,15 +4720,15 @@
 
         Args:
             name (str): The name of the destination.
             property_id (str): A Google Analytics GA4 property identifier whose events are tracked. Specified in the URL path and not the body
             credentials (Union[GoogleAnalyticsDataApiSource.AuthenticateViaGoogleOauth, GoogleAnalyticsDataApiSource.ServiceAccountKeyAuthentication]): Credentials for the service
             date_ranges_start_date (str): The start date. One of the values Ndaysago, yesterday, today or in the format YYYY-MM-DD
             custom_reports (Optional[str]): A JSON array describing the custom reports you want to sync from Google Analytics. See the docs for more information about the exact format you can use to fill out this field.
-            window_in_days (Optional[int]): The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the the docs. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364.
+            window_in_days (Optional[int]): The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the docs. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364.
         """
         self.property_id = check.str_param(property_id, "property_id")
         self.credentials = check.inst_param(
             credentials,
             "credentials",
             (
                 GoogleAnalyticsDataApiSource.AuthenticateViaGoogleOauth,
@@ -5926,15 +5926,15 @@
         Args:
             name (str): The name of the destination.
             pardot_business_unit_id (str): Pardot Business ID, can be found at Setup > Pardot > Pardot Account Setup
             client_id (str): The Consumer Key that can be found when viewing your app in Salesforce
             client_secret (str): The Consumer Secret that can be found when viewing your app in Salesforce
             refresh_token (str): Salesforce Refresh Token used for Airbyte to access your Salesforce account. If you don't know what this is, follow this guide to retrieve it.
             start_date (Optional[str]): UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated. Leave blank to skip this filter
-            is_sandbox (Optional[bool]): Whether or not the the app is in a Salesforce sandbox. If you do not know what this, assume it is false.
+            is_sandbox (Optional[bool]): Whether or not the app is in a Salesforce sandbox. If you do not know what this, assume it is false.
         """
         self.pardot_business_unit_id = check.str_param(
             pardot_business_unit_id, "pardot_business_unit_id"
         )
         self.client_id = check.str_param(client_id, "client_id")
         self.client_secret = check.str_param(client_secret, "client_secret")
         self.refresh_token = check.str_param(refresh_token, "refresh_token")
```

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/ops.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/resources.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/types.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte/utils.py` & `dagster-airbyte-0.23.2rc3/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.2rc2
+Version: 0.23.2rc3
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.2rc2/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.23.2rc3/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.2rc2/setup.py` & `dagster-airbyte-0.23.2rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.2rc2",
+        "dagster==1.7.2rc3",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.23.2rc2",
+            "dagster-managed-elements==0.23.2rc3",
         ],
     },
 )
```

