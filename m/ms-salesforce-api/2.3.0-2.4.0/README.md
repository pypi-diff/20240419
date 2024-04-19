# Comparing `tmp/ms_salesforce_api-2.3.0.tar.gz` & `tmp/ms_salesforce_api-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-2.3.0.tar", max compression
+gzip compressed data, was "ms_salesforce_api-2.4.0.tar", max compression
```

## Comparing `ms_salesforce_api-2.3.0.tar` & `ms_salesforce_api-2.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/LICENSE
--rw-r--r--   0        0        0     8326 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py
--rw-r--r--   0        0        0     4925 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/constants.py
--rw-r--r--   0        0        0    14992 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
--rw-r--r--   0        0        0     5240 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
--rw-r--r--   0        0        0     6011 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    10789 2024-04-11 08:06:36.595700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/helpers.py
--rw-r--r--   0        0        0     3788 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
--rw-r--r--   0        0        0    24290 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
--rw-r--r--   0        0        0    10430 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/constants.py
--rw-r--r--   0        0        0     3967 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    28488 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2485 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/dto/__init__.py
--rw-r--r--   0        0        0     8873 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
--rw-r--r--   0        0        0    12640 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    13717 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0        0 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/helpers/__init__.py
--rw-r--r--   0        0        0      303 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/helpers/string.py
--rw-r--r--   0        0        0     1055 2024-04-11 08:06:36.599700 ms_salesforce_api-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/LICENSE
+-rw-r--r--   0        0        0     8326 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/__init__.py
+-rw-r--r--   0        0        0     1620 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py
+-rw-r--r--   0        0        0     4925 2024-04-19 10:36:31.728721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/constants.py
+-rw-r--r--   0        0        0    14992 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
+-rw-r--r--   0        0        0     5240 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
+-rw-r--r--   0        0        0     6011 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    10789 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/helpers.py
+-rw-r--r--   0        0        0     3788 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    25119 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0    10921 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/constants.py
+-rw-r--r--   0        0        0     3967 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    35740 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2485 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/dto/__init__.py
+-rw-r--r--   0        0        0     9817 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12640 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    13717 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/helpers/__init__.py
+-rw-r--r--   0        0        0      303 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/helpers/string.py
+-rw-r--r--   0        0        0     1055 2024-04-19 10:36:31.732721 ms_salesforce_api-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.4.0/PKG-INFO
```

### Comparing `ms_salesforce_api-2.3.0/LICENSE` & `ms_salesforce_api-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/README.md` & `ms_salesforce_api-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/constants.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/__init__.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,14 +378,15 @@
             private_key,
             audience="https://login.salesforce.com",
         )
         opportunities = project.get_all()
         self.assertEqual(len(opportunities), 1)
 
         opportunity = opportunities[0]
