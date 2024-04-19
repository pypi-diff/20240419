# Comparing `tmp/open_exchange-0.1.9.tar.gz` & `tmp/open_exchange-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_exchange-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "open_exchange-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `open_exchange-0.1.9.tar` & `open_exchange-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       29 2024-03-05 16:34:03.069794 open_exchange-0.1.9/.github/CODEOWNERS
--rw-r--r--   0        0        0      172 2024-03-05 16:34:10.434965 open_exchange-0.1.9/.gitignore
--rw-r--r--   0        0        0      521 2024-04-09 17:08:56.595568 open_exchange-0.1.9/CHANGELOG.md
--rw-r--r--   0        0        0       99 2024-02-29 17:29:44.100867 open_exchange-0.1.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     1091 2024-02-29 17:29:44.101716 open_exchange-0.1.9/LICENSE.md
--rw-r--r--   0        0        0     1698 2024-03-20 15:26:18.626982 open_exchange-0.1.9/README.md
--rw-r--r--   0        0        0      892 2024-04-09 17:08:56.595669 open_exchange-0.1.9/cortex.yaml
--rw-r--r--   0        0        0     1405 2024-04-09 17:08:56.595799 open_exchange-0.1.9/examples/property_details.py
--rw-r--r--   0        0        0     1209 2024-04-09 17:08:56.595920 open_exchange-0.1.9/examples/property_values.py
--rw-r--r--   0        0        0     1224 2024-04-09 17:08:56.596033 open_exchange-0.1.9/examples/rent_estimates.py
--rw-r--r--   0        0        0     3197 2024-04-09 17:08:56.596141 open_exchange-0.1.9/examples/rental_comps.py
--rw-r--r--   0        0        0    39562 2024-03-29 16:19:05.495113 open_exchange-0.1.9/poetry.lock
--rw-r--r--   0        0        0       46 2024-02-29 17:29:44.102413 open_exchange-0.1.9/poetry.toml
--rw-r--r--   0        0        0     5335 2024-03-29 16:19:05.495458 open_exchange-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      896 2024-03-19 15:25:49.701762 open_exchange-0.1.9/setup.cfg
--rw-r--r--   0        0        0      171 2024-03-29 16:19:05.495841 open_exchange-0.1.9/src/open_exchange/__init__.py
--rw-r--r--   0        0        0     2442 2024-03-19 19:20:13.428869 open_exchange-0.1.9/src/open_exchange/client.py
--rw-r--r--   0        0        0      220 2024-03-19 15:25:49.702425 open_exchange-0.1.9/src/open_exchange/compat.py
--rw-r--r--   0        0        0      512 2024-03-19 19:12:44.330100 open_exchange-0.1.9/src/open_exchange/contants.py
--rw-r--r--   0        0        0       45 2024-03-18 21:34:52.403620 open_exchange-0.1.9/src/open_exchange/exceptions.py
--rw-r--r--   0        0        0      338 2024-03-19 15:25:49.702656 open_exchange-0.1.9/src/open_exchange/resource.py
--rw-r--r--   0        0        0      100 2024-03-19 15:25:49.702895 open_exchange-0.1.9/src/open_exchange/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 21:34:24.213650 open_exchange-0.1.9/src/open_exchange/resources/data/__init__.py
--rw-r--r--   0        0        0      901 2024-03-19 19:05:46.043254 open_exchange-0.1.9/src/open_exchange/resources/data/data.py
--rw-r--r--   0        0        0     2554 2024-03-29 16:19:05.496032 open_exchange-0.1.9/src/open_exchange/resources/data/property_details.py
--rw-r--r--   0        0        0     2503 2024-03-29 16:19:05.496228 open_exchange-0.1.9/src/open_exchange/resources/data/property_values.py
--rw-r--r--   0        0        0     2532 2024-03-29 16:19:05.496424 open_exchange-0.1.9/src/open_exchange/resources/data/rent_estimates.py
--rw-r--r--   0        0        0     6176 2024-03-29 16:19:05.496787 open_exchange-0.1.9/src/open_exchange/resources/data/rental_comps.py
--rw-r--r--   0        0        0        0 2024-03-19 15:25:49.703258 open_exchange-0.1.9/src/open_exchange/types/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 15:57:29.715648 open_exchange-0.1.9/src/open_exchange/types/data/__init__.py
--rw-r--r--   0        0        0     1306 2024-03-19 18:42:19.080554 open_exchange-0.1.9/src/open_exchange/types/data/property_details_fetch_params.py
--rw-r--r--   0        0        0     3813 2024-03-19 18:43:06.622696 open_exchange-0.1.9/src/open_exchange/types/data/property_details_response.py
--rw-r--r--   0        0        0     1304 2024-03-19 18:42:19.083863 open_exchange-0.1.9/src/open_exchange/types/data/property_values_fetch_params.py
--rw-r--r--   0        0        0      977 2024-03-19 15:25:49.704299 open_exchange-0.1.9/src/open_exchange/types/data/property_values_response.py
--rw-r--r--   0        0        0     1302 2024-03-19 18:42:19.082274 open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_fetch_params.py
--rw-r--r--   0        0        0      816 2024-03-19 15:25:49.704568 open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_response.py
--rw-r--r--   0        0        0    11318 2024-03-19 22:06:51.801434 open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_fetch_params.py
--rw-r--r--   0        0        0    10142 2024-03-19 16:00:43.707916 open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_response.py
--rw-r--r--   0        0        0       88 2024-03-19 15:25:49.705192 open_exchange-0.1.9/src/open_exchange/types/models.py
--rw-r--r--   0        0        0      272 2024-03-19 15:25:49.705577 open_exchange-0.1.9/src/open_exchange/typing.py
--rw-r--r--   0        0        0       75 2024-03-18 21:34:52.400922 open_exchange-0.1.9/tests/open_exchange/test_rental_comps.py
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 open_exchange-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       29 2024-03-05 16:34:03.069794 open_exchange-0.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      172 2024-03-05 16:34:10.434965 open_exchange-0.2.0/.gitignore
+-rw-r--r--   0        0        0      845 2024-04-17 18:57:31.359096 open_exchange-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       99 2024-02-29 17:29:44.100867 open_exchange-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1091 2024-02-29 17:29:44.101716 open_exchange-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1698 2024-03-20 15:26:18.626982 open_exchange-0.2.0/README.md
+-rw-r--r--   0        0        0      892 2024-04-09 17:08:56.595669 open_exchange-0.2.0/cortex.yaml
+-rw-r--r--   0        0        0     1405 2024-04-09 17:08:56.595799 open_exchange-0.2.0/examples/property_details.py
+-rw-r--r--   0        0        0     1209 2024-04-09 17:08:56.595920 open_exchange-0.2.0/examples/property_values.py
+-rw-r--r--   0        0        0     1224 2024-04-09 17:08:56.596033 open_exchange-0.2.0/examples/rent_estimates.py
+-rw-r--r--   0        0        0     3507 2024-04-17 18:54:03.015959 open_exchange-0.2.0/examples/rental_comps.py
+-rw-r--r--   0        0        0    39562 2024-03-29 16:19:05.495113 open_exchange-0.2.0/poetry.lock
+-rw-r--r--   0        0        0       46 2024-02-29 17:29:44.102413 open_exchange-0.2.0/poetry.toml
+-rw-r--r--   0        0        0     5335 2024-03-29 16:19:05.495458 open_exchange-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      896 2024-03-19 15:25:49.701762 open_exchange-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      171 2024-04-17 18:54:03.016863 open_exchange-0.2.0/src/open_exchange/__init__.py
+-rw-r--r--   0        0        0     2753 2024-04-19 16:44:44.973511 open_exchange-0.2.0/src/open_exchange/client.py
+-rw-r--r--   0        0        0      220 2024-03-19 15:25:49.702425 open_exchange-0.2.0/src/open_exchange/compat.py
+-rw-r--r--   0        0        0      512 2024-03-19 19:12:44.330100 open_exchange-0.2.0/src/open_exchange/contants.py
+-rw-r--r--   0        0        0      870 2024-04-17 18:53:49.278942 open_exchange-0.2.0/src/open_exchange/exceptions.py
+-rw-r--r--   0        0        0      338 2024-03-19 15:25:49.702656 open_exchange-0.2.0/src/open_exchange/resource.py
+-rw-r--r--   0        0        0      100 2024-03-19 15:25:49.702895 open_exchange-0.2.0/src/open_exchange/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 21:34:24.213650 open_exchange-0.2.0/src/open_exchange/resources/data/__init__.py
+-rw-r--r--   0        0        0      901 2024-03-19 19:05:46.043254 open_exchange-0.2.0/src/open_exchange/resources/data/data.py
+-rw-r--r--   0        0        0     2554 2024-03-29 16:19:05.496032 open_exchange-0.2.0/src/open_exchange/resources/data/property_details.py
+-rw-r--r--   0        0        0     2503 2024-03-29 16:19:05.496228 open_exchange-0.2.0/src/open_exchange/resources/data/property_values.py
+-rw-r--r--   0        0        0     2532 2024-03-29 16:19:05.496424 open_exchange-0.2.0/src/open_exchange/resources/data/rent_estimates.py
+-rw-r--r--   0        0        0     6176 2024-03-29 16:19:05.496787 open_exchange-0.2.0/src/open_exchange/resources/data/rental_comps.py
+-rw-r--r--   0        0        0        0 2024-03-19 15:25:49.703258 open_exchange-0.2.0/src/open_exchange/types/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 15:57:29.715648 open_exchange-0.2.0/src/open_exchange/types/data/__init__.py
+-rw-r--r--   0        0        0     1306 2024-03-19 18:42:19.080554 open_exchange-0.2.0/src/open_exchange/types/data/property_details_fetch_params.py
+-rw-r--r--   0        0        0     3813 2024-03-19 18:43:06.622696 open_exchange-0.2.0/src/open_exchange/types/data/property_details_response.py
+-rw-r--r--   0        0        0     1304 2024-03-19 18:42:19.083863 open_exchange-0.2.0/src/open_exchange/types/data/property_values_fetch_params.py
+-rw-r--r--   0        0        0      977 2024-03-19 15:25:49.704299 open_exchange-0.2.0/src/open_exchange/types/data/property_values_response.py
+-rw-r--r--   0        0        0     1302 2024-03-19 18:42:19.082274 open_exchange-0.2.0/src/open_exchange/types/data/rent_estimates_fetch_params.py
+-rw-r--r--   0        0        0      816 2024-03-19 15:25:49.704568 open_exchange-0.2.0/src/open_exchange/types/data/rent_estimates_response.py
+-rw-r--r--   0        0        0    11318 2024-03-19 22:06:51.801434 open_exchange-0.2.0/src/open_exchange/types/data/rental_comps_fetch_params.py
+-rw-r--r--   0        0        0    10581 2024-04-17 18:54:03.017676 open_exchange-0.2.0/src/open_exchange/types/data/rental_comps_response.py
+-rw-r--r--   0        0        0       88 2024-03-19 15:25:49.705192 open_exchange-0.2.0/src/open_exchange/types/models.py
+-rw-r--r--   0        0        0      272 2024-03-19 15:25:49.705577 open_exchange-0.2.0/src/open_exchange/typing.py
+-rw-r--r--   0        0        0       75 2024-03-18 21:34:52.400922 open_exchange-0.2.0/tests/open_exchange/test_rental_comps.py
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 open_exchange-0.2.0/PKG-INFO
```

### Comparing `open_exchange-0.1.9/CHANGELOG.md` & `open_exchange-0.2.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v0.2.0 (2024-04-17)
+
+* Added listing_description, concession_description, concession_start_date, and concession_end_date to ResultRentalComp.
+  ([#12](https://github.com/opendoor-labs/open-exchange-python/pull/12))
+* Improve HTTP errors within SDK. ([#13](https://github.com/opendoor-labs/open-exchange-python/pull/14))
+
 ## v0.1.9 (2024-03-29)
 
 * Improved support for interactively killing (KeyboardInterrupt) and rerunning endpoints, optimizing for reduced memory
   consumption and immediate results processing. ([#9](https://github.com/opendoor-labs/open-exchange-python/pull/9))
 * Improved examples based on client feedback. ([#10](https://github.com/opendoor-labs/open-exchange-python/pull/10))
 
 ## v0.1.8 (2024-03-19)
```

### Comparing `open_exchange-0.1.9/LICENSE.md` & `open_exchange-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/README.md` & `open_exchange-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/cortex.yaml` & `open_exchange-0.2.0/cortex.yaml`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/examples/property_details.py` & `open_exchange-0.2.0/examples/property_details.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/examples/property_values.py` & `open_exchange-0.2.0/examples/property_values.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/examples/rent_estimates.py` & `open_exchange-0.2.0/examples/rent_estimates.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/examples/rental_comps.py` & `open_exchange-0.2.0/examples/rental_comps.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,10 +69,14 @@
             print("initial list price date:", rental_comp.initial_list_price_date)
             print("last event date:", rental_comp.last_event_date)
             print("last list price:", rental_comp.last_list_price)
             print("listing status:", rental_comp.listing_status)
             print("move out date:", rental_comp.move_out_date)
             print("ownership profile:", rental_comp.ownership_profile)
             print("response codes:", rental_comp.response_codes)
-            print("similarity score:", rental_comp.similarity_score, end="\n\n")
+            print("similarity score:", rental_comp.similarity_score)
+            print("listing description:", rental_comp.listing_description)
+            print("concession description:", rental_comp.concession_description)
+            print("concession start date:", rental_comp.concession_start_date)
+            print("concession end date:", rental_comp.concession_end_date, end="\n\n")
     else:
         print("No rental comps available for this address.")
```

### Comparing `open_exchange-0.1.9/poetry.lock` & `open_exchange-0.2.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/pyproject.toml` & `open_exchange-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/setup.cfg` & `open_exchange-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/client.py` & `open_exchange-0.2.0/src/open_exchange/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import urllib3.util.retry
 
 # 1st Party Libraries
 import open_exchange
 from open_exchange import resources
 from open_exchange.compat import cached_property
 from open_exchange.contants import DEFAULT_MAX_RETRIES, DEFAULT_RETRY_BACKOFF_FACTOR, DEFAULT_RETRYABLE_STATUS_CODES
-from open_exchange.exceptions import OpenExchangeError
+from open_exchange.exceptions import APIError, OpenExchangeError
 
 logger = logging.getLogger(__name__)
 
 PYTHON_VERSION = platform.python_version()
 SDK_VERSION = open_exchange.__version__
 
 
@@ -56,19 +56,30 @@
             headers={
                 "AUTHORIZATION": self.api_key,
                 "X-PYTHON-VERSION": PYTHON_VERSION,
                 "X-SDK-VERSION": SDK_VERSION,
             },
             json=body,
         )
-        response.raise_for_status()  # Raise custom exception for HTTP errors here?
+        try:
+            response.raise_for_status()
+        except requests.HTTPError as e:
+            raise _make_api_error_from_http_error(e) from None
         return response.json()
 
     @cached_property
     def _retry_config(self) -> urllib3.util.retry.Retry:
         return urllib3.util.retry.Retry(
             total=DEFAULT_MAX_RETRIES,
             backoff_factor=DEFAULT_RETRY_BACKOFF_FACTOR,
             status_forcelist=DEFAULT_RETRYABLE_STATUS_CODES,
             # POST is not in the default set of allowed methods. Override the default to include it.
             allowed_methods=urllib3.util.retry.Retry.DEFAULT_ALLOWED_METHODS | {"POST"},
         )
+
+
+def _make_api_error_from_http_error(http_error: requests.HTTPError) -> APIError:
+    return APIError(
+        message=http_error.response.text,
+        request=http_error.request,
+        body=http_error.response.json(),
+    )
```

### Comparing `open_exchange-0.1.9/src/open_exchange/contants.py` & `open_exchange-0.2.0/src/open_exchange/contants.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/resources/data/data.py` & `open_exchange-0.2.0/src/open_exchange/resources/data/data.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/resources/data/property_details.py` & `open_exchange-0.2.0/src/open_exchange/resources/data/property_details.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/resources/data/property_values.py` & `open_exchange-0.2.0/src/open_exchange/resources/data/property_values.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/resources/data/rent_estimates.py` & `open_exchange-0.2.0/src/open_exchange/resources/data/rent_estimates.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/resources/data/rental_comps.py` & `open_exchange-0.2.0/src/open_exchange/resources/data/rental_comps.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/property_details_fetch_params.py` & `open_exchange-0.2.0/src/open_exchange/types/data/property_details_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/property_details_response.py` & `open_exchange-0.2.0/src/open_exchange/types/data/property_details_response.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/property_values_fetch_params.py` & `open_exchange-0.2.0/src/open_exchange/types/data/property_values_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/property_values_response.py` & `open_exchange-0.2.0/src/open_exchange/types/data/property_values_response.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_fetch_params.py` & `open_exchange-0.2.0/src/open_exchange/types/data/rent_estimates_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/rent_estimates_response.py` & `open_exchange-0.2.0/src/open_exchange/types/data/rent_estimates_response.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_fetch_params.py` & `open_exchange-0.2.0/src/open_exchange/types/data/rental_comps_fetch_params.py`

 * *Files identical despite different names*

### Comparing `open_exchange-0.1.9/src/open_exchange/types/data/rental_comps_response.py` & `open_exchange-0.2.0/src/open_exchange/types/data/rental_comps_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,14 +184,26 @@
     similarity_score: Optional[float] = None
     """
     A score between 0 and 1 describing how similar this comp is to the subject
     property. Similarity accounts for both home details (bed, bath, year built,
     etc.) as well as location. A larger score indicates a more similar comp.
     """
 
+    listing_description: Optional[str] = None
+    """Complete listing description as mentioned on the listing source website."""
+
+    concession_description: Optional[str] = None
+    """Description of any concessions available for the property."""
+
+    concession_start_date: Optional[date] = None
+    """Start date of the concession period."""
+
+    concession_end_date: Optional[date] = None
+    """End date of the concession period."""
+
 
 class ResultSubjectPropertyDetails(BaseModel):
     city: str
     """The city name where the property resides."""
 
     postal_code: str
     """The 5 digit zip or postal code of the location where the property resides."""
```

### Comparing `open_exchange-0.1.9/PKG-INFO` & `open_exchange-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-exchange
-Version: 0.1.9
+Version: 0.2.0
 Summary: Open Exchange Python SDK.
 Author-email: "Open Exchange Labs, Inc." <ox-data-eng@opendoor.com>
 Requires-Python: >=3.6.2,<4.0.0
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

