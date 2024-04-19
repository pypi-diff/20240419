# Comparing `tmp/airbyte_source_paypal_transaction-2.5.1.tar.gz` & `tmp/airbyte_source_paypal_transaction-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_paypal_transaction-2.5.1.tar", max compression
+gzip compressed data, was "airbyte_source_paypal_transaction-2.5.2.tar", max compression
```

## Comparing `airbyte_source_paypal_transaction-2.5.1.tar` & `airbyte_source_paypal_transaction-2.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11631 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/README.md
--rw-r--r--   0        0        0      832 2024-03-15 18:49:24.498053 airbyte_source_paypal_transaction-2.5.1/pyproject.toml
--rw-r--r--   0        0        0      146 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/__init__.py
--rw-r--r--   0        0        0     3072 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/components.py
--rw-r--r--   0        0        0    13334 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/manifest.yaml
--rw-r--r--   0        0        0      264 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/run.py
--rw-r--r--   0        0        0     1535 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/balances.json
--rw-r--r--   0        0        0     1772 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/list_disputes.json
--rw-r--r--   0        0        0     7895 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/list_payments.json
--rw-r--r--   0        0        0      689 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/list_products.json
--rw-r--r--   0        0        0    13751 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/search_invoices.json
--rw-r--r--   0        0        0      946 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/show_product_details.json
--rw-r--r--   0        0        0    11212 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/transactions.json
--rw-r--r--   0        0        0      523 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/source.py
--rw-r--r--   0        0        0     3021 2024-03-15 18:16:55.000000 airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/spec.yaml
--rw-r--r--   0        0        0    12369 1970-01-01 00:00:00.000000 airbyte_source_paypal_transaction-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11632 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/README.md
+-rw-r--r--   0        0        0      832 2024-04-19 13:30:50.120081 airbyte_source_paypal_transaction-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/__init__.py
+-rw-r--r--   0        0        0     3072 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/components.py
+-rw-r--r--   0        0        0    13334 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/manifest.yaml
+-rw-r--r--   0        0        0      264 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/run.py
+-rw-r--r--   0        0        0     1535 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/balances.json
+-rw-r--r--   0        0        0     1772 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_disputes.json
+-rw-r--r--   0        0        0     7895 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_payments.json
+-rw-r--r--   0        0        0      689 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_products.json
+-rw-r--r--   0        0        0    13751 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/search_invoices.json
+-rw-r--r--   0        0        0      946 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/show_product_details.json
+-rw-r--r--   0        0        0    11212 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/transactions.json
+-rw-r--r--   0        0        0      523 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/source.py
+-rw-r--r--   0        0        0     3021 2024-04-19 13:08:30.000000 airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/spec.yaml
+-rw-r--r--   0        0        0    12370 1970-01-01 00:00:00.000000 airbyte_source_paypal_transaction-2.5.2/PKG-INFO
```

### Comparing `airbyte_source_paypal_transaction-2.5.1/README.md` & `airbyte_source_paypal_transaction-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 ### Locally running the connector
 
 ```
 poetry run source-paypal-transaction spec
 poetry run source-paypal-transaction check --config secrets/config.json
 poetry run source-paypal-transaction discover --config secrets/config.json
-#Example with list_payments catalog and the debug flag
+# Example with list_payments catalog and the debug flag
 poetry run source-paypal-transaction read --config secrets/config.json --catalog integration_tests/configured_catalog_list_payments.json --debug
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 
 ```
```

### Comparing `airbyte_source_paypal_transaction-2.5.1/pyproject.toml` & `airbyte_source_paypal_transaction-2.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.1"
+version = "2.5.2"
 name = "airbyte-source-paypal-transaction"
 description = "Source implementation for Paypal Transaction."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/components.py` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/manifest.yaml` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/manifest.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: 0.50.2
+version: 0.82.0
 type: DeclarativeSource
 
 definitions:
   selector:
     type: RecordSelector
     extractor:
       type: DpathExtractor
```

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/balances.json` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/balances.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/list_disputes.json` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/list_payments.json` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_payments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/list_products.json` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/list_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/search_invoices.json` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/search_invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/show_product_details.json` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/show_product_details.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/schemas/transactions.json` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/source.py` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/source_paypal_transaction/spec.yaml` & `airbyte_source_paypal_transaction-2.5.2/source_paypal_transaction/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_paypal_transaction-2.5.1/PKG-INFO` & `airbyte_source_paypal_transaction-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-paypal-transaction
-Version: 2.5.1
+Version: 2.5.2
 Summary: Source implementation for Paypal Transaction.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -54,15 +54,15 @@
 
 ### Locally running the connector
 
 ```
 poetry run source-paypal-transaction spec
 poetry run source-paypal-transaction check --config secrets/config.json
 poetry run source-paypal-transaction discover --config secrets/config.json
-#Example with list_payments catalog and the debug flag
+# Example with list_payments catalog and the debug flag
 poetry run source-paypal-transaction read --config secrets/config.json --catalog integration_tests/configured_catalog_list_payments.json --debug
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 
 ```
```