+
         self.assertIsInstance(opportunity, dict)
         self.assertDictEqual(
             opportunity,
             {
                 "account_assigment_group": "03",
                 "account_billing_address": "211 Main Street, Webster, Maine, 01570, United "
                 "States",
@@ -413,14 +414,15 @@
                 "account_sap_id": "10000319",
                 "account_tax_category": None,
                 "account_tax_classification": "0",
                 "account_tax_id_type": "US01",
                 "account_tier": "T1",
                 "account_website": None,
                 "amount": 0.0,
+                "autorenewal": False,
                 "billing_lines": [
                     {
                         "billing_amount": 6708.0,
                         "billing_date": "2022-08-31",
                         "billing_period_ending_date": "2022-08-31",
                         "billing_period_starting_date": "2022-08-01",
                         "billing_plan_amount": "6708",
@@ -435,38 +437,52 @@
                         "last_modified_date": "2022-10-16T18:56:34.000+0000",
                         "name": "BL-000175313",
                         "project_code": "USMSEX05508",
                         "project_id": "a00AX000002DVi1YAG",
                         "revenue_dedication": 103.2,
                     }
                 ],
+                "comments": "",
                 "controller_email": "employee4@test.com",
                 "controller_sub_email": "employee3@test.com",
                 "cost_center": "",
                 "created_at": "2022-08-01T08:53:12.000+0000",
                 "currency": "EUR",
+                "end_date": "",
                 "group_bqid": "1",
                 "group_end_date": "2100-12-12",
                 "group_groupid": "a0cAX000000TSWUYA4",
                 "group_name": "MAPFRE",
                 "group_owner_email": "employee1@test.com",
                 "group_pck_type": "Key Account",
                 "group_start_date": "2023-06-01",
                 "group_supervisor_email": "employee2@test.com",
+                "internal_comment": "",
+                "international_deparments": False,
                 "invoicing_country_code": "US",
                 "jira_task_url": "<a "
                 "href=https://makingscience.atlassian.net/browse/ESMSBD0001-7168 "
                 "target=_blank>View Jira Task</a>",
                 "last_updated_at": "2023-09-01T10:00:54.000+0000",
                 "lead_source": "Crosselling/upselling",
+                "maintance_project": False,
+                "ms_project_id": False,
+                "operation_coordinator_controller": "",
                 "operation_coordinator_email": "employee5@test.com",
+                "operation_coordinator_name": "",
+                "operation_coordinator_sub": "",
                 "operation_coordinator_sub_email": "employee5@test.com",
+                "opportunity": "",
+                "opportunity_extension": "",
                 "opportunity_name": "New Site Mapfre AAA",
                 "opportunity_percentage": 100.0,
+                "periodicity": "",
                 "profit_center": "200018",
+                "profitcenter": "",
+                "project_account": "",
                 "project_code": "USMSEX05508",
                 "project_id": "a00AX000002DVi1YAG",
                 "project_line_items": [
                     {
                         "country": None,
                         "created_date": "2022-08-02T15:44:34.000+0000",
                         "effort": "516",
@@ -498,15 +514,21 @@
                         "total_price": 21515.0,
                         "unit_price": 65.0,
                     },
                 ],
                 "project_name": "MapfreAAA",
                 "project_start_date": "2022-08-01",
                 "project_tier": "Unkown",
+                "projectcode": "",
+                "projectid": "",
+                "quote": "",
+                "rejection_reason": "",
+                "revenue_details": "",
                 "stage": "Closed Won",
+                "status": "",
                 "subgroup_bqid": "5",
                 "subgroup_end_date": "2100-12-12",
                 "subgroup_groupid": "a0cAX000000TSWUYA4",
                 "subgroup_name": "MAPFRE USA",
                 "subgroup_owner_email": "employee1@test.com",
                 "subgroup_start_date": "2023-06-01",
                 "subgroup_subgroupid": "a19AX0000004simYAA",
```

#### html2text {}

```diff
@@ -167,62 +167,72 @@
 "account_currency_code": "EUR", "account_customer_groupId": "1",
 "account_customer_subgroupId": "5", "account_fax": None,
 "account_invoicing_email": "client1@test.com", "account_mail_invoicing":
 "client1@test.com", "account_name": "MAPFRE USA", "account_office": "Making
 Science LLC", "account_payment_terms": "T060", "account_pec_email": None,
 "account_phone": None, "account_sap_id": "10000319", "account_tax_category":
 None, "account_tax_classification": "0", "account_tax_id_type": "US01",
-"account_tier": "T1", "account_website": None, "amount": 0.0, "billing_lines":
-[ { "billing_amount": 6708.0, "billing_date": "2022-08-31",
-"billing_period_ending_date": "2022-08-31", "billing_period_starting_date":
-"2022-08-01", "billing_plan_amount": "6708", "billing_plan_billing_date":
-"2022-08-31", "billing_plan_item": "1", "billing_plan_service_end_date": "2022-
-08-31", "billing_plan_service_start_date": "2022-08-01", "created_date": "2022-
-08-09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
+"account_tier": "T1", "account_website": None, "amount": 0.0, "autorenewal":
+False, "billing_lines": [ { "billing_amount": 6708.0, "billing_date": "2022-08-
+31", "billing_period_ending_date": "2022-08-31",
+"billing_period_starting_date": "2022-08-01", "billing_plan_amount": "6708",
+"billing_plan_billing_date": "2022-08-31", "billing_plan_item": "1",
+"billing_plan_service_end_date": "2022-08-31",
+"billing_plan_service_start_date": "2022-08-01", "created_date": "2022-08-
+09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
 "a0sAX000000I8lgYAC", "last_modified_date": "2022-10-16T18:56:34.000+0000",
 "name": "BL-000175313", "project_code": "USMSEX05508", "project_id":
-"a00AX000002DVi1YAG", "revenue_dedication": 103.2, } ], "controller_email":
-"employee4@test.com", "controller_sub_email": "employee3@test.com",
-"cost_center": "", "created_at": "2022-08-01T08:53:12.000+0000", "currency":
-"EUR", "group_bqid": "1", "group_end_date": "2100-12-12", "group_groupid":
-"a0cAX000000TSWUYA4", "group_name": "MAPFRE", "group_owner_email":
-"employee1@test.com", "group_pck_type": "Key Account", "group_start_date":
-"2023-06-01", "group_supervisor_email": "employee2@test.com",
-"invoicing_country_code": "US", "jira_task_url": "
+"a00AX000002DVi1YAG", "revenue_dedication": 103.2, } ], "comments": "",
+"controller_email": "employee4@test.com", "controller_sub_email":
+"employee3@test.com", "cost_center": "", "created_at": "2022-08-01T08:53:
+12.000+0000", "currency": "EUR", "end_date": "", "group_bqid": "1",
+"group_end_date": "2100-12-12", "group_groupid": "a0cAX000000TSWUYA4",
+"group_name": "MAPFRE", "group_owner_email": "employee1@test.com",
+"group_pck_type": "Key Account", "group_start_date": "2023-06-01",
+"group_supervisor_email": "employee2@test.com", "internal_comment": "",
+"international_deparments": False, "invoicing_country_code": "US",
+"jira_task_url": "
  "href=https://makingscience.atlassian.net/browse/ESMSBD0001-7168 "
 "target=_blank>View Jira Task
 ", "last_updated_at": "2023-09-01T10:00:54.000+0000", "lead_source":
-"Crosselling/upselling", "operation_coordinator_email": "employee5@test.com",
-"operation_coordinator_sub_email": "employee5@test.com", "opportunity_name":
-"New Site Mapfre AAA", "opportunity_percentage": 100.0, "profit_center":
-"200018", "project_code": "USMSEX05508", "project_id": "a00AX000002DVi1YAG",
-"project_line_items": [ { "country": None, "created_date": "2022-08-02T15:44:
-34.000+0000", "effort": "516", "ending_date": "2022-12-31", "id":
-"a0VAX000000EE0b2AG", "last_modified_date": "2023-06-20T22:33:36.000+0000",
-"ms_pli_name": "USA_UX/UI Design_USMSEX05508", "ms_project_code": None,
-"product_name": "UXUI Project", "project_id": "a00AX000002DVi1YAG", "quantity":
-516.0, "starting_date": "2022-08-01", "total_price": 33540.0, "unit_price":
-65.0, }, { "country": None, "created_date": "2022-08-09T14:54:59.000+0000",
-"effort": "331", "ending_date": "2022-12-31", "id": "a0VAX000000ELU52AO",
-"last_modified_date": "2023-06-20T22:33:36.000+0000", "ms_pli_name": "ES_UX/UI
-Design_USMSEX05508", "ms_project_code": None, "product_name": "UXUI Project",
-"project_id": "a00AX000002DVi1YAG", "quantity": 331.0, "starting_date": "2022-
-08-01", "total_price": 21515.0, "unit_price": 65.0, }, ], "project_name":
-"MapfreAAA", "project_start_date": "2022-08-01", "project_tier": "Unkown",
-"stage": "Closed Won", "subgroup_bqid": "5", "subgroup_end_date": "2100-12-12",
-"subgroup_groupid": "a0cAX000000TSWUYA4", "subgroup_name": "MAPFRE USA",
-"subgroup_owner_email": "employee1@test.com", "subgroup_start_date": "2023-06-
-01", "subgroup_subgroupid": "a19AX0000004simYAA", }, ) billing_line =
-opportunity["billing_lines"][0] self.assertDictEqual( billing_line,
-{ "billing_amount": 6708.0, "billing_date": "2022-08-31",
-"billing_period_ending_date": "2022-08-31", "billing_period_starting_date":
-"2022-08-01", "billing_plan_amount": "6708", "billing_plan_billing_date":
-"2022-08-31", "billing_plan_item": "1", "billing_plan_service_end_date": "2022-
-08-31", "billing_plan_service_start_date": "2022-08-01", "created_date": "2022-
-08-09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
+"Crosselling/upselling", "maintance_project": False, "ms_project_id": False,
+"operation_coordinator_controller": "", "operation_coordinator_email":
+"employee5@test.com", "operation_coordinator_name": "",
+"operation_coordinator_sub": "", "operation_coordinator_sub_email":
+"employee5@test.com", "opportunity": "", "opportunity_extension": "",
+"opportunity_name": "New Site Mapfre AAA", "opportunity_percentage": 100.0,
+"periodicity": "", "profit_center": "200018", "profitcenter": "",
+"project_account": "", "project_code": "USMSEX05508", "project_id":
+"a00AX000002DVi1YAG", "project_line_items": [ { "country": None,
+"created_date": "2022-08-02T15:44:34.000+0000", "effort": "516", "ending_date":
+"2022-12-31", "id": "a0VAX000000EE0b2AG", "last_modified_date": "2023-06-20T22:
+33:36.000+0000", "ms_pli_name": "USA_UX/UI Design_USMSEX05508",
+"ms_project_code": None, "product_name": "UXUI Project", "project_id":
+"a00AX000002DVi1YAG", "quantity": 516.0, "starting_date": "2022-08-01",
+"total_price": 33540.0, "unit_price": 65.0, }, { "country": None,
+"created_date": "2022-08-09T14:54:59.000+0000", "effort": "331", "ending_date":
+"2022-12-31", "id": "a0VAX000000ELU52AO", "last_modified_date": "2023-06-20T22:
+33:36.000+0000", "ms_pli_name": "ES_UX/UI Design_USMSEX05508",
+"ms_project_code": None, "product_name": "UXUI Project", "project_id":
+"a00AX000002DVi1YAG", "quantity": 331.0, "starting_date": "2022-08-01",
+"total_price": 21515.0, "unit_price": 65.0, }, ], "project_name": "MapfreAAA",
+"project_start_date": "2022-08-01", "project_tier": "Unkown", "projectcode":
+"", "projectid": "", "quote": "", "rejection_reason": "", "revenue_details":
+"", "stage": "Closed Won", "status": "", "subgroup_bqid": "5",
+"subgroup_end_date": "2100-12-12", "subgroup_groupid": "a0cAX000000TSWUYA4",
+"subgroup_name": "MAPFRE USA", "subgroup_owner_email": "employee1@test.com",
+"subgroup_start_date": "2023-06-01", "subgroup_subgroupid":
+"a19AX0000004simYAA", }, ) billing_line = opportunity["billing_lines"][0]
+self.assertDictEqual( billing_line, { "billing_amount": 6708.0, "billing_date":
+"2022-08-31", "billing_period_ending_date": "2022-08-31",
+"billing_period_starting_date": "2022-08-01", "billing_plan_amount": "6708",
+"billing_plan_billing_date": "2022-08-31", "billing_plan_item": "1",
+"billing_plan_service_end_date": "2022-08-31",
+"billing_plan_service_start_date": "2022-08-01", "created_date": "2022-08-
+09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
 "a0sAX000000I8lgYAC", "last_modified_date": "2022-10-16T18:56:34.000+0000",
 "name": "BL-000175313", "project_code": "USMSEX05508", "project_id":
 "a00AX000002DVi1YAG", "revenue_dedication": 103.2, }, )
 mock_make_request.assert_called() @patch
 (
 "ms_salesforce_api.salesforce.api.project.SalesforceQueryExecutor.authenticate"
 # noqa: E501 ) @patch
```

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/constants.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,35 @@
     Operation_Coordinator__r.Controller__c,
     Operation_Coordinator_Sub__r.Controller_SUB__c,
     LKP_ProfitCenter__r.TXT_ProfitCenter__c,
     LKP_CostCenter__r.Name,
     Opportunity__r.Probability,
     Opportunity__r.Tier_Short__c,
     Opportunity__r.JiraComponentURL__c,
+    Autorenewal__c,
+    Comments__c,
+    End_Date__c,
+    International_Departments__c,
+    LKP_OpportunityExtension__c,
+    Maintenance_project__c,
+    MS_Project_Id__c,
+    Operation_Coordinator__c,
+    Operation_Coordinator_Sub__c,
+    Opportunity__c,
+    Periodicity__c,
+    LKP_ProfitCenter__c,
+    Project_Account__c,
+    Project_Code__c,
+    Project_id__c,
+    Quote__c,
+    Revenue_Details__c,
+    Status__c,
+    TXT_InternalComment__c,
+    TXT_RejectionReason__c,
+    ProjectID__c,
     Project_Account__r.Id,
     Project_Account__r.Name,
     Project_Account__r.MS_Customer_Account_Assigment_Group__c,
     Project_Account__r.MS_Customer_Tax_Category__c,
     Project_Account__r.MS_Customer_Tax_Classification__c,
     Project_Account__r.TXT_SAPId__c,
     Project_Account__r.ms_Business_Function__c,
```

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py`

 * *Files 26% similar despite different names*

```diff
@@ -68,14 +68,35 @@
         group_owner_email,
         subgroup_owner_email,
         subgroup_name,
         subgroup_start_date,
         subgroup_end_date,
         subgroup_bqid,
         subgroup_id,
+        autorenewal,
+        comments,
+        end_date,
+        international_deparments,
+        opportunity_extension,
+        maintance_project,
+        ms_project_id,
+        operation_coordinator_name,
+        operation_coordinator_controller,
+        operation_coordinator_sub,
+        opportunity,
+        periodicity,
+        profitcenter,
+        project_account,
+        projectcode,
+        revenue_details,
+        status,
+        internal_comment,
+        rejection_reason,
+        projectid,
+        quote,
         billing_lines=[],
         project_line_items=[],
     ):
         self.account_business_name = account_business_name
         self.account_name = account_name
         self.account_id = account_id
         self.currency = currency
@@ -138,17 +159,51 @@
         self.group_owner_email = group_owner_email
         self.subgroup_owner_email = subgroup_owner_email
         self.subgroup_name = subgroup_name
         self.subgroup_start_date = subgroup_start_date
         self.subgroup_end_date = subgroup_end_date
         self.subgroup_bqid = subgroup_bqid
         self.subgroup_id = subgroup_id
+        self.autorenewal = autorenewal
+        self.comments = comments
+        self.end_date = end_date
+        self.international_deparments = international_deparments
+        self.opportunity_extension = opportunity_extension
+        self.maintance_project = maintance_project
+        self.ms_project_id = ms_project_id
+        self.operation_coordinator_name = operation_coordinator_name
+        self.operation_coordinator_controller = (
+            operation_coordinator_controller
+        )
+        self.operation_coordinator_sub = operation_coordinator_sub
+        self.opportunity = opportunity
+        self.periodicity = periodicity
+        self.profitcenter = profitcenter
+        self.project_account = project_account
+        self.projectcode = projectcode
+        self.revenue_details = revenue_details
+        self.status = status
+        self.internal_comment = internal_comment
+        self.rejection_reason = rejection_reason
+        self.projectid = projectid
+        self.quote = quote
 
     @staticmethod
     def from_salesforce_record(record):
+        project_line_items = (
+            [
+                ProjectLineItemDTO.from_salesforce_record(item, record["Id"])
+                for item in record.get("Project_Line_Items__r", {}).get(
+                    "records", []
+                )
+            ]
+            if record.get("Project_Line_Items__r")
+            else []
+        )
+
         def _get_account_business_name():
             try:
                 return normalize_value(
                     record["Project_Account__r"]["Business_Name__c"]
                 )
             except (TypeError, KeyError):
                 return ""
@@ -592,24 +647,142 @@
             try:
                 return record["Project_Account__r"]["LKP_CustomerSubgroup__r"][
                     "TXT_BQId__c"
                 ]
             except (TypeError, KeyError):
                 return ""
 
-        project_line_items = (
-            [
-                ProjectLineItemDTO.from_salesforce_record(item, record["Id"])
-                for item in record.get("Project_Line_Items__r", {}).get(
-                    "records", []
-                )
-            ]
-            if record.get("Project_Line_Items__r")
-            else []
-        )
+        def _get_autorenewal():
+            try:
+                return record["Autorenewal__c"]
+            except KeyError:
+                return False
+
+        def _get_comments():
+            try:
+                return record["Comments__c"]
+            except KeyError:
+                return ""
+
+        def _get_end_date():
+            try:
+                return record["End_Date__c"]
+            except KeyError:
+                return ""
+
+        def _get_international_deparments():
+            try:
+                return record["International_Departments__c"]
+            except KeyError:
+                return False
+
+        def _get_opportunity_extension():
+            try:
+                return record["LKP_OpportunityExtension__c"]
+            except KeyError:
+                return ""
+
+        def _get_maintance_project():
+            try:
+                return record["Maintenance_project__c"]
+            except KeyError:
+                return False
+
+        def _get_ms_project_id():
+            try:
+                return record["MS_Project_Id__c"]
+            except KeyError:
+                return False
+
+        def _get_operation_coordinator_name():
+            try:
+                return record["Operation_Coordinator__c"]["Name"]
+            except (KeyError, TypeError):
+                return ""
+
+        def _get_operation_coordinator_controller():
+            try:
+                return record["Operation_Coordinator__c"]["Controller__c"]
+            except (KeyError, TypeError):
+                return ""
+
+        def _get_operation_coordinator_sub():
+            try:
+                return record["Operation_Coordinator_Sub__c"]
+            except KeyError:
+                return ""
+
+        def _get_opportunity():
+            try:
+                return record["Opportunity__c"]
+            except KeyError:
+                return ""
+
+        def _get_periodicity():
+            try:
+                return record["Periodicity__c"]
+            except KeyError:
+                return ""
+
+        def _get_profitcenter():
+            try:
+                return record["LKP_ProfitCenter__c"]
+            except KeyError:
+                return ""
+
+        def _get_project_account():
+            try:
+                return record["Project_Account__c"]
+            except KeyError:
+                return ""
+
+        def _get_project_code():
+            try:
+                return record["Project_Code__c"]
+            except KeyError:
+                return ""
+
+        def _get_quote():
+            try:
+                return record["Quote__c"]
+            except KeyError:
+                return ""
+
+        def _get_revenue_details():
+            try:
+                return record["Revenue_Details__c"]
+            except KeyError:
+                return ""
+
+        def _get_status():
+            try:
+                return record["Status__c"]
+            except KeyError:
+                return ""
+
+        def _get_internal_comment():
+            try:
+                return record["TXT_InternalComment__c"]
+            except KeyError:
+                return ""
+
+        def _get_rejection_reason():
+            try:
+                return record["TXT_RejectionReason__c"]
+            except KeyError:
+                return ""
+
+        def _get_projectid():
+            try:
+                return record["ProjectID__c"]
+            except KeyError:
+                return ""
+
+        if _get_internal_comment():
+            print(record)
 
         return OpportunityDTO(
             account_business_name=_get_account_business_name(),
             account_name=_get_account_name(),
             account_id=_get_account_id(),
             currency=record["CurrencyIsoCode"],
             amount=record.get("RU_TotalAmount__c", 0.0),
@@ -670,14 +843,35 @@
             group_owner_email=_get_group_owner_email(),
             subgroup_owner_email=_get_subgroup_owner_emial(),
             subgroup_name=_get_subgroup_name(),
             subgroup_start_date=_get_subgroup_start(),
             subgroup_end_date=_get_subgroup_end(),
             subgroup_bqid=_get_subgroup_bqid(),
             subgroup_id=_get_subgroup_id(),
+            autorenewal=_get_autorenewal(),
+            comments=_get_comments(),
+            end_date=_get_end_date(),
+            international_deparments=_get_international_deparments(),
+            opportunity_extension=_get_opportunity_extension(),
+            maintance_project=_get_maintance_project(),
+            ms_project_id=_get_ms_project_id(),
+            operation_coordinator_name=_get_operation_coordinator_name(),
+            operation_coordinator_controller=_get_operation_coordinator_controller(),  # noqa: E501
+            operation_coordinator_sub=_get_operation_coordinator_sub(),
+            opportunity=_get_opportunity(),
+            periodicity=_get_periodicity(),
+            profitcenter=_get_profitcenter(),
+            project_account=_get_project_account(),
+            projectcode=_get_project_code(),
+            revenue_details=_get_revenue_details(),
+            status=_get_status(),
+            internal_comment=_get_internal_comment(),
+            rejection_reason=_get_rejection_reason(),
+            projectid=_get_projectid(),
+            quote=_get_quote(),
         )
 
     def add_billing_lines(self, billing_lines):
         self.billing_lines.extend(billing_lines)
 
     def to_dict(self):
         return {
@@ -746,8 +940,29 @@
             "subgroup_owner_email": self.subgroup_owner_email,
             "subgroup_name": self.subgroup_name,
             "subgroup_start_date": self.subgroup_start_date,
             "subgroup_end_date": self.subgroup_end_date,
             "subgroup_bqid": self.subgroup_bqid,
             "subgroup_subgroupid": self.subgroup_id,
             "subgroup_groupid": self.group_id,
+            "autorenewal": self.autorenewal,
+            "comments": self.comments,
+            "end_date": self.end_date,
+            "international_deparments": self.international_deparments,
+            "opportunity_extension": self.opportunity_extension,
+            "maintance_project": self.maintance_project,
+            "ms_project_id": self.ms_project_id,
+            "operation_coordinator_name": self.operation_coordinator_name,
+            "operation_coordinator_controller": self.operation_coordinator_controller,  # noqa: E501
+            "operation_coordinator_sub": self.operation_coordinator_sub,
+            "opportunity": self.opportunity,
+            "periodicity": self.periodicity,
+            "profitcenter": self.profitcenter,
+            "project_account": self.project_account,
+            "projectcode": self.projectcode,
+            "revenue_details": self.revenue_details,
+            "status": self.status,
+            "internal_comment": self.internal_comment,
+            "rejection_reason": self.rejection_reason,
+            "projectid": self.projectid,
+            "quote": self.quote,
         }
```

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,35 @@
                 "profit_center": "INTEGER",
                 "project_code": "STRING",
                 "project_id": "STRING",
                 "project_name": "STRING",
                 "project_start_date": "DATE",
                 "project_tier": "STRING",
                 "stage": "STRING",
+                "autorenewal": "BOOLEAN",
+                "comments": "STRING",
+                "end_date": "DATE",
+                "international_deparments": "BOOLEAN",
+                "opportunity_extension": "STRING",
+                "maintance_project": "BOOLEAN",
+                "ms_project_id": "STRING",
+                "operation_coordinator_name": "STRING",
+                "operation_coordinator_controller": "STRING",
+                "operation_coordinator_sub": "STRING",
+                "opportunity": "STRING",
+                "periodicity": "STRING",
+                "profitcenter": "STRING",
+                "project_account": "STRING",
+                "projectcode": "STRING",
+                "revenue_details": "BOOLEAN",
+                "status": "STRING",
+                "internal_comment": "STRING",
+                "rejection_reason": "STRING",
+                "projectid": "STRING",
+                "quote": "STRING",
             },
             "billing_lines": {
                 "billing_amount": "FLOAT",
                 "billing_date": "DATE",
                 "billing_period_ending_date": "DATE",
                 "billing_period_starting_date": "DATE",
                 "billing_plan_amount": "FLOAT",
```

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.4.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.3.0/pyproject.toml` & `ms_salesforce_api-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "2.3.0"
+version = "2.4.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-2.3.0/PKG-INFO` & `ms_salesforce_api-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

