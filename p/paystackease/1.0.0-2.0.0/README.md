# Comparing `tmp/paystackease-1.0.0.tar.gz` & `tmp/paystackease-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystackease-1.0.0.tar", max compression
+gzip compressed data, was "paystackease-2.0.0.tar", max compression
```

## Comparing `paystackease-1.0.0.tar` & `paystackease-2.0.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
--rwxr-xr-x   0        0        0     1090 2024-02-21 14:06:29.101210 paystackease-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     4976 2024-04-05 08:20:03.228602 paystackease-1.0.0/README.md
--rwxr-xr-x   0        0        0     1437 2024-04-05 08:20:03.231124 paystackease-1.0.0/paystackease/__init__.py
--rwxr-xr-x   0        0        0     8198 2024-04-05 01:26:16.260246 paystackease-1.0.0/paystackease/_abase.py
--rwxr-xr-x   0        0        0     7815 2024-04-05 01:26:16.262246 paystackease-1.0.0/paystackease/_base.py
--rwxr-xr-x   0        0        0      353 2024-04-05 01:26:16.263248 paystackease-1.0.0/paystackease/_utils.py
--rwxr-xr-x   0        0        0     5787 2024-03-19 18:44:47.663437 paystackease-1.0.0/paystackease/apaystack.py
--rwxr-xr-x   0        0        0     1549 2024-03-19 18:18:06.367036 paystackease-1.0.0/paystackease/apis/__init__.py
--rwxr-xr-x   0        0        0     2123 2024-04-05 08:20:03.232124 paystackease-1.0.0/paystackease/apis/apple_pay.py
--rwxr-xr-x   0        0        0     4314 2024-04-05 01:26:16.265246 paystackease-1.0.0/paystackease/apis/bulk_charges.py
--rwxr-xr-x   0        0        0     5821 2024-04-05 01:26:16.267246 paystackease-1.0.0/paystackease/apis/charges.py
--rwxr-xr-x   0        0        0     6728 2024-04-05 01:26:16.268247 paystackease-1.0.0/paystackease/apis/customers.py
--rwxr-xr-x   0        0        0     9220 2024-04-05 01:26:16.270245 paystackease-1.0.0/paystackease/apis/dedicated_virtual_accounts.py
--rwxr-xr-x   0        0        0     7920 2024-04-05 01:26:16.271246 paystackease-1.0.0/paystackease/apis/disputes.py
--rwxr-xr-x   0        0        0     1140 2024-04-05 01:26:16.272247 paystackease-1.0.0/paystackease/apis/integration.py
--rwxr-xr-x   0        0        0     4355 2024-04-05 01:26:16.273246 paystackease-1.0.0/paystackease/apis/miscellaneous.py
--rwxr-xr-x   0        0        0     5610 2024-04-05 01:26:16.275247 paystackease-1.0.0/paystackease/apis/payment_pages.py
--rwxr-xr-x   0        0        0     9778 2024-04-05 01:26:16.276247 paystackease-1.0.0/paystackease/apis/payment_requests.py
--rwxr-xr-x   0        0        0     4572 2024-04-05 01:26:16.277245 paystackease-1.0.0/paystackease/apis/plans.py
--rwxr-xr-x   0        0        0     4254 2024-04-05 01:26:16.279250 paystackease-1.0.0/paystackease/apis/products.py
--rwxr-xr-x   0        0        0     3250 2024-04-05 01:26:16.280246 paystackease-1.0.0/paystackease/apis/refund.py
--rwxr-xr-x   0        0        0     3302 2024-04-05 01:26:16.282247 paystackease-1.0.0/paystackease/apis/settlements.py
--rwxr-xr-x   0        0        0     6263 2024-04-05 01:26:16.283246 paystackease-1.0.0/paystackease/apis/subaccounts.py
--rwxr-xr-x   0        0        0     4306 2024-04-05 01:26:16.284248 paystackease-1.0.0/paystackease/apis/subscriptions.py
--rwxr-xr-x   0        0        0     5278 2024-04-05 01:26:16.285247 paystackease-1.0.0/paystackease/apis/terminal.py
--rwxr-xr-x   0        0        0     5758 2024-04-05 01:26:16.287246 paystackease-1.0.0/paystackease/apis/transaction_splits.py
--rwxr-xr-x   0        0        0    12570 2024-04-05 01:26:16.288246 paystackease-1.0.0/paystackease/apis/transactions.py
--rwxr-xr-x   0        0        0     5228 2024-04-05 01:26:16.289246 paystackease-1.0.0/paystackease/apis/transfer_recipients.py
--rwxr-xr-x   0        0        0     4769 2024-04-05 01:26:16.290248 paystackease-1.0.0/paystackease/apis/transfers.py
--rwxr-xr-x   0        0        0     2598 2024-04-05 01:26:16.291247 paystackease-1.0.0/paystackease/apis/transfers_control.py
--rwxr-xr-x   0        0        0     2789 2024-04-05 09:22:55.621501 paystackease-1.0.0/paystackease/apis/verification.py
--rwxr-xr-x   0        0        0     1826 2024-03-19 18:18:06.382037 paystackease-1.0.0/paystackease/async_apis/__init__.py
--rwxr-xr-x   0        0        0     2182 2024-04-05 08:20:03.234654 paystackease-1.0.0/paystackease/async_apis/aapple_pay.py
--rwxr-xr-x   0        0        0     4416 2024-04-05 01:26:16.295246 paystackease-1.0.0/paystackease/async_apis/abulk_charges.py
--rwxr-xr-x   0        0        0     5926 2024-04-05 01:26:16.296246 paystackease-1.0.0/paystackease/async_apis/acharges.py
--rwxr-xr-x   0        0        0     6836 2024-04-05 01:26:16.297246 paystackease-1.0.0/paystackease/async_apis/acustomers.py
--rwxr-xr-x   0        0        0     9357 2024-04-05 01:26:16.299246 paystackease-1.0.0/paystackease/async_apis/adedicated_virtual_accounts.py
--rwxr-xr-x   0        0        0     8045 2024-04-05 01:26:16.300246 paystackease-1.0.0/paystackease/async_apis/adisputes.py
--rwxr-xr-x   0        0        0     1185 2024-04-05 01:26:16.301247 paystackease-1.0.0/paystackease/async_apis/aintegration.py
--rwxr-xr-x   0        0        0     4409 2024-04-05 01:26:16.303247 paystackease-1.0.0/paystackease/async_apis/amiscellaneous.py
--rwxr-xr-x   0        0        0     5703 2024-04-05 01:26:16.305247 paystackease-1.0.0/paystackease/async_apis/apayment_pages.py
--rwxr-xr-x   0        0        0     9915 2024-04-05 01:26:16.306246 paystackease-1.0.0/paystackease/async_apis/apayment_requests.py
--rwxr-xr-x   0        0        0     4649 2024-04-05 01:26:16.308247 paystackease-1.0.0/paystackease/async_apis/aplans.py
--rwxr-xr-x   0        0        0     4331 2024-04-05 01:26:16.309248 paystackease-1.0.0/paystackease/async_apis/aproducts.py
--rwxr-xr-x   0        0        0     3315 2024-04-05 01:26:16.310247 paystackease-1.0.0/paystackease/async_apis/arefund.py
--rwxr-xr-x   0        0        0     3347 2024-04-05 01:26:16.311248 paystackease-1.0.0/paystackease/async_apis/asettlements.py
--rwxr-xr-x   0        0        0     6346 2024-04-05 01:26:16.312246 paystackease-1.0.0/paystackease/async_apis/asubaccounts.py
--rwxr-xr-x   0        0        0     4406 2024-04-05 01:26:16.313248 paystackease-1.0.0/paystackease/async_apis/asubscriptions.py
--rwxr-xr-x   0        0        0     5400 2024-04-05 01:26:16.314248 paystackease-1.0.0/paystackease/async_apis/aterminal.py
--rwxr-xr-x   0        0        0     5863 2024-04-05 01:26:16.315248 paystackease-1.0.0/paystackease/async_apis/atransaction_splits.py
--rwxr-xr-x   0        0        0    12717 2024-04-05 01:26:16.316249 paystackease-1.0.0/paystackease/async_apis/atransactions.py
--rwxr-xr-x   0        0        0     5329 2024-04-05 01:26:16.318246 paystackease-1.0.0/paystackease/async_apis/atransfer_recipients.py
--rwxr-xr-x   0        0        0     4870 2024-04-05 01:26:16.319247 paystackease-1.0.0/paystackease/async_apis/atransfers.py
--rwxr-xr-x   0        0        0     2699 2024-04-05 01:26:16.320247 paystackease-1.0.0/paystackease/async_apis/atransfers_control.py
--rwxr-xr-x   0        0        0     2854 2024-04-05 09:23:13.351851 paystackease-1.0.0/paystackease/async_apis/averification.py
--rwxr-xr-x   0        0        0      544 2024-04-05 08:20:03.235653 paystackease-1.0.0/paystackease/errors.py
--rwxr-xr-x   0        0        0      582 2024-04-05 08:20:03.238175 paystackease-1.0.0/paystackease/helpers/__init__.py
--rwxr-xr-x   0        0        0      768 2024-04-03 01:47:46.289946 paystackease-1.0.0/paystackease/helpers/convert.py
--rwxr-xr-x   0        0        0     3756 2024-04-04 20:07:23.519543 paystackease-1.0.0/paystackease/helpers/tool_kit.py
--rwxr-xr-x   0        0        0     3079 2024-03-19 18:44:47.645434 paystackease-1.0.0/paystackease/paystack.py
--rwxr-xr-x   0        0        0     2012 2024-04-05 08:18:54.694176 paystackease-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6133 1970-01-01 00:00:00.000000 paystackease-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1090 2024-02-21 14:06:29.101210 paystackease-2.0.0/LICENSE
+-rwxr-xr-x   0        0        0     4989 2024-04-19 08:56:04.255180 paystackease-2.0.0/README.md
+-rwxr-xr-x   0        0        0     1407 2024-04-19 07:37:11.942415 paystackease-2.0.0/paystackease/__init__.py
+-rwxr-xr-x   0        0        0     5768 2024-04-19 07:37:11.944394 paystackease-2.0.0/paystackease/apaystack.py
+-rwxr-xr-x   0        0        0     1041 2024-04-19 07:37:11.946391 paystackease-2.0.0/paystackease/apis/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-04-19 07:37:11.946391 paystackease-2.0.0/paystackease/apis/async_apis/__init__.py
+-rwxr-xr-x   0        0        0     2208 2024-04-19 07:37:11.947568 paystackease-2.0.0/paystackease/apis/async_apis/aapple_pay.py
+-rwxr-xr-x   0        0        0     4498 2024-04-19 07:37:11.949191 paystackease-2.0.0/paystackease/apis/async_apis/abulk_charges.py
+-rwxr-xr-x   0        0        0     6009 2024-04-19 07:37:11.949414 paystackease-2.0.0/paystackease/apis/async_apis/acharges.py
+-rwxr-xr-x   0        0        0     6947 2024-04-19 07:37:11.951390 paystackease-2.0.0/paystackease/apis/async_apis/acustomers.py
+-rwxr-xr-x   0        0        0     9518 2024-04-19 07:37:11.952391 paystackease-2.0.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py
+-rwxr-xr-x   0        0        0     8198 2024-04-19 07:37:11.953392 paystackease-2.0.0/paystackease/apis/async_apis/adisputes.py
+-rwxr-xr-x   0        0        0     1185 2024-04-19 07:37:11.954391 paystackease-2.0.0/paystackease/apis/async_apis/aintegration.py
+-rwxr-xr-x   0        0        0     4426 2024-04-19 07:37:11.955392 paystackease-2.0.0/paystackease/apis/async_apis/amiscellaneous.py
+-rwxr-xr-x   0        0        0     5801 2024-04-19 07:37:11.956393 paystackease-2.0.0/paystackease/apis/async_apis/apayment_pages.py
+-rwxr-xr-x   0        0        0    10076 2024-04-19 07:37:11.957476 paystackease-2.0.0/paystackease/apis/async_apis/apayment_requests.py
+-rwxr-xr-x   0        0        0     4690 2024-04-19 07:37:11.958390 paystackease-2.0.0/paystackease/apis/async_apis/aplans.py
+-rwxr-xr-x   0        0        0     4381 2024-04-19 07:37:11.959391 paystackease-2.0.0/paystackease/apis/async_apis/aproducts.py
+-rwxr-xr-x   0        0        0     3332 2024-04-19 07:37:11.960391 paystackease-2.0.0/paystackease/apis/async_apis/arefund.py
+-rwxr-xr-x   0        0        0     3340 2024-04-19 07:37:11.961390 paystackease-2.0.0/paystackease/apis/async_apis/asettlements.py
+-rwxr-xr-x   0        0        0     6387 2024-04-19 07:37:11.962392 paystackease-2.0.0/paystackease/apis/async_apis/asubaccounts.py
+-rwxr-xr-x   0        0        0     4528 2024-04-19 07:37:11.963391 paystackease-2.0.0/paystackease/apis/async_apis/asubscriptions.py
+-rwxr-xr-x   0        0        0     5537 2024-04-19 07:37:11.964391 paystackease-2.0.0/paystackease/apis/async_apis/aterminal.py
+-rwxr-xr-x   0        0        0     6009 2024-04-19 07:37:11.965390 paystackease-2.0.0/paystackease/apis/async_apis/atransaction_splits.py
+-rwxr-xr-x   0        0        0    12878 2024-04-19 07:37:11.966390 paystackease-2.0.0/paystackease/apis/async_apis/atransactions.py
+-rwxr-xr-x   0        0        0     5418 2024-04-19 07:37:11.967390 paystackease-2.0.0/paystackease/apis/async_apis/atransfer_recipients.py
+-rwxr-xr-x   0        0        0     4957 2024-04-19 07:37:11.968390 paystackease-2.0.0/paystackease/apis/async_apis/atransfers.py
+-rwxr-xr-x   0        0        0     2795 2024-04-19 07:37:11.969390 paystackease-2.0.0/paystackease/apis/async_apis/atransfers_control.py
+-rwxr-xr-x   0        0        0     2878 2024-04-19 07:37:11.970390 paystackease-2.0.0/paystackease/apis/async_apis/averification.py
+-rwxr-xr-x   0        0        0        0 2024-04-19 07:37:11.971391 paystackease-2.0.0/paystackease/apis/sync_apis/__init__.py
+-rwxr-xr-x   0        0        0     2154 2024-04-19 07:37:11.972390 paystackease-2.0.0/paystackease/apis/sync_apis/apple_pay.py
+-rwxr-xr-x   0        0        0     4405 2024-04-19 07:37:11.973390 paystackease-2.0.0/paystackease/apis/sync_apis/bulk_charges.py
+-rwxr-xr-x   0        0        0     5913 2024-04-19 07:37:11.975391 paystackease-2.0.0/paystackease/apis/sync_apis/charges.py
+-rwxr-xr-x   0        0        0     6848 2024-04-19 07:37:11.976390 paystackease-2.0.0/paystackease/apis/sync_apis/customers.py
+-rwxr-xr-x   0        0        0     9390 2024-04-19 07:37:11.977390 paystackease-2.0.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py
+-rwxr-xr-x   0        0        0     8082 2024-04-19 07:37:11.978395 paystackease-2.0.0/paystackease/apis/sync_apis/disputes.py
+-rwxr-xr-x   0        0        0     1149 2024-04-19 07:37:11.979583 paystackease-2.0.0/paystackease/apis/sync_apis/integration.py
+-rwxr-xr-x   0        0        0     4381 2024-04-19 07:37:11.980986 paystackease-2.0.0/paystackease/apis/sync_apis/miscellaneous.py
+-rwxr-xr-x   0        0        0     5717 2024-04-19 07:37:11.982162 paystackease-2.0.0/paystackease/apis/sync_apis/payment_pages.py
+-rwxr-xr-x   0        0        0     9948 2024-04-19 07:37:11.983416 paystackease-2.0.0/paystackease/apis/sync_apis/payment_requests.py
+-rwxr-xr-x   0        0        0     4622 2024-04-19 07:37:11.984565 paystackease-2.0.0/paystackease/apis/sync_apis/plans.py
+-rwxr-xr-x   0        0        0     4313 2024-04-19 07:37:11.985391 paystackease-2.0.0/paystackease/apis/sync_apis/products.py
+-rwxr-xr-x   0        0        0     3276 2024-04-19 07:37:11.986391 paystackease-2.0.0/paystackease/apis/sync_apis/refund.py
+-rwxr-xr-x   0        0        0     3304 2024-04-19 07:37:11.987391 paystackease-2.0.0/paystackease/apis/sync_apis/settlements.py
+-rwxr-xr-x   0        0        0     6313 2024-04-19 07:37:11.988571 paystackease-2.0.0/paystackease/apis/sync_apis/subaccounts.py
+-rwxr-xr-x   0        0        0     4437 2024-04-19 07:37:11.989391 paystackease-2.0.0/paystackease/apis/sync_apis/subscriptions.py
+-rwxr-xr-x   0        0        0     5424 2024-04-19 07:37:11.990390 paystackease-2.0.0/paystackease/apis/sync_apis/terminal.py
+-rwxr-xr-x   0        0        0     5913 2024-04-19 07:37:11.992392 paystackease-2.0.0/paystackease/apis/sync_apis/transaction_splits.py
+-rwxr-xr-x   0        0        0    12740 2024-04-19 07:37:11.993390 paystackease-2.0.0/paystackease/apis/sync_apis/transactions.py
+-rwxr-xr-x   0        0        0     5326 2024-04-19 07:37:11.995392 paystackease-2.0.0/paystackease/apis/sync_apis/transfer_recipients.py
+-rwxr-xr-x   0        0        0     4865 2024-04-19 07:37:11.996436 paystackease-2.0.0/paystackease/apis/sync_apis/transfers.py
+-rwxr-xr-x   0        0        0     2703 2024-04-19 07:37:11.997390 paystackease-2.0.0/paystackease/apis/sync_apis/transfers_control.py
+-rwxr-xr-x   0        0        0     2822 2024-04-19 07:37:11.998390 paystackease-2.0.0/paystackease/apis/sync_apis/verification.py
+-rwxr-xr-x   0        0        0      490 2024-04-19 07:37:11.999391 paystackease-2.0.0/paystackease/core/__init__.py
+-rwxr-xr-x   0        0        0     3921 2024-04-19 07:37:12.001391 paystackease-2.0.0/paystackease/core/_api_base.py
+-rwxr-xr-x   0        0        0     5859 2024-04-19 07:37:12.002463 paystackease-2.0.0/paystackease/core/_api_base_client.py
+-rwxr-xr-x   0        0        0     4845 2024-04-19 07:37:12.003393 paystackease-2.0.0/paystackease/core/_api_client_requests.py
+-rwxr-xr-x   0        0        0      683 2024-04-19 07:37:12.004392 paystackease-2.0.0/paystackease/core/_api_client_response.py
+-rwxr-xr-x   0        0        0     1009 2024-04-19 07:37:12.006389 paystackease-2.0.0/paystackease/core/_api_errors.py
+-rwxr-xr-x   0        0        0      582 2024-04-05 08:20:03.238175 paystackease-2.0.0/paystackease/helpers/__init__.py
+-rwxr-xr-x   0        0        0      768 2024-04-03 01:47:46.289946 paystackease-2.0.0/paystackease/helpers/convert.py
+-rwxr-xr-x   0        0        0     3756 2024-04-04 20:07:23.519543 paystackease-2.0.0/paystackease/helpers/tool_kit.py
+-rwxr-xr-x   0        0        0     3064 2024-04-19 07:37:12.008473 paystackease-2.0.0/paystackease/paystack.py
+-rwxr-xr-x   0        0        0     2035 2024-04-19 08:11:17.248078 paystackease-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 paystackease-2.0.0/PKG-INFO
```

### Comparing `paystackease-1.0.0/LICENSE` & `paystackease-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paystackease-1.0.0/README.md` & `paystackease-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PayStackEase Library  
 
-------
+--------------
 
-![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
+![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease.svg) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
 
 
 **PayStackEase API Library**  is a Python library that simplifies interacting with the Paystack API. 
 It provides both asynchronous and synchronous wrappers for various Paystack functionalities, 
 making it easier to integrate payment processing into your Python projects.
 
 > 📝: Read more on paystack api documentation: [Paystack API DOCUMENTATION](https://paystack.com/docs/api/)
@@ -36,15 +36,15 @@
        ```
     * Activate the virtual environment
 
         ```
             <environment_name>\Scripts\activate
        ```
 
-2. For Unix/MacOS
+2. For Unix/macOS
 
     * Create virtual environment
 
         ```
             python3 -m venv <environment_name>
        ```
     * Activate the virtual environment
@@ -71,24 +71,24 @@
 > poetry add paystackease
 
 
 ## If you want to download the sdist packages directly:
 
 Download the wheel distribution file and install using pip
 
->  pip install paystackease-1.0.0-py3-none-any.whl 
+>  pip install paystackease-2.0.0-py3-none-any.whl 
 
 Download the source distribution file, and install using pip
 
-> pip install paystackease-1.0.0.tar.gz 
+> pip install paystackease-2.0.0.tar.gz 
 
 
 ## To get a development version of paystackease
 
-Clone from the ``dev`` branch github repository, unzip and install:
+Clone from the ``dev`` branch GitHub repository, unzip and install:
 
 > git clone -b dev https://github.com/cla-bit/PayStackEase.git
 
 > cd PayStackEase
 
 > pip install paystackease
 
@@ -123,15 +123,15 @@
     create_transaction = paystack_client.transactions.initialize(
         email="johndoe@email.com",
         amount=10000000)
     
     print(f"Transaction Created: {create_transaction}")
 ```
 
-> ✅: **Good**: You can check your Paystack account, go to the Transaction page and you will see the transaction just created.
+> ✅: **Good**: You can check your Paystack account, go to the Transaction page, and you will see the transaction just created.
 
 
 # Other Tools
 Similar to calling the PayStackBase, you can also call other tools to make your work easy. For example:
 
 * ### Account Type
 ```apacheconf
```

### Comparing `paystackease-1.0.0/paystackease/__init__.py` & `paystackease-2.0.0/paystackease/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """ Wrappers for Paystack API calls"""
-
-from paystackease.apaystack import AsyncPayStackBase
-from paystackease.errors import (
+from paystackease.core import (
     PayStackError,
     SecretKeyError,
     TypeValueError,
     InvalidRequestMethodError
 )
+from paystackease.apaystack import AsyncPayStackBase
 from paystackease.paystack import PayStackBase
-from paystackease.helpers import convert_to_subunit
 from paystackease.helpers import (
+    convert_to_subunit,
     AccountType,
     Bearer,
     Currency,
     Channels,
     DisputeStatus,
     DocumentType,
     DVABank,
@@ -66,8 +65,8 @@
     'Resolution',
     'RiskAction',
     'SettlementSchedule',
     'SplitType',
     'STATUS',
     'TransactionStatus',
     'USSD',
-]
+]
```

### Comparing `paystackease-1.0.0/paystackease/_abase.py` & `paystackease-2.0.0/paystackease/apis/async_apis/adisputes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,257 +1,218 @@
 """
-Async Base client API for Paystack API with methods for handling asynchronous AIOHTTP requests,
-authentication using a secret key,
-constructing HTTP headers, joining URLs with the API base URL, and logging response information.
+Wrapper for Asynchronous Paystack Disputes API
+
+The Disputes API allows you manage transaction disputes on your integration.
 """
 
-import json
-import logging
+from datetime import date
+from typing import Optional, Union
 
-from datetime import date, datetime
-from typing import Union, Optional, Dict, List, Any
-from urllib.parse import urljoin
-from decouple import config
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import DisputeStatus, Resolution
 
-import aiohttp
-from paystackease._utils import Response
 
-from paystackease.errors import (
-    SecretKeyError,
-    TypeValueError,
-    InvalidRequestMethodError,
-    PayStackError,
-)
+class AsyncDisputesClientAPI(AsyncRequestAPI):
+    """
+    Paystack Disputes API
+    Reference: https://paystack.com/docs/api/dispute/
+    """
+
+    async def list_disputes(
+            self,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> PayStackResponse:
+        """
+        List disputes filed against you
+
+        :param: from_date: A timestamp from which to start listing dispute e.g. 2016-09-21
+        :param: to_date: A timestamp from which to start listing dispute e.g. 2016-09-21
+        :param: per_page:
+        :param: page:
+        :param: transaction_id:
+        :param: status: Dispute Status. Acceptable values:
+                        { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+            "transaction": transaction_id,
+            "status": status,
+        }
+        return await self._get_request("/dispute", params=params)
 
+    async def fetch_dispute(self, dispute_id: str) -> PayStackResponse:
+        """
+        Fetch details about a dispute
 
-logger = logging.getLogger(__name__)
+        :param: dispute_id: The dispute ID to fetch
 
-PAYSTACK_SECRET_KEY = config("PAYSTACK_SECRET_KEY")
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/dispute/{dispute_id}")
 
+    async def list_transaction_disputes(self, transaction_id: str) -> PayStackResponse:
+        """
+        List disputes for a transaction
 
-class AsyncBaseClientAPI:
-    """Base Client API for Paystack API"""
+        :param: transaction_id: The transaction id to fetch
 
-    _PAYSTACK_API_URL: str = "https://api.paystack.co/"
-    _VALID_HTTP_METHODS: set[str] = {"GET", "POST", "PUT", "DELETE"}
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        return await self._get_request(f"/dispute/transaction/{transaction_id}")
 
-    # pylint: disable=too-few-public-methods
-    def __init__(self, secret_key: str = None) -> None:
-        self._secret_key = secret_key
+    async def update_dispute(
+            self,
+            dispute_id: str,
+            refund_amount: int,
+            uploaded_filename: Optional[Union[str, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Update details of a dispute
 
-        # Default to PAYSTACK_SECRET_KEY if not provided in the instance
-        if not self._secret_key:
-            self._secret_key = PAYSTACK_SECRET_KEY  # or environment variables
+        :param: dispute_id: The dispute id to fetch
+        :param: refund_amount: The amount to refund to the customer
+        :param: uploaded_filename: filename of attachment returned via
+                                    PayStackResponse from upload url(GET /dispute/:id/upload_url)
 
-        # Raise an error if PAYSTACK_SECRET_KEY is not set in the instance or environment variables
-        if not self._secret_key:
-            logger.error(
-                "Please provide a secret key or set the environment variable PAYSTACK_SECRET_KEY"
-            )
-            raise SecretKeyError(
-                "Please provide a secret key or set the environment variable PAYSTACK_SECRET_KEY"
-            )
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {"refund_amount": refund_amount, "uploaded_filename": uploaded_filename}
+        return await self._put_request(f"/dispute/{dispute_id}", data=data)
 
-        self.timeout = aiohttp.ClientTimeout(total=30)
+    async def add_evidence(
+            self,
+            dispute_id: str,
+            customer_email: str,
+            customer_name: str,
+            customer_phone: str,
+            service_details: str,
+            delivery_address: Optional[Union[str, None]] = None,
+            delivery_date: Optional[Union[date, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Add evidence to a dispute
 
-        self._session = aiohttp.ClientSession(
-            headers=self._make_paystack_http_headers(), timeout=self.timeout
-        )
+        :param: dispute_id: The dispute id to fetch
+        :param: customer_email: The customer email
+        :param: customer_name: The customer name
+        :param: customer_phone: The customer phone
+        :param: service_details: The service details
+        :param: delivery_address: The delivery address
+        :param: delivery_date: The delivery date: YYYY-MM-DD
 
-    async def __aenter__(self):
-        return self
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
 
-    async def __aexit__(self, exc_type, exc, tb):
-        if not self._session.closed:
-            await self._session.close()
+        # convert date to string
+        delivery_date = self._convert_to_string(delivery_date)
 
-    @classmethod
-    def _set_secret_key(cls, secret_key: str) -> None:
-        """Set the secret key for all instances of this class"""
-        cls._secret_key = secret_key
+        data = {
+            "customer_email": customer_email,
+            "customer_name": customer_name,
+            "customer_phone": customer_phone,
+            "service_details": service_details,
+            "delivery_address": delivery_address,
+            "delivery_date": delivery_date,
+        }
+        return await self._post_request(f"/dispute/{dispute_id}/evidence", data=data)
 
-    def _join_url(self, path: str) -> str:
+    async def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> PayStackResponse:
         """
-        Join URL with Paystack API URL
-        :param path:
-        :return:
-        """
-        if path.startswith("/"):
-            path = path[1:]
-        return urljoin(self._PAYSTACK_API_URL, path)
+        Get upload url for dispute evidence
 
-    def _make_paystack_http_headers(self) -> dict:
-        """
-        Make Paystack HTTP Headers
-        :return:
-        """
-        return {
-            "Authorization": f"Bearer {self._secret_key}",
-            "content-type": "application/json",
-        }
+        :param: dispute_id: The dispute id to fetch
+        :param: uploaded_filename: The file name, with its extension, that you want to upload. e.g. filename.pdf
 
-    @staticmethod
-    def _convert_to_string(
-        value: Union[bool, date, datetime, None]
-    ) -> Union[str, int, None]:
-        """
-        Convert the type of value to a string
-        :param value: The value to be converted
-
-        :raise TypeError: if the value is not a supported type
-
-        :return: The value as a string
-        :rtype: str
-        """
-        # each supported type is mapped to its corresponding conversion function
-        conversion_functions = {
-            bool: lambda val: str(val),
-            date: lambda val: val.strftime("%Y-%m-%d"),
-            datetime: lambda val: val.strftime("%Y-%m-%d %H:%M:%S"),  # Added a datetime
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        params = {"uploaded_filename": uploaded_filename}
+        return await self._get_request(f"/dispute/{dispute_id}/upload_url", params=params)
+
+    async def resolve_dispute(
+            self,
+            dispute_id: str,
+            resolution: Resolution,
+            message: str,
+            refund_amount: int,
+            uploaded_filename: str,
+            evidence: Optional[Union[int, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Resolve a dispute
+
+        :param: dispute_id: The dispute id to fetch
+        :param: resolution: The resolution to resolve the dispute: Accepted values: { merchant-accepted | declined }.
+        :param: message: The message for resolution
+        :param: refund_amount: The amount to refund to the customer
+        :param: uploaded_filename: filename of attachment returned via PayStackResponse from method get_upload_url
+        :param: evidence: The evidence id for fraud claims
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+        data = {
+            "resolution": resolution,
+            "message": message,
+            "refund_amount": refund_amount,
+            "uploaded_filename": uploaded_filename,
+            "evidence": evidence,
         }
+        return await self._put_request(f"/dispute/{dispute_id}/resolve", data=data)
 
-        if value is None:
-            return None
-        if type(value) in conversion_functions:
-            return conversion_functions[type(value)](value)
-        logger.error(
-            "Unsupported type: %s Expected type -bool, -date, -datetime", {type(value)}
-        )
-        raise TypeValueError(
-            f"Unsupported type: {type(value)}. Expected type -bool, -date, -datetime"
-        )
-
-    async def _request_url(
-        self,
-        method: str,
-        url: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> Response:
-        """
-        Handles the request to Paystack API
-        :param method:
-        :param url:
-        :param data:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        if method.upper() not in self._VALID_HTTP_METHODS:
-            logger.error(
-                "Invalid HTTP method. Supported methods are GET, POST, PUT, DELETE. : %s",
-                {method},
-            )
-            raise InvalidRequestMethodError(
-                f"Invalid HTTP method. Supported methods are GET, POST, PUT, DELETE. : {method}"
-            )
-
-        url = self._join_url(url)
-        # Filtering params and data, then converting data to JSON
-        params = (
-            {key: value for key, value in params.items() if value is not None}
-            if params
-            else None
-        )
-        data = json.dumps(data) if data else None
-
-        try:
-            async with self._session.request(
-                method,
-                url=url,
-                data=data,
-                params=params,
-                **kwargs,
-            ) as response:
-                response_json = await response.json()
-                logger.info("Response Status Code: %s", response.status)
-                logger.info("Response JSON: %s", response_json)
-                return response_json
-        except aiohttp.ClientError as error:
-            # Extract status code if available from the exception
-            status_code = getattr(error, "response", None) and getattr(
-                error.args[0], "status_code", None
-            )
-            logger.error("Error: %s", error)
-            raise PayStackError(
-                f"Error making request to Paystack API: {str(error)}", status_code
-            ) from error
-
-
-class AsyncPayStackBaseClientAPI(AsyncBaseClientAPI):
-    """Requests methods to Paystack API"""
-
-    async def _request(
-        self,
-        method: str,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> Response:
-        """
-        Handles the request to Paystack API
-        :param method:
-        :param endpoint:
-        :param data:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        return await self._request_url(
-            method, endpoint, data=data, params=params, **kwargs
-        )
-
-    async def _get_request(
-        self,
-        endpoint: str,
-        params: Optional[Union[Dict[str, Any], None]] = None,
-        **kwargs,
-    ) -> Response:
-        """
-        Makes the GET request to Paystack API
-        :param endpoint:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("GET", endpoint, params=params, **kwargs)
-
-    async def _post_request(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> Response:
-        """
-        Makes the POST request to Paystack API
-        :param endpoint:
-        :param data:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("POST", endpoint, data=data, **kwargs)
-
-    async def _put_request(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> Response:
-        """
-        Makes the PUT request to Paystack API
-        :param endpoint:
-        :param data:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("PUT", endpoint, data=data, **kwargs)
-
-    async def _delete_request(self, endpoint: str, **kwargs) -> Response:
-        """
-        Makes the DELETE request to Paystack API
-        :param endpoint:
-        :param kwargs:
-        :return:
-        """
-        return await self._request("DELETE", endpoint, **kwargs)
+    async def export_disputes(
+            self,
+            per_page: Optional[Union[int, None]] = 50,
+            page: Optional[Union[int, None]] = 1,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+            transaction_id: Optional[Union[str, None]] = None,
+            status: Optional[Union[DisputeStatus, None]] = None,
+    ) -> PayStackResponse:
+        """
+        Export disputes
+
+        :param: per_page:
+        :param: page:
+        :param: from_date: The start date to fetch disputes from
+        :param: to_date: The end date to fetch disputes from
+        :param: transaction_id: The transaction ID
+        :param: status: The dispute status:
+                        Acceptable values: { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
+
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
+        """
+
+        # convert date to string
+        from_date = self._convert_to_string(from_date)
+        to_date = self._convert_to_string(to_date)
+
+        params = {
+            "perPage": per_page,
+            "page": page,
+            "from": from_date,
+            "to": to_date,
+            "transaction": transaction_id,
+            "status": status,
+        }
+        return await self._get_request("/dispute/export", params=params)
```

### Comparing `paystackease-1.0.0/paystackease/apaystack.py` & `paystackease-2.0.0/paystackease/apaystack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Wrapper classes for various Asynchronous Paystack API endpoints,
 providing simplified access to functionality in Paystack
 """
 
-from paystackease.async_apis import (
+from paystackease.apis.async_apis import (
     aapple_pay,
     abulk_charges,
     acharges,
     acustomers,
     adedicated_virtual_accounts,
     adisputes,
     aintegration,
@@ -23,18 +23,18 @@
     atransaction_splits,
     atransactions,
     atransfer_recipients,
     atransfers,
     atransfers_control,
     averification,
 )
-from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease.core import AsyncRequestAPI
 
 
-class AsyncPayStackBase(AsyncPayStackBaseClientAPI):
+class AsyncPayStackBase(AsyncRequestAPI):
     """AsyncPayStackBase acts as a wrapper around various client APIs to
     interact with the PayStack API
     """
 
     # pylint: disable=too-many-instance-attributes
     def __init__(self, secret_key=None):
         super().__init__(secret_key)
```

### Comparing `paystackease-1.0.0/paystackease/apis/apple_pay.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/apple_pay.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 """
 Wrapper class for Paystack Apple Pay API.
 
 The Apple Pay API allows you register your application's top-level domain or subdomain.
 """
 
 from typing import Optional, Union
+from paystackease.core import PayStackResponse, SyncRequestAPI
 
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
 
-
-class ApplePayClientAPI(PayStackBaseClientAPI):
+class ApplePayClientAPI(SyncRequestAPI):
     """
     Paystack Apple Pay API
     Reference: https://paystack.com/docs/api/apple-pay/
     """
 
-    def register_domain(self, domain_name: str) -> Response:
+    def register_domain(self, domain_name: str) -> PayStackResponse:
         """
         Register a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "domainName": domain_name,
         }
         return self._post_request("/apple-pay/domain", data=data)
 
     def list_domains(
             self,
             use_cursor: Optional[Union[bool, None]] = False,
             next_page: Optional[Union[int, None]] = None,
             previous_page: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all registered domains
 
         :param: use_cursor  # use cursor for pagination
         :param: next_page  # next page
         :param: previous_page  # previous page
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         use_cursor = self._convert_to_string(use_cursor)
 
         params = {
             "use_cursor": use_cursor,
             "next": next_page,
             "previous": previous_page,
         }
         return self._get_request("/apple-pay/domain", params=params)
 
-    def unregister_domain(self, domain_name: str) -> Response:
+    def unregister_domain(self, domain_name: str) -> PayStackResponse:
         """
         Unregister a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "domainName": domain_name,
         }
         return self._delete_request("/apple-pay/domain", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/apis/bulk_charges.py` & `paystackease-2.0.0/paystackease/apis/async_apis/abulk_charges.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-""" Wrapper for Paystack Bulk Charges API.
+"""
+Wrapper for Asynchronous Paystack Bulk Charges API.
 
 The Bulk Charges API allows you to create and manage multiple recurring payments from your customers.
 """
 
 from datetime import date
 from typing import List, Dict, Optional, Any, Union
 
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import STATUS
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import STATUS
 
 
-class BulkChargesClientAPI(PayStackBaseClientAPI):
+class AsyncBulkChargesClientAPI(AsyncRequestAPI):
     """
     Paystack Bulk Charges API
     Reference: https://paystack.com/docs/api/bulk-charge/
     """
 
-    def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> Response:
+    async def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> PayStackResponse:
         """
         Send an array of objects with authorization codes and amount
 
         :param: objects
 
         note::
 
             A list of dictionary with authorization codes, amount and reference as keys
-            [{"authorization_code": "123456", "amount": 1000, "reference": "123456" }]
+            [{"authorization": "123456", "amount": 1000, "reference": "123456" }]
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._post_request("/bulkcharge", data=objects)
+        return await self._post_request("/bulkcharge", data=objects)
 
-    def list_bulk_charge_batches(
+    async def list_bulk_charge_batches(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all bulk charges
 
         :param: per_page
         :param: page
         :param: from_date
         :param: to_date
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/bulkcharge", params=params)
+        return await self._get_request("/bulkcharge", params=params)
 
-    def fetch_bulk_charge_batch(self, id_or_code: str) -> Response:
+    async def fetch_bulk_charge_batch(self, id_or_code: str) -> PayStackResponse:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/bulkcharge/{id_or_code}")
+        return await self._get_request(f"/bulkcharge/{id_or_code}")
 
-    def fetch_charge_bulk_batch(
+    async def fetch_charge_bulk_batch(
             self,
             id_or_code: str,
             status: Optional[Union[STATUS, None]] = None,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
         :param: status:  {STATUS.value.value}
         :param: per_page
         :param: page
@@ -99,45 +99,45 @@
         :param: to_date
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
             status: STATUS.value.value
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "status": status,
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
+        return await self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
 
-    def pause_bulk_charge_batch(self, batch_code: str) -> Response:
+    async def pause_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
         """
         Pause a bulk charge of a specific batch
 
         :param: batch_code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/bulkcharge/pause/{batch_code}")
+        return await self._get_request(f"/bulkcharge/pause/{batch_code}")
 
-    def resume_bulk_charge_batch(self, batch_code: str) -> Response:
+    async def resume_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
         """
         Resume a bulk charge of a specific batch
 
         :param: batch_code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/bulkcharge/resume/{batch_code}")
+        return await self._get_request(f"/bulkcharge/resume/{batch_code}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/charges.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/charges.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 Wrapper for Paystack Charges API.
 
 The Charge API allows you to configure payment channel of your choice when initiating a payment.
 """
 
 from datetime import date
 from typing import Optional, Dict, Any, List, Union
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import PWT
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import PWT
 
-class ChargesClientAPI(PayStackBaseClientAPI):
+
+class ChargesClientAPI(SyncRequestAPI):
     """
     Paystack Charges API
     Reference: https://paystack.com/docs/api/charge/
     """
 
     def create_charge(
             self,
             email: str,
             amount: int,
-            pin: Optional[Union[int, None]] = None,
+            metadata: Dict[str, List[Dict[str, Any]]],
             authorization_code: Optional[Union[str, None]] = None,
+            pin: Optional[Union[int, None]] = None,
             reference: Optional[Union[str, None]] = None,
             device_id: Optional[Union[str, None]] = None,
             bank: Optional[Union[Dict[str, str], None]] = None,
             bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
             qr: Optional[Union[Dict[str, str], None]] = None,
             ussd: Optional[Union[Dict[str, str], None]] = None,
             mobile_money: Optional[Union[Dict[str, str], None]] = None,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a charge
 
         :param: email
         :param: amount
         :param: bank. (Set key ass: {code, account_number})
         :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
@@ -60,130 +60,130 @@
             * mobile_money
 
             Send with a non-reusable authorization code:
             * pin
 
             mobile_money is only available in Ghana and Kenya
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "amount": amount,
+            "metadata": metadata,
             "authorization_code": authorization_code,
             "bank": bank,
             "bank_transfer": bank_transfer,
             "qr": qr,
             "pin": pin,
             "reference": reference,
             "ussd": ussd,
             "mobile_money": mobile_money,
             "device_id": device_id,
-            "metadata": metadata,
         }
         return self._post_request("/charge", data=data)
 
-    def submit_pin(self, pin: int, reference: str) -> Response:
+    def submit_pin(self, pin: int, reference: str) -> PayStackResponse:
         """
         Submit a PIN for a charge
 
         :param: pin
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "pin": pin,
             "reference": reference,
         }
         return self._post_request("/charge/submit_pin", data=data)
 
-    def submit_otp(self, otp: int, reference: str) -> Response:
+    def submit_otp(self, otp: int, reference: str) -> PayStackResponse:
         """
         Submit OTP to complete a charge
 
         :param: otp
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "otp": otp,
             "reference": reference,
         }
         return self._post_request("/charge/submit_otp", data=data)
 
-    def submit_phone(self, phone: str, reference: str) -> Response:
+    def submit_phone(self, phone: str, reference: str) -> PayStackResponse:
         """
         Submit a phone number to complete a charge
 
         :param: phone
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "phone": phone,
             "reference": reference,
         }
         return self._post_request("/charge/submit_phone", data=data)
 
-    def submit_birthday(self, birthday: date, reference: str) -> Response:
+    def submit_birthday(self, birthday: date, reference: str) -> PayStackResponse:
         """
         Submit birthday when required
 
         :param: birthday
         :param: reference
 
         note::
 
             Birthday submitted by user e.g. 2016-09-21
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         birthday = self._convert_to_string(birthday)
 
         data = {
             "birthday": birthday,
             "reference": reference,
         }
         return self._post_request("/charge/submit_birthday", data=data)
 
     def submit_address(
             self, reference: str, address: str, city: str, state: str, zipcode: str
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Submit address to continue a charge
 
         :param: reference
         :param: address
         :param: city
         :param: state
         :param: zipcode
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "reference": reference,
             "address": address,
             "city": city,
             "state": state,
             "zip_code": zipcode,
         }
         return self._post_request("/charge/submit_address", data=data)
 
-    def check_pending_charge(self, reference: str) -> Response:
+    def check_pending_charge(self, reference: str) -> PayStackResponse:
         """
         Check pending charge
 
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/charge/{reference}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/customers.py` & `paystackease-2.0.0/paystackease/apis/async_apis/acustomers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,186 +1,185 @@
 """
-Wrapper for Paystack Customers API.
+Wrapper for Asynchronous Paystack Customers API.
 
 The Customers API allows you to create and manage customers on your integration.
 """
 
 from datetime import date
-
 from typing import Optional, Dict, Any, Union
-from paystackease.helpers.tool_kit import RiskAction
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
+
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import RiskAction
 
 
-class CustomerClientAPI(PayStackBaseClientAPI):
+class AsyncCustomerClientAPI(AsyncRequestAPI):
     """
     Paystack Customer API
     Reference: https://paystack.com/docs/api/customer/
     """
 
-    def create_customer(
-            self, 
-            email: str, 
-            first_name: str, 
-            last_name: str, 
-            phone: str, 
+    async def create_customer(
+            self,
+            email: str,
+            first_name: str,
+            last_name: str,
+            phone: str,
             metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return self._post_request("/customer", data=data)
+        return await self._post_request("/customer", data=data)
 
-    def validate_customer(
+    async def validate_customer(
             self,
             email_or_code: str,
             first_name: str,
             last_name: str,
             account_type: str,
             country: str,
             bank_code: str,
             account_number: str,
             bvn: str,
             customer_id_num: Optional[Union[str, None]] = None,
             middle_name: Optional[Union[str, None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Validate a customer's identity
 
         :param: email_or_code: The email or code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: middle_name: The middle name of the customer.
         :param: account_type: The type of account. Only bank_account is currently supported.
         :param: customer_id_num: The customer identification number
         :param: country: The country of the customer. 2-letter country code of identification issuer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: account_number: The account number of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "middle_name": middle_name,
             "type": account_type,
             "value": customer_id_num,
             "country": country,
             "bvn": bvn,
             "bank_code": bank_code,
             "account_number": account_number,
         }
-        return self._post_request(f"customer/{email_or_code}/identification", data=data)
+        return await self._post_request(f"customer/{email_or_code}/identification", data=data)
 
-    def whitelist_blacklist_customer(
+    async def whitelist_blacklist_customer(
             self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Whitelist or blacklist a customer
 
         :param: email_or_code: The code or email of the customer.
         :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "customer": email_or_code,
             "risk_action": risk_action
         }
-        return self._post_request("/customer/set_risk_action", data=data)
+        return await self._post_request("/customer/set_risk_action", data=data)
 
-    def deactivate_authorization(self, authorization_code: str) -> Response:
+    async def deactivate_authorization(self, authorization_code: str) -> PayStackResponse:
         """
         Deactivate an authorization when the card needs to be forgotten
 
         :param: authorization_code: The authorization code to be deactivated.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"authorization_code": authorization_code}
-        return self._post_request("/customer/deactivate_authorization", data=data)
+        return await self._post_request("/customer/deactivate_authorization", data=data)
 
-    def update_customer(
+    async def update_customer(
             self,
             customer_code: str,
             first_name: Optional[Union[str, None]] = None,
             last_name: Optional[Union[str, None]] = None,
             phone: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a customer
 
         :param: customer_code: The code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return self._put_request(f"/customer/{customer_code}", data=data)
+        return await self._put_request(f"/customer/{customer_code}", data=data)
 
-    def fetch_customer(self, email_or_code: str) -> Response:
+    async def fetch_customer(self, email_or_code: str) -> PayStackResponse:
         """
         Fetch details of a specific customer
 
         :param: email_or_code: The email or code of the customer.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/customer/{email_or_code}")
+        return await self._get_request(f"/customer/{email_or_code}")
 
-    def list_customers(
+    async def list_customers(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all customers
 
         :param: per_page: The number of records to return.
         :param: page: The page number to return.
         :param: from_date: The date to start returning customers from
         :param: to_date: The date to stop returning customers from
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date  to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/customer", params=params)
+        return await self._get_request("/customer", params=params)
```

### Comparing `paystackease-1.0.0/paystackease/apis/dedicated_virtual_accounts.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/dedicated_virtual_accounts.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Wrapper for Paystack Dedicated Virtual Account API
 
 The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import Currency
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
 
-class DedicatedVirtualAccountClientAPI(PayStackBaseClientAPI):
+
+class DedicatedVirtualAccountClientAPI(SyncRequestAPI):
     """
     Paystack Dedicated Virtual Account API
     Reference: https://paystack.com/docs/api/dedicated-virtual-account/
 
     note::
         Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
     """
@@ -25,15 +25,15 @@
             customer_id_or_code: str,
             preferred_bank: Optional[Union[str, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             split_code: Optional[Union[str, None]] = None,
             first_name: Optional[Union[str, None]] = None,
             last_name: Optional[Union[str, None]] = None,
             phone: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a dedicated virtual account for existing customers.
         Currently, support Wema Bank and Titan Paystack.
 
         :param: customer_id_or_code: The customer's ID or Code
         :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
 
@@ -43,16 +43,16 @@
 
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
         :param: first_name: First name of the customer
         :param: last_name: Last name of the customer
         :param: phone: Phone number of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
             "first_name": first_name,
@@ -70,15 +70,15 @@
             preferred_bank: str,
             country: str,
             account_number: Optional[Union[str, None]] = None,
             bvn: Optional[Union[str, None]] = None,
             bank_code: Optional[Union[str, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             split_code: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         create a customer, validate the customer, and assign a DVA to the customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
@@ -96,16 +96,16 @@
 
         :param: account_number: The account number of the customer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "preferred_bank": preferred_bank,
@@ -121,129 +121,129 @@
     def list_dedicated_account(
             self,
             active: Optional[Union[bool, None]] = True,
             currency: Optional[Union[Currency, None]] = None,
             provider_slug: Optional[Union[str, None]] = None,
             bank_id: Optional[Union[str, None]] = None,
             customer_id: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List dedicated accounts
 
         :param: active: Shows the status of the dedicated virtual account
         :param: currency: Currency of the dedicated virtual account
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: bank_id: Bank ID of the dedicated virtual account eg: 035
         :param: customer_id: Customer ID of the dedicated virtual account
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert date to string
         active = self._convert_to_string(active)
 
         params = {
             "active": active,
             "currency": currency,
             "provider_slug": provider_slug,
             "bank_id": bank_id,
             "customer": customer_id,
         }
         return self._get_request("/dedicated_account", params=params)
 
-    def fetch_dedicated_account(self, dedicated_account_id: int) -> Response:
+    def fetch_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
         """
         Get details of a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/dedicated_account/{dedicated_account_id}")
 
     def requery_dedicated_account(
             self,
             account_number: Optional[Union[str, None]] = None,
             provider_slug: Optional[Union[str, None]] = None,
             date_transfer: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Requery a dedicated virtual account for new transactions
 
         :param: account_number: Virtual Account number to requery
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: date_transfer: Date of when the transfer was made
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         date_transfer = self._convert_to_string(date_transfer)
 
         params = {
             "account_number": account_number,
             "provider_slug": provider_slug,
             "date": date_transfer,
         }
         return self._get_request("/dedicated_account/requery", params=params)
 
-    def deactivate_dedicated_account(self, dedicated_account_id: int) -> Response:
+    def deactivate_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
         """
         Deactivate a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._delete_request(f"/dedicated_account/{dedicated_account_id}")
 
     def split_dedicated_account(
             self,
             customer_id_or_code: str,
             subaccount: Optional[Union[str, None]] = None,
             split_code: Optional[Union[str, None]] = None,
             preferred_bank: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Split a dedicated virtual account transaction with one or more accounts
 
         :param: customer_id_or_code: Customer's ID or Code
         :param: subaccount: Subaccount code of the account you want to split the transaction
         :param: split_code: Split code
         :param: preferred_bank: Preferred bank for the virtual account
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
         }
         return self._post_request("/dedicated_account/split", data=data)
 
-    def remove_split_dedicated_account(self, account_number: str) -> Response:
+    def remove_split_dedicated_account(self, account_number: str) -> PayStackResponse:
         """
         Remove a split dedicated virtual account
 
         :param: account_number: the account number of the dedicated virtual account
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "account_number": account_number,
         }
         return self._delete_request("/dedicated_account/split", data=data)
 
-    def fetch_bank_providers(self) -> Response:
+    def fetch_bank_providers(self) -> PayStackResponse:
         """
         Fetch bank providers
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request("/dedicated_account/available_providers")
```

### Comparing `paystackease-1.0.0/paystackease/apis/disputes.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/disputes.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,47 +2,47 @@
 Wrapper for Paystack Disputes API
 
 The Disputes API allows you manage transaction disputes on your integration.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import DisputeStatus, Resolution
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import DisputeStatus, Resolution
 
-class DisputesClientAPI(PayStackBaseClientAPI):
+
+class DisputesClientAPI(SyncRequestAPI):
     """
     Paystack Disputes API
     Reference: https://paystack.com/docs/api/dispute/
     """
 
     def list_disputes(
             self,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             transaction_id: Optional[Union[str, None]] = None,
             status: Optional[Union[DisputeStatus, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List disputes filed against you
 
         :param: from_date: A timestamp from which to start listing dispute e.g. 2016-09-21
         :param: to_date: A timestamp from which to start listing dispute e.g. 2016-09-21
         :param: per_page:
         :param: page:
         :param: transaction_id:
         :param: status: Dispute Status. Acceptable values:
                         { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -51,79 +51,79 @@
             "from": from_date,
             "to": to_date,
             "transaction": transaction_id,
             "status": status,
         }
         return self._get_request("/dispute", params=params)
 
-    def fetch_dispute(self, dispute_id: str) -> Response:
+    def fetch_dispute(self, dispute_id: str) -> PayStackResponse:
         """
         Fetch details about a dispute
 
         :param: dispute_id: The dispute ID to fetch
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/dispute/{dispute_id}")
 
-    def list_transaction_disputes(self, transaction_id: str) -> Response:
+    def list_transaction_disputes(self, transaction_id: str) -> PayStackResponse:
         """
         List disputes for a transaction
 
         :param: transaction_id: The transaction id to fetch
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/dispute/transaction/{transaction_id}")
 
     def update_dispute(
             self,
             dispute_id: str,
             refund_amount: int,
             uploaded_filename: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update details of a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: refund_amount: The amount to refund to the customer
         :param: uploaded_filename: filename of attachment returned via
-                                    response from upload url(GET /dispute/:id/upload_url)
+                                    PayStackResponse from upload url(GET /dispute/:id/upload_url)
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"refund_amount": refund_amount, "uploaded_filename": uploaded_filename}
         return self._put_request(f"/dispute/{dispute_id}", data=data)
 
     def add_evidence(
             self,
             dispute_id: str,
             customer_email: str,
             customer_name: str,
             customer_phone: str,
             service_details: str,
             delivery_address: Optional[Union[str, None]] = None,
             delivery_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Add evidence to a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: customer_email: The customer email
         :param: customer_name: The customer name
         :param: customer_phone: The customer phone
         :param: service_details: The service details
         :param: delivery_address: The delivery address
         :param: delivery_date: The delivery date: YYYY-MM-DD
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         delivery_date = self._convert_to_string(delivery_date)
 
         data = {
             "customer_email": customer_email,
@@ -131,48 +131,48 @@
             "customer_phone": customer_phone,
             "service_details": service_details,
             "delivery_address": delivery_address,
             "delivery_date": delivery_date,
         }
         return self._post_request(f"/dispute/{dispute_id}/evidence", data=data)
 
-    def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> Response:
+    def get_upload_url(self, dispute_id: str, uploaded_filename: str) -> PayStackResponse:
         """
         Get upload url for dispute evidence
 
         :param: dispute_id: The dispute id to fetch
         :param: uploaded_filename: The file name, with its extension, that you want to upload. e.g. filename.pdf
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {"uploaded_filename": uploaded_filename}
         return self._get_request(f"/dispute/{dispute_id}/upload_url", params=params)
 
     def resolve_dispute(
             self,
             dispute_id: str,
             resolution: Resolution,
             message: str,
             refund_amount: int,
             uploaded_filename: str,
             evidence: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Resolve a dispute
 
         :param: dispute_id: The dispute id to fetch
         :param: resolution: The resolution to resolve the dispute: Accepted values: { merchant-accepted | declined }.
         :param: message: The message for resolution
         :param: refund_amount: The amount to refund to the customer
-        :param: uploaded_filename: filename of attachment returned via response from method get_upload_url
+        :param: uploaded_filename: filename of attachment returned via PayStackResponse from method get_upload_url
         :param: evidence: The evidence id for fraud claims
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "resolution": resolution,
             "message": message,
             "refund_amount": refund_amount,
             "uploaded_filename": uploaded_filename,
             "evidence": evidence,
@@ -183,28 +183,28 @@
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
             transaction_id: Optional[Union[str, None]] = None,
             status: Optional[Union[DisputeStatus, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Export disputes
 
         :param: per_page:
         :param: page:
         :param: from_date: The start date to fetch disputes from
         :param: to_date: The end date to fetch disputes from
         :param: transaction_id: The transaction ID
         :param: status: The dispute status:
                         Acceptable values: { awaiting-merchant-feedback | awaiting-bank-feedback | pending | resolved }
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
```

### Comparing `paystackease-1.0.0/paystackease/apis/integration.py` & `paystackease-2.0.0/paystackease/apis/async_apis/aintegration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 """
-Wrapper for Paystack Integration API
+Wrapper for Asynchronous Paystack Integration API
 
 The Integration API allows you manage some settings on your integration.
 """
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
+from paystackease.core import AsyncRequestAPI, PayStackResponse
 
 
-class IntegrationClientAPI(PayStackBaseClientAPI):
+class AsyncIntegrationClientAPI(AsyncRequestAPI):
     """
     Paystack Integration API
     Reference: https://paystack.com/docs/api/integration/
     """
 
-    def fetch_timeout(self) -> Response:
+    async def fetch_timeout(self) -> PayStackResponse:
         """
         Fetch payment session timeout
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request("/integration/payment_session_timeout")
+        return await self._get_request("/integration/payment_session_timeout")
 
-    def update_timeout(self, timeout: int) -> Response:
+    async def update_timeout(self, timeout: int) -> PayStackResponse:
         """
         Update payment session timeout
 
         :param: timeout: The new payment session timeout before session
-        
+
         note::
 
             timeout is in seconds. Set 0 to cancel the timeout
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         data = {"timeout": timeout}
-        return self._put_request("/integration/payment_session_timeout", data=data)
+        return await self._put_request("/integration/payment_session_timeout", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/apis/miscellaneous.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/miscellaneous.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Wrapper for Paystack Miscellaneous API.
 
 The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
 """
 
 from typing import Optional, Union
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import GateWay, Channels, Currency
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import GateWay, Channels, Currency
 
-class MiscellaneousClientAPI(PayStackBaseClientAPI):
+
+class MiscellaneousClientAPI(SyncRequestAPI):
     """
     Paystack Miscellaneous API
     Reference: https://paystack.com/docs/api/miscellaneous/
     """
 
     def list_banks(
             self,
@@ -25,15 +25,15 @@
             pay_with_bank: Optional[Union[bool, None]] = False,
             enabled_for_verification: Optional[Union[bool, None]] = False,
             next_cursor: Optional[Union[str, None]] = None,
             previous_cursor: Optional[Union[str, None]] = None,
             gateway: Optional[Union[GateWay, None]] = None,
             channel_type: Optional[Union[Channels, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Get a list of all supported banks and their properties
 
         :param: country: The country to obtain the list of supported banks.
                         Values { country=ghana or country=nigeria }
         :param: use_cursor: Use cursor to paginate through the list of supported banks
         :param: per_page: The number of records to return per page: 10, 20 or 50
@@ -48,16 +48,16 @@
         :param: currency: filter for banks that support a specific currency
         :param: channel_type: Type of financial channel. { Channels.value.value}
 
         **note::**
 
         For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert to strings
         use_cursor = self._convert_to_string(use_cursor)
         pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
         pay_with_bank = self._convert_to_string(pay_with_bank)
         enabled_for_verification = self._convert_to_string(enabled_for_verification)
 
@@ -72,27 +72,27 @@
             "previous": previous_cursor,
             "gateway": gateway,
             "type": channel_type,
             "currency": currency,
         }
         return self._get_request("/bank", params=params)
 
-    def list_countries(self) -> Response:
+    def list_countries(self) -> PayStackResponse:
         """
         Get a list of all supported countries and their properties
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request("/country")
 
-    def list_states(self, country: str) -> Response:
+    def list_states(self, country: str) -> PayStackResponse:
         """
         Get a list of all supported states and their properties
 
         :param: country: The country code from which to obtain the list of supported states
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {"country": country}
         return self._get_request("/address_verification/states", params=params)
```

### Comparing `paystackease-1.0.0/paystackease/apis/payment_pages.py` & `paystackease-2.0.0/paystackease/apis/async_apis/apayment_pages.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,157 +1,157 @@
 """
-Wrapper for Paystack Payment Pages API.
+Wrapper for Asynchronous Paystack Payment Pages API.
 
 The Payment Pages API provides a quick and secure way to collect payment for products.
 """
 
 from datetime import date
 from typing import Optional, Dict, List, Any, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
 
-class PaymentPagesClientAPI(PayStackBaseClientAPI):
+
+class AsyncPaymentPagesClientAPI(AsyncRequestAPI):
     """
     Paystack Payment Pages API
     Reference: https://paystack.com/docs/api/page/
     """
 
-    def create_payment_page(
+    async def create_payment_page(
             self,
             name: str,
             description: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             split_code: Optional[Union[str, None]] = None,
             page_slug: Optional[Union[str, None]] = None,
             redirect_url: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, Any], None]] = None,
             custom_fields: Optional[Union[List[Dict[str, Any]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a payment page
 
         :param: name: Name of the page
         :param: description: Description of the page
         :param: amount: Amount of the page
         :param: split_code: Split code of the transaction split
         :param: page_slug: URL slug you would like to be associated with this page.
-        
+
         note::
 
             Page will be accessible at https://paystack.com/pay/page_slug
 
         :param: redirect_url: If you would like Paystack to redirect someplace
                                 upon successful payment, specify the URL here.
         :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
         :param: custom_fields: If you would like to accept custom fields, specify them here.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "name": name,
             "description": description,
             "amount": amount,
             "split_code": split_code,
             "slug": page_slug,
             "redirect_url": redirect_url,
             "metadata": metadata,
             "custom_fields": custom_fields,
         }
-        return self._post_request("/page", data=data)
+        return await self._post_request("/page", data=data)
 
-    def list_payment_pages(
+    async def list_payment_pages(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the payment pages
 
         :param: per_page: Number of records to return
         :param: page: number to return
         :param: from_date: A timestamp from which to start listing page
         :param: to_date: A timestamp from which to start listing page
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
 
         note::
             Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/page", params=params)
+        return await self._get_request("/page", params=params)
 
-    def fetch_payment_page(self, page_id_or_slug: str) -> Response:
+    async def fetch_payment_page(self, page_id_or_slug: str) -> PayStackResponse:
         """
         Get details of a payment page
 
         :param: page_id_or_slug: ID or slug of the payment page
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/page/{page_id_or_slug}")
+        return await self._get_request(f"/page/{page_id_or_slug}")
 
-    def update_payment_page(
+    async def update_payment_page(
             self,
             page_id_or_slug: str,
             name: Optional[Union[str, None]] = None,
             description: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             active: Optional[Union[bool, None]] = True,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a payment page detail
 
         :param: page_id_or_slug: ID or slug of the payment page
         :param: name: Name of the page
         :param: description: Description of the page
         :param: amount: Amount of the page
         :param: active: Set false to deactivate the page url
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "name": name,
             "description": description,
             "amount": amount,
             "active": active,
         }
-        return self._put_request(f"/page/{page_id_or_slug}", data=data)
+        return await self._put_request(f"/page/{page_id_or_slug}", data=data)
 
-    def check_slug_available(self, page_slug: str) -> Response:
+    async def check_slug_available(self, page_slug: str) -> PayStackResponse:
         """
         Check if a slug is available
 
         :param: page_slug: URL slug you would like to be associated with this page.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/page/check_slug_availability/{page_slug}")
+        return await self._get_request(f"/page/check_slug_availability/{page_slug}")
 
-    def add_products(self, payment_id: int, product: List[int]) -> Response:
+    async def add_products(self, payment_id: int, product: List[int]) -> PayStackResponse:
         """
         Add products to a payment page
 
         :param: payment_id: ID of the payment page
         :param: product: List of IDS of all the products
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"product": product}
-        return self._post_request(f"/page/{payment_id}/product", data=data)
+        return await self._post_request(f"/page/{payment_id}/product", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/apis/payment_requests.py` & `paystackease-2.0.0/paystackease/apis/async_apis/apayment_requests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
-Wrapper for Paystack Payment Requests API.
+Wrapper for Asynchronous Paystack Payment Requests API.
 
 The Payment Requests API allows you manage requests for payment of goods and services.
 """
 
 from datetime import date
 from typing import Optional, List, Dict, Any, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
-from paystackease.helpers.tool_kit import PayMentRequestStatus, Currency
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import PayMentRequestStatus, Currency
 
-class PaymentRequestClientAPI(PayStackBaseClientAPI):
+
+class AsyncPaymentRequestClientAPI(AsyncRequestAPI):
     """
     Paystack Payment Request API
     Reference: https://paystack.com/docs/api/payment-request/
     """
 
-    def create_payment_request(
+    async def create_payment_request(
             self,
             customer: str,
             amount: int,
             draft: bool,
             has_invoice: bool,
             send_notification: bool,
             due_date: Optional[Union[date, None]] = None,
             description: Optional[Union[str, Any]] = None,
             line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
             tax: Optional[Union[List[Dict[str, Any]], None]] = None,
             currency: Optional[Union[Currency, Any]] = None,
             invoice_number: Optional[Union[int, Any]] = None,
             split_code: Optional[Union[str, Any]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a payment request for a transaction
 
         :param: customer: Customer ID of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
         :param: description: Description of the payment request
@@ -44,16 +44,16 @@
         :param: currency: Currency of the payment request
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: has_invoice: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request
         :param: split_code: split code of the transaction split
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
         draft = self._convert_to_string(draft)
         has_invoice = self._convert_to_string(has_invoice)
         send_notification = self._convert_to_string(send_notification)
 
@@ -67,41 +67,41 @@
             "currency": currency,
             "send_notification": send_notification,
             "draft": draft,
             "has_invoice": has_invoice,
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
-        return self._post_request("/paymentrequest", data=data)
+        return await self._post_request("/paymentrequest", data=data)
 
-    def list_payment_requests(
+    async def list_payment_requests(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[str, None]] = None,
             status: Optional[Union[PayMentRequestStatus, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             include_archive: Optional[Union[bool, None]] = True,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the payment requests
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: customer: Filter by customer ID
         :param: status: Filter by payment request status
         :param: currency:
         :param: include_archive: Show archived payment requests
         :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
         :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
         include_archive = self._convert_to_string(include_archive)
 
@@ -111,89 +111,89 @@
             "customer": customer,
             "status": status,
             "currency": currency,
             "include_archive": include_archive,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/paymentrequest", params=params)
+        return await self._get_request("/paymentrequest", params=params)
 
-    def fetch_payment_request(self, id_or_code: str) -> Response:
+    async def fetch_payment_request(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a payment request on your integration
 
         :param: id_or_code: ID or Code of the payment request
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/paymentrequest/{id_or_code}")
+        return await self._get_request(f"/paymentrequest/{id_or_code}")
 
-    def verify_payment_request(self, code: str) -> Response:
+    async def verify_payment_request(self, code: str) -> PayStackResponse:
         """
         Verify details of a payment request on your integration
 
         :param: code: Payment request code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/paymentrequest/verify/{code}")
+        return await self._get_request(f"/paymentrequest/verify/{code}")
 
-    def send_notification(self, code: str) -> Response:
+    async def send_notification(self, code: str) -> PayStackResponse:
         """
         Send notification of a payment request to a customer
 
         :param: code: Payment request code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._post_request(f"/paymentrequest/notify/{code}")
+        return await self._post_request(f"/paymentrequest/notify/{code}")
 
-    def payment_request_total(self) -> Response:
+    async def payment_request_total(self) -> PayStackResponse:
         """
         Get total of a payment request metric
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request("/paymentrequest/totals")
+        return await self._get_request("/paymentrequest/totals")
 
-    def finalize_payment_request(self, code: str, send_notification: bool) -> Response:
+    async def finalize_payment_request(self, code: str, send_notification: bool) -> PayStackResponse:
         """
         Finalize a draft payment request
 
         :param: code: Payment request code
         :param: send_notification: Set true if you want to send a notification to the customer email
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert to strings
         send_notification = self._convert_to_string(send_notification)
 
         data = {"send_notification": send_notification}
-        return self._post_request(f"/paymentrequest/finalize/{code}", data=data)
+        return await self._post_request(f"/paymentrequest/finalize/{code}", data=data)
 
-    def update_payment_request(
+    async def update_payment_request(
             self,
             id_or_code: str,
             customer: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             description: Optional[Union[str, None]] = None,
             line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
             tax: Optional[Union[List[Dict[str, Any]], None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             due_date: Optional[Union[date, None]] = None,
             send_notification: Optional[Union[bool, None]] = True,
             draft: Optional[Union[bool, None]] = True,
             invoice_number: Optional[Union[int, None]] = None,
             split_code: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a payment request
 
         :param: id_or_code: ID or Code of the payment request
         :param: customer: Customer ID or code of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
@@ -202,16 +202,16 @@
         :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
         :param: currency: Currency of the payment request
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
         :param: split_code: split code of the transaction split
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
         draft = self._convert_to_string(draft)
         send_notification = self._convert_to_string(send_notification)
 
@@ -224,19 +224,19 @@
             "tax": tax,
             "currency": currency,
             "send_notification": send_notification,
             "draft": draft,
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
-        return self._put_request(f"/paymentrequest/{id_or_code}", data=data)
+        return await self._put_request(f"/paymentrequest/{id_or_code}", data=data)
 
-    def archive_payment_request(self, code: str) -> Response:
+    async def archive_payment_request(self, code: str) -> PayStackResponse:
         """
         Archive a payment request
 
         :param: code: Payment request code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._post_request(f"/paymentrequest/archive/{code}")
+        return await self._post_request(f"/paymentrequest/archive/{code}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/plans.py` & `paystackease-2.0.0/paystackease/apis/async_apis/aplans.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 """
-Wrapper for Paystack Plans API
+Wrapper for Asynchronous Paystack Plans API
 
 The Plans API allows you to create and manage installment payment options on your integration.
 """
 
 from typing import Optional, Union
-from paystackease.helpers.tool_kit import Interval
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Interval
 
-class PlanClientAPI(PayStackBaseClientAPI):
+
+class AsyncPlanClientAPI(AsyncRequestAPI):
     """
     Paystack Plan API
     Reference: https://paystack.com/docs/api/plan/
     """
 
-    def create_plan(
+    async def create_plan(
             self,
             name: str,
             amount: int,
             interval: Interval,
             currency: str,
             invoice_limit: int,
             send_invoices: bool,
             send_sms: bool,
             description: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a plan
 
         :param: name: Name of the plan
         :param: amount: Amount of the plan
         :param: interval: Interval of the plan. Values [Interval.value.value]
         :param: description: Description of the plan
         :param: send_invoices: Send invoices to customer
         :param: send_sms: Send SMS to customer
         :param: currency: Currency of the plan
         :param: invoice_limit: Invoice limit of the plan
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert to strings
         send_invoices = self._convert_to_string(send_invoices)
         send_sms = self._convert_to_string(send_sms)
 
         data = {
             "name": name,
@@ -52,83 +52,83 @@
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
             "currency": currency,
             "invoice_limit": invoice_limit,
         }
-        return self._post_request("/plan", data=data)
+        return await self._post_request("/plan", data=data)
 
-    def list_plans(
+    async def list_plans(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             status: Optional[Union[str, None]] = None,
             interval: Optional[Union[Interval, None]] = None,
             amount: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the plans
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: status: Filter list by plans with specified status
         :param: interval: Filter list by plans with specified interval
         :param: amount
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {
             "perPage": per_page,
             "page": page,
             "status": status,
             "interval": interval,
             "amount": amount,
         }
-        return self._get_request("/plan", params=params)
+        return await self._get_request("/plan", params=params)
 
-    def fetch_plan(self, id_or_code: str) -> Response:
+    async def fetch_plan(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a plan
 
         :param: id_or_code: ID or Code of the plan
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/plan/{id_or_code}")
+        return await self._get_request(f"/plan/{id_or_code}")
 
-    def update_plan(
+    async def update_plan(
             self,
             id_or_code: str,
             name: str,
             amount: int,
             interval: Interval,
             send_invoices: bool,
             send_sms: bool,
             currency: str,
             invoice_limit: int,
             description: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a plan detail
 
         :param: id_or_code: ID or Code of the plan
         :param: name: Name of the plan
         :param: amount: Amount of the plan
         :param: interval: Interval of the plan. [Interval.value.value]
         :param: description:
         :param: send_invoices:
         :param: send_sms:
         :param: currency:
         :param: invoice_limit:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert to strings
         send_invoices = self._convert_to_string(send_invoices)
         send_sms = self._convert_to_string(send_sms)
 
         data = {
             "name": name,
@@ -136,8 +136,8 @@
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
             "currency": currency,
             "invoice_limit": invoice_limit,
         }
-        return self._put_request(f"/plan/{id_or_code}", data=data)
+        return await self._put_request(f"/plan/{id_or_code}", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/apis/products.py` & `paystackease-2.0.0/paystackease/apis/async_apis/aproducts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 """
-Wrapper for Paystack Products API
+Wrapper for Asynchronous Paystack Products API
 
 The Products API allows you to create and manage inventories on your integration.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
 
-class ProductClientAPI(PayStackBaseClientAPI):
+
+class AsyncProductClientAPI(AsyncRequestAPI):
     """
     Paystack Product API
     Reference: https://paystack.com/docs/api/product/
     """
 
-    def create_product(
+    async def create_product(
             self,
             name: str,
             description: str,
             amount: int,
             currency: str,
             unlimited: Optional[Union[bool, None]] = True,
             quantity: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a product
 
         :param: name: Name of the product
         :param: description: Description of the product
         :param: amount: Price of the product
         :param: currency: Currency of the product
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         unlimited = self._convert_to_string(unlimited)
 
         data = {
             "name": name,
             "description": description,
             "price": amount,
             "currency": currency,
             "unlimited": unlimited,
             "quantity": quantity,
         }
-        return self._post_request("/product", data=data)
+        return await self._post_request("/product", data=data)
 
-    def list_products(
+    async def list_products(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the products
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: from_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date: A timestamp from which to start listing product e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to strings
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/product", params=params)
+        return await self._get_request("/product", params=params)
 
-    def fetch_product(self, product_id: str) -> Response:
+    async def fetch_product(self, product_id: str) -> PayStackResponse:
         """
         Get details of a product
 
         :param: product_id: ID or Code of the product
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/product/{product_id}")
+        return await self._get_request(f"/product/{product_id}")
 
-    def update_product(
+    async def update_product(
             self,
             product_id: str,
             name: str,
             description: str,
             amount: int,
             currency: str,
             unlimited: Optional[Union[bool, None]] = True,
             quantity: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a product detail
 
         :param: product_id: ID or Code of the product
         :param: name: Name of the product
         :param: description: Description of the product
         :param: amount: Price of the product
         :param: currency: Currency of the product
         :param: unlimited: Set true if the product has unlimited stock,
         :param: quantity: Quantity of the product in stock Use if unlimited is false
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         unlimited = self._convert_to_string(unlimited)
 
         data = {
             "name": name,
             "description": description,
             "price": amount,
             "currency": currency,
             "unlimited": unlimited,
             "quantity": quantity,
         }
-        return self._put_request(f"/product/{product_id}", data=data)
+        return await self._put_request(f"/product/{product_id}", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/apis/refund.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/refund.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 Wrapper for Paystack Refund API
 
 The Refunds API allows you to create and manage transaction refunds.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
-from paystackease.helpers.tool_kit import Currency
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
 
-class RefundClientAPI(PayStackBaseClientAPI):
+
+class RefundClientAPI(SyncRequestAPI):
     """
     Paystack Refund API
     Reference: https://paystack.com/docs/api/refund/
     """
 
     def create_refund(
             self,
             transaction_ref_or_id: str,
             amount: Optional[Union[int, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             customer_note: Optional[Union[str, None]] = None,
             merchant_note: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a refund
 
         :param: transaction_ref_or_id: The transaction id or reference to fetch
         :param: amount: The amount to refund
         :param: currency: The currency to refund { Currency.value.value }
         :param: customer_note: The customer note or reason
         :param: merchant_note: The merchant note or reason
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "transaction": transaction_ref_or_id,
             "amount": amount,
             "currency": currency,
             "customer_note": customer_note,
             "merchant_note": merchant_note,
@@ -50,27 +50,27 @@
             self,
             reference: Optional[Union[str, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List refunds
 
         :param: reference: The transaction reference to fetch for the refund
         :param: currency: The currency to refund
         :param: per_page
         :param: page
         :param: from_date: A timestamp at which to stop listing refund
         :param: to_date: A timestamp at which to stop listing refund
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
 
         note::
 
             Date time format: 2016-09-21
         """
 
         # convert date to string
@@ -83,17 +83,17 @@
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
         return self._get_request("/refund", params=params)
 
-    def fetch_refund(self, reference: str) -> Response:
+    def fetch_refund(self, reference: str) -> PayStackResponse:
         """
         Fetch a refund
 
         :param: reference: The transaction reference to fetch for the refund
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/refund/{reference}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/settlements.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/settlements.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 Wrapper for Paystack Settlements API
 
 The Settlements API allows you to gain insights into payouts made by Paystack to your bank account.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
-from paystackease.helpers.tool_kit import STATUS
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import STATUS
 
-class SettlementClientAPI(PayStackBaseClientAPI):
+
+class SettlementClientAPI(SyncRequestAPI):
     """
     Paystack Settlement API
     Reference: https://paystack.com/docs/api/settlement/
     """
 
     def list_settlements(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             status: Optional[Union[STATUS, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List settlements made to your settlement accounts
 
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: status: Value can be one of success, processing, pending or failed.
         :param: subaccount:
         :param: from_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -57,26 +57,26 @@
     def list_settlement_transactions(
             self,
             settlement_id: int,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Get the transactions that make up a particular settlement
 
         :param: settlement_id: The id of the settlement.
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: from_date: A timestamp from which to start listing settlements
         :param: to_date: A timestamp from which to start listing settlements
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         
         note::
 
             Date and time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
         """
```

### Comparing `paystackease-1.0.0/paystackease/apis/subaccounts.py` & `paystackease-2.0.0/paystackease/apis/async_apis/asubaccounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 """
-Wrapper for Paystack SubAccounts API
+Wrapper for Asynchronous Paystack SubAccounts API
 
 The Subaccounts API allows you to create and manage subaccounts on your integration.
 Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
 """
 
 from datetime import date
 from typing import Optional, Dict, List, Any, Union
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import SettlementSchedule
-from paystackease._base import PayStackBaseClientAPI
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import SettlementSchedule
 
-class SubAccountClientAPI(PayStackBaseClientAPI):
+
+class AsyncSubAccountClientAPI(AsyncRequestAPI):
     """
     Paystack SubAccount API
     Reference: https://paystack.com/docs/api/subaccount/
     """
 
-    def create_subaccount(
+    async def create_subaccount(
             self,
             business_name: str,
             settlement_bank: str,
             account_number: str,
             percentage_charge: float,
             description: str,
             primary_contact_email: Optional[Union[str, None]] = None,
             primary_contact_name: Optional[Union[str, None]] = None,
             primary_contact_phone: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a subaccount
 
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: Bank Code for the bank
         :param: account_number: The account number of the subaccount.
         :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
         :param: description: The description of the subaccount.
         :param: primary_contact_email: A contact email for the subaccount
         :param: primary_contact_name: A name for the contact person for this subaccount
         :param: primary_contact_phone: A phone number to call for this subaccount
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "business_name": business_name,
             "settlement_bank": settlement_bank,
             "account_number": account_number,
             "percentage_charge": percentage_charge,
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "metadata": metadata,
         }
-        return self._post_request("/subaccount", data=data)
+        return await self._post_request("/subaccount", data=data)
 
-    def update_subaccount(
+    async def update_subaccount(
             self,
             id_or_code: str,
             business_name: str,
             settlement_bank: str,
             account_number: str,
             active: Optional[Union[bool, None]] = True,
             percentage_charge: Optional[Union[float, None]] = None,
             description: Optional[Union[str, None]] = None,
             primary_contact_email: Optional[Union[str, None]] = None,
             primary_contact_name: Optional[Union[str, None]] = None,
             primary_contact_phone: Optional[Union[str, None]] = None,
             settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
             metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a subaccount
 
         :param: id_or_code: The id or code of the subaccount.
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: The settlement bank of the subaccount.
         :param: account_number
@@ -87,20 +87,20 @@
         :param: primary_contact_email
         :param: primary_contact_name
         :param: primary_contact_phone
         :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
 
         note::
             Auto means payout is T+1
-            Manual means payout to the subaccount should only be made when requested. Defaults to auto
+            Manual means payout to the subaccount should only be made when requested. async defaults to auto
 
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "business_name": business_name,
@@ -111,45 +111,45 @@
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "settlement_schedule": settlement_schedule,
             "metadata": metadata,
         }
-        return self._put_request(f"/subaccount/{id_or_code}", data=data)
+        return await self._put_request(f"/subaccount/{id_or_code}", data=data)
 
-    def list_subaccounts(
+    async def list_subaccounts(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all subaccounts
 
         :param: per_page: The number of records to return per page.
         :param: page: The number to retrieve.
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return self._get_request("/subaccount", params=params)
+        return await self._get_request("/subaccount", params=params)
 
-    def fetch_subaccount(self, id_or_code: str) -> Response:
+    async def fetch_subaccount(self, id_or_code: str) -> PayStackResponse:
         """
         Fetch details of a specific subaccount
 
         :param: id_or_code: The id or code of the subaccount.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/subaccount/{id_or_code}")
+        return await self._get_request(f"/subaccount/{id_or_code}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/subscriptions.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/subscriptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 Wrapper for Paystack Subscriptions API
 
 The Subscriptions API allows you to create and manage recurring payment on your integration.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
 
-class SubscriptionClientAPI(PayStackBaseClientAPI):
+
+class SubscriptionClientAPI(SyncRequestAPI):
     """
     Paystack Subscription API
     Reference: https://paystack.com/docs/api/subscription/
     """
 
     def create_subscription(
             self,
             customer: str,
             plan_code: str,
             authorization: str,
             start_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a subscription
 
         :param: customer: Email or Code of the customer
         :param: plan_code: Code of the plan
         :param: authorization: Code of the authorization
         :param: start_date: Start date of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         start_date = self._convert_to_string(start_date)
 
         data = {
             "customer": customer,
@@ -48,85 +48,85 @@
 
     def list_subscriptions(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[int, None]] = None,
             plan_code: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the subscriptions
 
         :param: per_page: Number of records to return per page.
         :param: page: THe number to return
         :param: customer:
         :param: plan_code:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {
             "perPage": per_page,
             "page": page,
             "customer": customer,
             "plan": plan_code,
         }
         return self._get_request("/subscription", params=params)
 
-    def fetch_subscription(self, id_or_code: str) -> Response:
+    def fetch_subscription(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a subscription
 
         :param: id_or_code: ID or Code of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/subscription/{id_or_code}")
 
-    def enable_subscription(self, subscription_code: str, token: str) -> Response:
+    def enable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
         """
         Enable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"code": subscription_code, "token": token}
         return self._post_request("/subscription/enable", data=data)
 
-    def disable_subscription(self, subscription_code: str, token: str) -> Response:
+    def disable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
         """
         Disable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"code": subscription_code, "token": token}
         return self._post_request("/subscription/disable", data=data)
 
-    def generate_update_subscription(self, subscription_code: str) -> Response:
+    def generate_update_subscription(self, subscription_code: str) -> PayStackResponse:
         """
         Generate a link for updating the card on subscription
 
         :param: subscription_code: Code of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._post_request(f"/subscription/{subscription_code}/manage/link")
 
-    def send_update_subscription_link(self, subscription_code: str) -> Response:
+    def send_update_subscription_link(self, subscription_code: str) -> PayStackResponse:
         """
         Email a customer a link for updating the card on their subscription
 
         :param: subscription_code: Code of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._post_request(f"/subscription/{subscription_code}/manage/email")
```

### Comparing `paystackease-1.0.0/paystackease/apis/terminal.py` & `paystackease-2.0.0/paystackease/apis/async_apis/aterminal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,139 +1,138 @@
 """
-Wrapper for Paystack Terminal APIs
+Wrapper for Asynchronous Paystack Terminal APIs
 
 The Terminal API allows you to build delightful in-person payment experiences.
 """
 
 from typing import Optional, Dict, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
-from paystackease.helpers.tool_kit import EventAction, EventType
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import EventAction, EventType
 
-class TerminalClientAPI(PayStackBaseClientAPI):
+
+class AsyncTerminalClientAPI(AsyncRequestAPI):
     """
     Paystack Terminal API
     Reference: https://paystack.com/docs/api/terminal/
     """
 
-    def send_event(
+    async def send_event(
             self,
             terminal_id: str,
             event_type: EventType,
             terminal_action: EventAction,
             data_object: Dict[str, str],
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Send an event from your application to the Paystack Terminal
 
         :param: terminal_id: The terminal iD the event is sent to
         :param: event_type: The type of event to send. We currently support [ invoice | transaction ]
         :param: terminal_action: The action to perform on the terminal
-                                    [invoice type]:the action can either be [ process || view ]
-                                    [transaction type], the action can either be [ process || print ].
+                                [invoice type]:the action can either be [ process || view ]
+                                [transaction type], the action can either be [ process || print ].
         :param: data_object: parameters needed to perform the specified action.
                             [invoice type]: you need to pass {id: invoice_id, reference: offline_reference}.
                             [transaction type], you can pass {id: transaction_id}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"type": event_type, "action": terminal_action, "data": data_object}
-        return self._post_request(f"/terminal/{terminal_id}/event", data=data)
+        return await self._post_request(f"/terminal/{terminal_id}/event", data=data)
 
-    def commission_terminal(self, serial_number: str) -> Response:
+    async def commission_terminal(self, serial_number: str) -> PayStackResponse:
         """
         Activate debug device by linking it to your integration
 
         :param: serial_number: The serial number of the device
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"serial_number": serial_number}
-        return self._post_request("/terminal/commission_device", data=data)
+        return await self._post_request("/terminal/commission_device", data=data)
 
-    def decommission_terminal(self, serial_number: str) -> Response:
+    async def decommission_terminal(self, serial_number: str) -> PayStackResponse:
         """
         Deactivate debug device by unlinking it from your integration
 
         :param: serial_number: The serial number of the device
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"serial_number": serial_number}
-        return self._post_request("/terminal/decommission_device", data=data)
+        return await self._post_request("/terminal/decommission_device", data=data)
 
-    def update_terminal(
+    async def update_terminal(
             self, terminal_id: str, terminal_name: str, terminal_address: str
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update details of a terminal
 
         :param: terminal_id: The terminal iD the event is sent to
         :param: terminal_name: Name of the terminal
         :param: terminal_address: Address of the terminal
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"name": terminal_name, "address": terminal_address}
-        return self._put_request(f"/terminal/{terminal_id}", data=data)
+        return await self._put_request(f"/terminal/{terminal_id}", data=data)
 
-    def fetch_event_status(self, terminal_id: str, event_id: str) -> Response:
+    async def fetch_event_status(self, terminal_id: str, event_id: str) -> PayStackResponse:
         """
         Fetch details of a specific event status sent to the terminal
 
         :param: terminal_id: iD of the terminal the event is sent to
         :param: event_id: The event id sent to the terminal
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/terminal/{terminal_id}/event/{event_id}")
+        return await self._get_request(f"/terminal/{terminal_id}/event/{event_id}")
 
-    def fetch_terminal_status(self, terminal_id: str) -> Response:
+    async def fetch_terminal_status(self, terminal_id: str) -> PayStackResponse:
         """
         Fetch the availability of a terminal before sending an event
 
         :param: terminal_id: The terminal iD the event is sent to
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/terminal/{terminal_id}/presence")
+        return await self._get_request(f"/terminal/{terminal_id}/presence")
 
-    def list_terminals(
+    async def list_terminals(
             self,
             per_page: int = 50,
             next_cursor: Optional[Union[bool, None]] = True,
             previous_cursor: Optional[Union[bool, None]] = True,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List the Terminals available on your integration
 
-        :param: per_page: The number of records to return. Default value is 50
+        :param: per_page: The number of records to return. async default value is 50
         :param: next_cursor:
         :param: previous_cursor:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        # convert to strings
+        # convert toi strings
         next_cursor = self._convert_to_string(next_cursor)
         previous_cursor = self._convert_to_string(previous_cursor)
-
         params = {"perPage": per_page, "next": next_cursor, "previous": previous_cursor}
-        return self._get_request("/terminal", params=params)
+        return await self._get_request("/terminal", params=params)
 
-    def fetch_terminal(self, terminal_id: str) -> Response:
+    async def fetch_terminal(self, terminal_id: str) -> PayStackResponse:
         """
         Get the details of a terminal
 
         :param: terminal_id: The terminal iD the event is sent to
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/terminal/timeline/{terminal_id}")
+        return await self._get_request(f"/terminal/timeline/{terminal_id}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/transaction_splits.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/transaction_splits.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,106 +3,107 @@
 
 The Transaction Splits API enables merchants split the settlement for a transaction
 across their payout account, and one or more subaccounts.
 """
 
 from datetime import date
 from typing import Optional, List, Dict, Any, Union
-from paystackease._utils import Response
-from paystackease._base import PayStackBaseClientAPI
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
 
-class TransactionSplitClientAPI(PayStackBaseClientAPI):
+
+class TransactionSplitClientAPI(SyncRequestAPI):
     """
     Paystack Transaction Split API
     Reference: https://paystack.com/docs/api/split/
     """
 
     def create_split(
             self,
             transaction_split_name: str,
             transaction_split_type: str,
-            currency: str,
+            currency: Currency,
             subaccounts: List[Dict[str, Any]],
             bearer_type: str,
             bearer_subaccount: str,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a split payment on your integration
 
         :param: transaction_split_name: Name of the transaction split
         :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
         :param: currency: [ Currency.value.value ]
         :param: subaccounts: A list of object containing subaccount code and number of shares
                             [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
         :param: bearer_type: Any of subaccount | account | all-proportional | all
         :param: bearer_subaccount: Subaccount code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "name": transaction_split_name,
             "type": transaction_split_type,
             "currency": currency,
             "subaccounts": subaccounts,
             "bearer_type": bearer_type,
             "bearer_subaccount": bearer_subaccount,
         }
         return self._post_request("/split", data=data)
 
     def add_or_update_subaccount_split(
             self, split_id: str, subaccount: str, transaction_share: int
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Add a Subaccount to a Transaction Split, or update the share of
         an existing Subaccount in a Transaction Split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
         :param: transaction_share: The number of shares
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"subaccount": subaccount, "share": transaction_share}
         return self._post_request(f"/split/{split_id}/subaccount/add", data=data)
 
-    def remove_sub_account_split(self, split_id: str, subaccount: str) -> Response:
+    def remove_sub_account_split(self, split_id: str, subaccount: str) -> PayStackResponse:
         """
         Remove a Sub Account from a transaction split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"subaccount": subaccount}
         return self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
 
     def update_split(
             self,
             split_id: str,
             transaction_split_name: str,
             active: bool,
             bearer_type: Optional[Union[str, None]] = None,
             bearer_subaccount: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a specific transaction split details
 
         :param: split_id: The split ID
         :param: transaction_split_name: Name of the transaction split
         :param: active: True or False
         :param: bearer_type:
         :param: bearer_subaccount:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "name": transaction_split_name,
@@ -117,28 +118,28 @@
             split_name: Optional[Union[str, None]] = None,
             active: Optional[Union[bool, None]] = True,
             sort_by: Optional[Union[str, None]] = None,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the transaction splits
 
         :param: split_name: Name of the transaction split
         :param: active: True or False
         :param: sort_by: Sort by name, defaults to createdAt date,
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         active = self._convert_to_string(active)
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
@@ -149,17 +150,17 @@
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
         return self._get_request("/split", params=params)
 
-    def fetch_split(self, split_id: str) -> Response:
+    def fetch_split(self, split_id: str) -> PayStackResponse:
         """
         Fetch details of a specific transaction split
 
         :param: split_id: The split ID
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/split/{split_id}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/transactions.py` & `paystackease-2.0.0/paystackease/apis/async_apis/atransactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 """
-Wrapper for Paystack Transactions API
+Wrapper for Asynchronous Paystack Transactions API
 
 The Transactions API allows you to create and manage payments on your integration.
 """
 
 from datetime import date
 from typing import List, Optional, Dict, Any, Union
-from paystackease.helpers.tool_kit import Channels, Currency, Bearer, TransactionStatus
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import TransactionStatus, Channels, Bearer, Currency
 
-class TransactionClientAPI(PayStackBaseClientAPI):
+
+class AsyncTransactionClientAPI(AsyncRequestAPI):
     """
     Paystack Transaction API
     Reference: https://paystack.com/docs/api/transaction/
     """
 
-    def initialize(
+    async def initialize(
             self,
             email: str,
             amount: int,
             currency: Optional[Union[Currency, None]] = Currency.NGN.value,
             reference: Optional[Union[str, None]] = None,
             callback_url: Optional[Union[str, None]] = None,
             plan: Optional[Union[str, None]] = None,
             invoice_limit: Optional[Union[int, None]] = None,
             channels: Optional[Union[List[Channels], None]] = None,
             split_code: Optional[Union[str, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             transaction_charge: Optional[Union[int, None]] = None,
             bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
             metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Initialize a transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # Currency.value.value
         :param: reference:
         :param: callback_url: # Use this to override the callback url provided on the  dashboard
-                            # https://example.com/callback
-        :param: plan:  # If transaction is to create a subscription to a predefined plan, provide plan code here.
+                                # https://example.com/callback
+        :param: plan:  # If transaction is to create a subscription to a preasync defined plan, provide plan code here.
         :param: invoice_limit:  # Number of times to charge customer during subscription to plan
         :param: channels:  # [Channels.value.value, Channels.value.value, ...]
         :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
         :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge: # An amount used to override the split configuration for a
                                     # single split payment
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "callback_url": callback_url,
@@ -67,30 +67,30 @@
             "channels": channels,
             "split_code": split_code,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "metadata": metadata,
         }
-        return self._post_request("/transaction/initialize", data=data)
+        return await self._post_request("/transaction/initialize", data=data)
 
-    def charge_authorization(
+    async def charge_authorization(
             self,
             email: str,
             amount: int,
             authorization_code: str,
             reference: Optional[Union[str, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             channels: Optional[Union[List[Channels], None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             transaction_charge: Optional[int] = None,
             bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
             queue: Optional[Union[bool, None]] = True,
             metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Charge an authorization transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: authorization_code:  # value = AUTH_1234234WRFW
@@ -99,16 +99,16 @@
         :param: channels:  # [Channels.value.value, Channels.value.value, ...]
         :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge:
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: queue:  # If set to true, the transaction will be queued for processing
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         queue = self._convert_to_string(queue)
 
         data = {
             "email": email,
@@ -119,74 +119,74 @@
             "channels": channels,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "queue": queue,
             "metadata": metadata,
         }
-        return self._post_request("/transaction/charge_authorization", data=data)
+        return await self._post_request("/transaction/charge_authorization", data=data)
 
-    def partial_debit(
+    async def partial_debit(
             self,
             email: str,
             authorization_code: str,
             amount: int,
             currency: str,
             reference: Optional[Union[str, None]] = None,
             at_least: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Charge a partial debit transaction
 
         :param: email:
         :param: authorization_code:  # value = AUTH_1234234WRFW
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # value = Currency.value.value
         :param: reference:  # Unique transaction reference.
         :param: at_least:  # Minimum amount to charge
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "authorization_code": authorization_code,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "at_least": at_least,
         }
-        return self._post_request("/transaction/partial_debit", data=data)
+        return await self._post_request("/transaction/partial_debit", data=data)
 
-    def list_transactions(
+    async def list_transactions(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[int, None]] = None,
             terminal_id: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             status: Optional[Union[TransactionStatus, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all transactions
 
         :param: per_page:  # Specify how many records you want to retrieve per page.
         :param: page:  # Specify a page number to retrieve
         :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
         :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
         :param: amount:  # Specify an amount for the transactions you want to retrieve
         :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
         :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -195,94 +195,94 @@
             "customer": customer,
             "terminalid": terminal_id,
             "amount": amount,
             "status": status,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/transaction", params=params)
+        return await self._get_request("/transaction", params=params)
 
-    def verify_transaction(self, reference: str) -> Response:
+    async def verify_transaction(self, reference: str) -> PayStackResponse:
         """
         Verify a transaction by reference
 
         :param: reference:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/transaction/verify/{reference}")
+        return await self._get_request(f"/transaction/verify/{reference}")
 
-    def fetch_transaction(self, transaction_id: int) -> Response:
+    async def fetch_transaction(self, transaction_id: int) -> PayStackResponse:
         """
         Fetch details of a specific transaction
 
         :param: transaction_id:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/transaction/{transaction_id}")
+        return await self._get_request(f"/transaction/{transaction_id}")
 
-    def transaction_timeline(self, id_or_reference: str) -> Response:
+    async def transaction_timeline(self, id_or_reference: str) -> PayStackResponse:
         """
         Get the timeline of a transaction
 
         :param: id_or_reference:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return self._get_request(f"/transaction/timeline/{id_or_reference}")
+        return await self._get_request(f"/transaction/timeline/{id_or_reference}")
 
-    def transaction_totals(
+    async def transaction_totals(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Get totals of all transactions
 
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/transaction/totals", params=params)
+        return await self._get_request("/transaction/totals", params=params)
 
-    def export_transactions(
+    async def export_transactions(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[int, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             amount: Optional[Union[int, None]] = None,
             status: Optional[Union[TransactionStatus, None]] = None,
             settled: Optional[Union[bool, None]] = True,
             settlement: Optional[Union[int, None]] = None,
             payment_page: Optional[Union[int, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Export transactions
 
         :param: per_page:
         :param: page:
         :param: customer:
         :param: currency:  # value = Currency.value.value
@@ -290,16 +290,16 @@
         :param: status:
         :param: settled:  # true or false
         :param: settlement:
         :param: payment_page:
         :param: from_date:  # 2016-09-24T00:00:05.000Z
         :param: to_date:  # 2016-09-24T00:00:05.000Z
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
         settled = self._convert_to_string(settled)
 
@@ -312,8 +312,8 @@
             "status": status,
             "settled": settled,
             "settlement": settlement,
             "payment_page": payment_page,
             "from": from_date,
             "to": to_date,
         }
-        return self._get_request("/transaction/export", params=params)
+        return await self._get_request("/transaction/export", params=params)
```

### Comparing `paystackease-1.0.0/paystackease/apis/transfer_recipients.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/transfer_recipients.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Wrapper for Paystack Transfer Recipient APIs
 
 The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
 """
 
 from datetime import date
 from typing import Optional, Dict, List, Any, Union
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import Currency
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
 
-class TransferRecipientsClientAPI(PayStackBaseClientAPI):
+
+class TransferRecipientsClientAPI(SyncRequestAPI):
     """
     Paystack Transfer Recipients API
     Reference: https://paystack.com/docs/api/transfer-recipient/
     """
 
     def create_transfer_recipients(
             self,
@@ -23,115 +23,115 @@
             recipient_name: str,
             account_number: str,
             bank_code: str,
             description: Optional[Union[str, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             authorization_code: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a transfer recipient
 
         :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
         :param: recipient_name: The name of the transfer recipient according to their account registration
         :param: account_number: transfer recipient's account number.
                                 Required for all recipient types except authorization
         :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
         :param: description:
         :param: currency: transfer recipient's currency. [Currency.value.value ]
         :param: authorization_code: transfer recipient's authorization code from previous transaction
         :param: metadata: transfer recipient's metadata
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "type": recipient_type,
             "name": recipient_name,
             "account_number": account_number,
             "bank_code": bank_code,
             "description": description,
             "currency": currency,
             "authorization_code": authorization_code,
             "metadata": metadata,
         }
         return self._post_request("/transferrecipient", data=data)
 
-    def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> Response:
+    def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> PayStackResponse:
         """
         Create multiple transfer recipients in batches.
 
         :param: batch: A list of transfer recipient object
                         keys [ { type, name, account_number, bank_code, currency etc. }]
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"batch": batch}
         return self._post_request("/transferrecipient/bulk", data=data)
 
     def list_transfer_recipients(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List transfer recipients
 
         :param: per_page: The number of records to return per page.
         :param: page: The page number to retrieve.
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to strings
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
         return self._get_request("/transferrecipient", params=params)
 
-    def fetch_transfer_recipient(self, id_or_code: str) -> Response:
+    def fetch_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
         """
         Fetch details of a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/transferrecipient/{id_or_code}")
 
     def update_transfer_recipient(
             self,
             id_or_code: str,
             recipient_name: str,
             recipient_email: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
         :param: recipient_name: The name of the transfer recipient
         :param: recipient_email: The email of the transfer recipient
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"name": recipient_name, "email": recipient_email}
         return self._put_request(f"/transferrecipient/{id_or_code}", data=data)
 
-    def delete_transfer_recipient(self, id_or_code: str) -> Response:
+    def delete_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
         """
         Delete a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._delete_request(f"/transferrecipient/{id_or_code}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/transfers.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/transfers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,105 +3,104 @@
 
 The Transfers API allows you to automate sending money to your customers.
 """
 
 from datetime import date
 from typing import Optional, List, Dict, Any, Union
 
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import Currency
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Currency
 
 
-class TransfersClientAPI(PayStackBaseClientAPI):
+class TransfersClientAPI(SyncRequestAPI):
     """
     Paystack Transfers API
     Reference: https://paystack.com/docs/api/transfer/
     """
 
     def initiate_transfer(
             self,
             transfer_source: str,
             amount: int,
             transfer_recipient: str,
             reason: Optional[Union[str, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             reference: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Initiate a transfer. Upgrade your business to a Registered Business to use
 
         :param: transfer_source: Where should we transfer from? Only balance for now
         :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
         :param: transfer_recipient: The code of the recipient
         :param: currency: The currency of the transfer
         :param: reason: The reason for the transfer
         :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
                             Only -,_ and alphanumeric characters allowed.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "source": transfer_source,
             "amount": amount,
             "recipient": transfer_recipient,
             "reason": reason,
             "currency": currency,
             "reference": reference,
         }
         return self._post_request("/transfer", data=data)
 
-    def finalize_transfer(self, transfer_code: str, otp: str) -> Response:
+    def finalize_transfer(self, transfer_code: str, otp: str) -> PayStackResponse:
         """
         Finalize an initiated transfer
 
         :param: transfer_code: The code of the transfer to finalize
         :param: otp: The OTP sent to the business phone to verify transfer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"transfer_code": transfer_code, "otp": otp}
         return self._post_request("/transfer/finalize_transfer", data=data)
 
     def initiate_bulk_transfer(
             self, transfer_source: str, transfers: List[Dict[str, Any]]
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Batch multiple transfers in a single request
 
         :param: transfer_source: Where should we transfer from? Only balance for now
         :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"source": transfer_source, "transfers": transfers}
         return self._post_request("/transfer/bulk", data=data)
 
     def list_transfers(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer_id: Optional[Union[str, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List transfers
 
         :param: per_page: The number of records to return per page.
         :param: page: The page number to retrieve.
         :param: customer_id
         :param: from_date
         :param: to_date
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -109,28 +108,28 @@
             "page": page,
             "customer": customer_id,
             "from": from_date,
             "to": to_date,
         }
         return self._get_request("/transfer", params=params)
 
-    def fetch_transfer(self, id_or_code: str) -> Response:
+    def fetch_transfer(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a transfer
 
         :param: id_or_code: The id or code of the transfer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/transfer/{id_or_code}")
 
-    def verify_transfer(self, reference: str) -> Response:
+    def verify_transfer(self, reference: str) -> PayStackResponse:
         """
         Verify a transfer
 
         :param: reference: The reference of the transfer to verify
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._post_request(f"/transfer/verify/{reference}")
```

### Comparing `paystackease-1.0.0/paystackease/apis/transfers_control.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/transfers_control.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 """
 Wrapper for Paystack Transfer Control APIs
 
 The Transfers Control API allows you manage settings of your transfers.
 """
 
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
+from paystackease.core import PayStackResponse, SyncRequestAPI
 
 
-class TransferControlClientAPI(PayStackBaseClientAPI):
+class TransferControlClientAPI(SyncRequestAPI):
     """
     Paystack Transfers Control API
     Reference: https://paystack.com/docs/api/transfer-control/
     """
 
-    def check_balance(self) -> Response:
+    def check_balance(self) -> PayStackResponse:
         """
         Get the available balance
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request("/balance")
 
-    def fetch_balance_ledger(self) -> Response:
+    def fetch_balance_ledger(self) -> PayStackResponse:
         """
         Fetch all pay-ins and pay-outs that occurred on your integration
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request("/balance/ledger")
 
-    def resend_otp(self, transfer_code: str, reason: str) -> Response:
+    def resend_otp(self, transfer_code: str, reason: str) -> PayStackResponse:
         """
         Generates a new OTP and sends to customer in the event
         they are having trouble receiving one.
 
         :param: transfer_code: The code of the transfer to finalize
         :param: reason: Either resend_otp or transfer as the value of this field
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"transfer_code": transfer_code, "reason": reason}
         return self._post_request("/transfer/resend_otp", data=data)
 
-    def disable_otp(self) -> Response:
+    def disable_otp(self) -> PayStackResponse:
         """
         This is used in the event that you want to be able to
          complete transfers programmatically without use of OTPs
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._post_request("/transfer/disable_otp")
 
-    def finalize_disable_otp(self, otp: str) -> Response:
+    def finalize_disable_otp(self, otp: str) -> PayStackResponse:
         """
         Finalize the request to disable OTP on your transfers.
 
         :param: otp: The OTP sent to the business phone to verify disabling of OTP
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"otp": otp}
         return self._post_request("/transfer/disable_otp_finalize", data=data)
 
-    def enable_otp(self) -> Response:
+    def enable_otp(self) -> PayStackResponse:
         """
         This is used in the event that you want to stop
         being able to complete transfers programmatically with use of OTPs
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._post_request("/transfer/enable_otp")
```

### Comparing `paystackease-1.0.0/paystackease/apis/verification.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/verification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 """
 Wrapper for Paystack Verification APIs
 
 The Verification API allows you to perform KYC processes.
 """
 
-from paystackease._base import PayStackBaseClientAPI
-from paystackease._utils import Response
+from paystackease.core import PayStackResponse, SyncRequestAPI
 
 
-class VerificationClientAPI(PayStackBaseClientAPI):
+class VerificationClientAPI(SyncRequestAPI):
     """
     Paystack Verification API
     Reference: https://paystack.com/docs/api/verification/
     """
 
-    def resolve_account(self, account_number: str, bank_code: str) -> Response:
+    def resolve_account(self, account_number: str, bank_code: str) -> PayStackResponse:
         """
         Confirm an account belongs to the right customer.
         This feature is available to business in Nigeria and Ghana.
 
         :param: account_number: The account number to verify
         :param: bank_code: The bank code to verify
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {"account_number": account_number, "bank_code": bank_code}
         return self._get_request("/bank/resolve", params=params)
 
     def validate_account(
             self,
             account_name: str,
             account_number: str,
             account_type: str,
             bank_code: str,
             country_code: str,
             document_type: str,
             document_number: str,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Confirm the authenticity of a customer's account number before sending money.
         This feature is only available to businesses in South Africa.
 
         :param: account_name: The account name to validate: first and last name
         :param: account_number: The account number to validate
         :param: account_type: The account type to validate: personal or business
         :param: bank_code: The bank code to validate
         :param: country_code: The country code to validate
         :param: document_type: The customer's mode of identity:
                                 identityNumber, passportNumber or businessRegistrationNumber
         :param: document_number: The customer's document number
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "account_name": account_name,
             "account_number": account_number,
             "account_type": account_type,
             "bank_code": bank_code,
             "country_code": country_code,
             "document_type": document_type,
             "document_number": document_number,
         }
         return self._post_request("/bank/validate", data=data)
 
-    def resolve_card_bin(self, bin_code: str) -> Response:
+    def resolve_card_bin(self, bin_code: str) -> PayStackResponse:
         """
         Resolve a card BIN
 
         :param: bin_code: First 6 characters of card
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return self._get_request(f"/decision/bin/{bin_code}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/aapple_pay.py` & `paystackease-2.0.0/paystackease/apis/async_apis/aapple_pay.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 """
 Wrapper class for Asynchronous Paystack Apple Pay API.
 
 The Apple Pay API allows you register your application's top-level domain or subdomain.
 """
 
 from typing import Optional, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
 
-class AsyncApplePayClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncApplePayClientAPI(AsyncRequestAPI):
     """
     Paystack Apple Pay API
     Reference: https://paystack.com/docs/api/apple-pay/
     """
 
-    async def register_domain(self, domain_name: str) -> Response:
+    async def register_domain(self, domain_name: str) -> PayStackResponse:
         """
         Register a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "domainName": domain_name,
         }
         return await self._post_request("/apple-pay/domain", data=data)
 
     async def list_domains(
         self,
             use_cursor: Optional[Union[bool, None]] = False,
             next_page: Optional[Union[int, None]] = None,
             previous_page: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all registered domains
 
         :param: use_cursor  # use cursor for pagination
         :param: next_page  # next page
         :param: previous_page  # previous page
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         use_cursor = self._convert_to_string(use_cursor)
 
         params = {
             "use_cursor": use_cursor,
             "next": next_page,
             "previous": previous_page,
         }
         return await self._get_request("/apple-pay/domain", params=params)
 
-    async def unregister_domain(self, domain_name: str) -> Response:
+    async def unregister_domain(self, domain_name: str) -> PayStackResponse:
         """
         Unregister a domain or subdomain for Apple Pay
 
         :param: domain_name  # domain name or subdomain
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "domainName": domain_name,
         }
         return await self._delete_request("/apple-pay/domain", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/abulk_charges.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/bulk_charges.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,96 @@
-"""
-Wrapper for Asynchronous Paystack Bulk Charges API.
+""" Wrapper for Paystack Bulk Charges API.
 
 The Bulk Charges API allows you to create and manage multiple recurring payments from your customers.
 """
 
 from datetime import date
-
 from typing import List, Dict, Optional, Any, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import STATUS
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import STATUS
 
 
-class AsyncBulkChargesClientAPI(AsyncPayStackBaseClientAPI):
+class BulkChargesClientAPI(SyncRequestAPI):
     """
     Paystack Bulk Charges API
     Reference: https://paystack.com/docs/api/bulk-charge/
     """
 
-    async def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> Response:
+    def initiate_bulk_charge(self, objects: List[Dict[str, Any]]) -> PayStackResponse:
         """
         Send an array of objects with authorization codes and amount
 
         :param: objects
 
         note::
 
             A list of dictionary with authorization codes, amount and reference as keys
-            [{"authorization_code": "123456", "amount": 1000, "reference": "123456" }]
+            [{"authorization": "123456", "amount": 1000, "reference": "123456" }]
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._post_request("/bulkcharge", data=objects)
+        return self._post_request("/bulkcharge", data=objects)
 
-    async def list_bulk_charge_batches(
+    def list_bulk_charge_batches(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all bulk charges
 
         :param: per_page
         :param: page
         :param: from_date
         :param: to_date
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/bulkcharge", params=params)
+        return self._get_request("/bulkcharge", params=params)
 
-    async def fetch_bulk_charge_batch(self, id_or_code: str) -> Response:
+    def fetch_bulk_charge_batch(self, id_or_code: str) -> PayStackResponse:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/bulkcharge/{id_or_code}")
+        return self._get_request(f"/bulkcharge/{id_or_code}")
 
-    async def fetch_charge_bulk_batch(
+    def fetch_charge_bulk_batch(
             self,
             id_or_code: str,
             status: Optional[Union[STATUS, None]] = None,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Fetch a bulk charge of a specific batch
 
         :param: id_or_code
         :param: status:  {STATUS.value.value}
         :param: per_page
         :param: page
@@ -100,45 +98,45 @@
         :param: to_date
 
         note::
 
             Date Time format: 2016-09-24T00:00:05.000Z, 2016-09-21
             status: STATUS.value.value
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # Convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "status": status,
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
+        return self._get_request(f"/bulkcharge/{id_or_code}/charges", params=params)
 
-    async def pause_bulk_charge_batch(self, batch_code: str) -> Response:
+    def pause_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
         """
         Pause a bulk charge of a specific batch
 
         :param: batch_code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/bulkcharge/pause/{batch_code}")
+        return self._get_request(f"/bulkcharge/pause/{batch_code}")
 
-    async def resume_bulk_charge_batch(self, batch_code: str) -> Response:
+    def resume_bulk_charge_batch(self, batch_code: str) -> PayStackResponse:
         """
         Resume a bulk charge of a specific batch
 
         :param: batch_code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/bulkcharge/resume/{batch_code}")
+        return self._get_request(f"/bulkcharge/resume/{batch_code}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/acharges.py` & `paystackease-2.0.0/paystackease/apis/async_apis/acharges.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 Wrapper for Asynchronous Paystack Charges API.
 
 The Charge API allows you to configure payment channel of your choice when initiating a payment.
 """
 
 from datetime import date
 from typing import Optional, Dict, Any, List, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import PWT
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import PWT
 
-class AsyncChargesClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncChargesClientAPI(AsyncRequestAPI):
     """
     Paystack Charges API
     Reference: https://paystack.com/docs/api/charge/
     """
 
     async def create_charge(
         self,
             email: str,
             amount: int,
-            pin: Optional[Union[int, None]] = None,
+            metadata: Dict[str, List[Dict[str, Any]]],
             authorization_code: Optional[Union[str, None]] = None,
+            pin: Optional[Union[int, None]] = None,
             reference: Optional[Union[str, None]] = None,
             device_id: Optional[Union[str, None]] = None,
             bank: Optional[Union[Dict[str, str], None]] = None,
             bank_transfer: Optional[Union[Dict[PWT, Any], None]] = None,
             qr: Optional[Union[Dict[str, str], None]] = None,
             ussd: Optional[Union[Dict[str, str], None]] = None,
             mobile_money: Optional[Union[Dict[str, str], None]] = None,
-            metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a charge
 
         :param: email
         :param: amount
         :param: bank. (Set key ass: {code, account_number})
         :param: bank_transfer. (Set key as: {account_expires_at} and value: {datetime iso format})
@@ -60,130 +60,130 @@
             * mobile_money
 
             Send with a non-reusable authorization code:
             * pin
 
             mobile_money is only available in Ghana and Kenya
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "amount": amount,
+            "metadata": metadata,
             "authorization_code": authorization_code,
             "bank": bank,
             "bank_transfer": bank_transfer,
             "qr": qr,
             "pin": pin,
             "reference": reference,
             "ussd": ussd,
             "mobile_money": mobile_money,
             "device_id": device_id,
-            "metadata": metadata,
         }
         return await self._post_request("/charge", data=data)
 
-    async def submit_pin(self, pin: int, reference: str) -> Response:
+    async def submit_pin(self, pin: int, reference: str) -> PayStackResponse:
         """
         Submit a PIN for a charge
 
         :param: pin
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "pin": pin,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_pin", data=data)
 
-    async def submit_otp(self, otp: int, reference: str) -> Response:
+    async def submit_otp(self, otp: int, reference: str) -> PayStackResponse:
         """
         Submit OTP to complete a charge
 
         :param: otp
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "otp": otp,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_otp", data=data)
 
-    async def submit_phone(self, phone: str, reference: str) -> Response:
+    async def submit_phone(self, phone: str, reference: str) -> PayStackResponse:
         """
         Submit a phone number to complete a charge
 
         :param: phone
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "phone": phone,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_phone", data=data)
 
-    async def submit_birthday(self, birthday: date, reference: str) -> Response:
+    async def submit_birthday(self, birthday: date, reference: str) -> PayStackResponse:
         """
         Submit birthday when required
 
         :param: birthday
         :param: reference
 
         note::
 
             Birthday submitted by user e.g. 2016-09-21
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         birthday = self._convert_to_string(birthday)
 
         data = {
             "birthday": birthday,
             "reference": reference,
         }
         return await self._post_request("/charge/submit_birthday", data=data)
 
     async def submit_address(
         self, reference: str, address: str, city: str, state: str, zipcode: str
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Submit address to continue a charge
 
         :param: reference
         :param: address
         :param: city
         :param: state
         :param: zipcode
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "reference": reference,
             "address": address,
             "city": city,
             "state": state,
             "zip_code": zipcode,
         }
         return await self._post_request("/charge/submit_address", data=data)
 
-    async def check_pending_charge(self, reference: str) -> Response:
+    async def check_pending_charge(self, reference: str) -> PayStackResponse:
         """
         Check pending charge
 
         :param: reference
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request(f"/charge/{reference}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/acustomers.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/customers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,186 +1,185 @@
 """
-Wrapper for Asynchronous Paystack Customers API.
+Wrapper for Paystack Customers API.
 
 The Customers API allows you to create and manage customers on your integration.
 """
 
 from datetime import date
-
 from typing import Optional, Dict, Any, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import RiskAction
+
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import RiskAction
 
 
-class AsyncCustomerClientAPI(AsyncPayStackBaseClientAPI):
+class CustomerClientAPI(SyncRequestAPI):
     """
     Paystack Customer API
     Reference: https://paystack.com/docs/api/customer/
     """
 
-    async def create_customer(
-            self,
-            email: str,
-            first_name: str,
-            last_name: str,
-            phone: str,
+    def create_customer(
+            self, 
+            email: str, 
+            first_name: str, 
+            last_name: str, 
+            phone: str, 
             metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return await self._post_request("/customer", data=data)
+        return self._post_request("/customer", data=data)
 
-    async def validate_customer(
+    def validate_customer(
             self,
             email_or_code: str,
             first_name: str,
             last_name: str,
             account_type: str,
             country: str,
             bank_code: str,
             account_number: str,
             bvn: str,
             customer_id_num: Optional[Union[str, None]] = None,
             middle_name: Optional[Union[str, None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Validate a customer's identity
 
         :param: email_or_code: The email or code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: middle_name: The middle name of the customer.
         :param: account_type: The type of account. Only bank_account is currently supported.
         :param: customer_id_num: The customer identification number
         :param: country: The country of the customer. 2-letter country code of identification issuer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: account_number: The account number of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "middle_name": middle_name,
             "type": account_type,
             "value": customer_id_num,
             "country": country,
             "bvn": bvn,
             "bank_code": bank_code,
             "account_number": account_number,
         }
-        return await self._post_request(f"customer/{email_or_code}/identification", data=data)
+        return self._post_request(f"customer/{email_or_code}/identification", data=data)
 
-    async def whitelist_blacklist_customer(
+    def whitelist_blacklist_customer(
             self, email_or_code: str, risk_action: Optional[Union[RiskAction, None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Whitelist or blacklist a customer
 
         :param: email_or_code: The code or email of the customer.
         :param: risk_action: The action to take on the customer. value: RiskAction.value.value = "allow" pr "deny"
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "customer": email_or_code,
             "risk_action": risk_action
         }
-        return await self._post_request("/customer/set_risk_action", data=data)
+        return self._post_request("/customer/set_risk_action", data=data)
 
-    async def deactivate_authorization(self, authorization_code: str) -> Response:
+    def deactivate_authorization(self, authorization_code: str) -> PayStackResponse:
         """
         Deactivate an authorization when the card needs to be forgotten
 
         :param: authorization_code: The authorization code to be deactivated.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"authorization_code": authorization_code}
-        return await self._post_request("/customer/deactivate_authorization", data=data)
+        return self._post_request("/customer/deactivate_authorization", data=data)
 
-    async def update_customer(
+    def update_customer(
             self,
             customer_code: str,
             first_name: Optional[Union[str, None]] = None,
             last_name: Optional[Union[str, None]] = None,
             phone: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, Any], None]] = None
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a customer
 
         :param: customer_code: The code of the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
         :param: metadata: The metadata of the customer in JSON format. {"key1": "value1", "key2": "value2"}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "metadata": metadata,
         }
-        return await self._put_request(f"/customer/{customer_code}", data=data)
+        return self._put_request(f"/customer/{customer_code}", data=data)
 
-    async def fetch_customer(self, email_or_code: str) -> Response:
+    def fetch_customer(self, email_or_code: str) -> PayStackResponse:
         """
         Fetch details of a specific customer
 
         :param: email_or_code: The email or code of the customer.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/customer/{email_or_code}")
+        return self._get_request(f"/customer/{email_or_code}")
 
-    async def list_customers(
+    def list_customers(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all customers
 
         :param: per_page: The number of records to return.
         :param: page: The page number to return.
         :param: from_date: The date to start returning customers from
         :param: to_date: The date to stop returning customers from
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date  to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/customer", params=params)
+        return self._get_request("/customer", params=params)
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/adedicated_virtual_accounts.py` & `paystackease-2.0.0/paystackease/apis/async_apis/adedicated_virtual_accounts.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Wrapper for Asynchronous Paystack Dedicated Virtual Account API
 
 The Dedicated Virtual Account API enables Nigerian merchants to manage unique payment accounts of their customers.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import Currency
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
 
-class AsyncDedicatedVirtualAccountClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncDedicatedVirtualAccountClientAPI(AsyncRequestAPI):
     """
     Paystack Dedicated Virtual Account API
     Reference: https://paystack.com/docs/api/dedicated-virtual-account/
 
     note::
         Ensure Dedicated NUBAN is available for your business. Contact Paystack Support
     """
@@ -25,15 +25,15 @@
             customer_id_or_code: str,
             preferred_bank: Optional[Union[str, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             split_code: Optional[Union[str, None]] = None,
             first_name: Optional[Union[str, None]] = None,
             last_name: Optional[Union[str, None]] = None,
             phone: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a dedicated virtual account for existing customers.
         Currently, support Wema Bank and Titan Paystack.
 
         :param: customer_id_or_code: The customer's ID or Code
         :param: preferred_bank: Preferred bank slug for the virtual account. Eg: "wema-bank"
 
@@ -43,16 +43,16 @@
 
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
         :param: first_name: First name of the customer
         :param: last_name: Last name of the customer
         :param: phone: Phone number of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
             "first_name": first_name,
@@ -70,15 +70,15 @@
             preferred_bank: str,
             country: str,
             account_number: Optional[Union[str, None]] = None,
             bvn: Optional[Union[str, None]] = None,
             bank_code: Optional[Union[str, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             split_code: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         create a customer, validate the customer, and assign a DVA to the customer
 
         :param: email: The email associated with the customer.
         :param: first_name: The first name of the customer.
         :param: last_name: The last name of the customer.
         :param: phone: The phone number of the customer.
@@ -96,16 +96,16 @@
 
         :param: account_number: The account number of the customer
         :param: bvn: The Bank Verification Number
         :param: bank_code: The bank code of the customer
         :param: subaccount: Subaccount code of the account you want to split the transaction.
         :param: split_code: Split code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "first_name": first_name,
             "last_name": last_name,
             "phone": phone,
             "preferred_bank": preferred_bank,
@@ -121,129 +121,129 @@
     async def list_dedicated_account(
             self,
             active: Optional[Union[bool, None]] = True,
             currency: Optional[Union[Currency, None]] = None,
             provider_slug: Optional[Union[str, None]] = None,
             bank_id: Optional[Union[str, None]] = None,
             customer_id: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List dedicated accounts
 
         :param: active: Shows the status of the dedicated virtual account
         :param: currency: Currency of the dedicated virtual account
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: bank_id: Bank ID of the dedicated virtual account eg: 035
         :param: customer_id: Customer ID of the dedicated virtual account
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert date to string
         active = self._convert_to_string(active)
 
         params = {
             "active": active,
             "currency": currency,
             "provider_slug": provider_slug,
             "bank_id": bank_id,
             "customer": customer_id,
         }
         return await self._get_request("/dedicated_account", params=params)
 
-    async def fetch_dedicated_account(self, dedicated_account_id: int) -> Response:
+    async def fetch_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
         """
         Get details of a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request(f"/dedicated_account/{dedicated_account_id}")
 
     async def requery_dedicated_account(
             self,
             account_number: Optional[Union[str, None]] = None,
             provider_slug: Optional[Union[str, None]] = None,
             date_transfer: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Requery a dedicated virtual account for new transactions
 
         :param: account_number: Virtual Account number to requery
         :param: provider_slug: Provider slug in lowercase eg: wema-bank
         :param: date_transfer: Date of when the transfer was made
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         date_transfer = self._convert_to_string(date_transfer)
 
         params = {
             "account_number": account_number,
             "provider_slug": provider_slug,
             "date": date_transfer,
         }
         return await self._get_request("/dedicated_account/requery", params=params)
 
-    async def deactivate_dedicated_account(self, dedicated_account_id: int) -> Response:
+    async def deactivate_dedicated_account(self, dedicated_account_id: int) -> PayStackResponse:
         """
         Deactivate a dedicated virtual account
 
         :param: dedicated_account_id: Dedicated account ID
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._delete_request(f"/dedicated_account/{dedicated_account_id}")
 
     async def split_dedicated_account(
             self,
             customer_id_or_code: str,
             subaccount: Optional[Union[str, None]] = None,
             split_code: Optional[Union[str, None]] = None,
             preferred_bank: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Split a dedicated virtual account transaction with one or more accounts
 
         :param: customer_id_or_code: Customer's ID or Code
         :param: subaccount: Subaccount code of the account you want to split the transaction
         :param: split_code: Split code
         :param: preferred_bank: Preferred bank for the virtual account
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "customer": customer_id_or_code,
             "preferred_bank": preferred_bank,
             "subaccount": subaccount,
             "split_code": split_code,
         }
         return await self._post_request("/dedicated_account/split", data=data)
 
-    async def remove_split_dedicated_account(self, account_number: str) -> Response:
+    async def remove_split_dedicated_account(self, account_number: str) -> PayStackResponse:
         """
         Remove a split dedicated virtual account
 
         :param: account_number: the account number of the dedicated virtual account
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "account_number": account_number,
         }
         return await self._delete_request("/dedicated_account/split", data=data)
 
-    async def fetch_bank_providers(self) -> Response:
+    async def fetch_bank_providers(self) -> PayStackResponse:
         """
         Fetch bank providers
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request("/dedicated_account/available_providers")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/amiscellaneous.py` & `paystackease-2.0.0/paystackease/apis/async_apis/amiscellaneous.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Wrapper for Paystack Miscellaneous API.
 
 The Miscellaneous API are supporting APIs that can be used to provide more details to other APIs.
 """
 
 from typing import Optional, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import GateWay, Channels, Currency
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import GateWay, Channels, Currency
 
-class AsyncMiscellaneousClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncMiscellaneousClientAPI(AsyncRequestAPI):
     """
     Paystack Miscellaneous API
     Reference: https://paystack.com/docs/api/miscellaneous/
     """
 
     async def list_banks(
             self,
@@ -25,15 +25,15 @@
             pay_with_bank: Optional[Union[bool, None]] = False,
             enabled_for_verification: Optional[Union[bool, None]] = False,
             next_cursor: Optional[Union[str, None]] = None,
             previous_cursor: Optional[Union[str, None]] = None,
             gateway: Optional[Union[GateWay, None]] = None,
             channel_type: Optional[Union[Channels, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Get a list of all supported banks and their properties
 
         :param: country: The country to obtain the list of supported banks.
                         Values { country=ghana or country=nigeria }
         :param: use_cursor: Use cursor to paginate through the list of supported banks
         :param: per_page: The number of records to return per page: 10, 20 or 50
@@ -48,16 +48,16 @@
         :param: currency: filter for banks that support a specific currency
         :param: channel_type: Type of financial channel. { Channels.value.value}
 
         **note::**
 
         For Ghanaian channels, please use either mobile_money for mobile money channels OR ghipps for bank channels
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert to strings
         use_cursor = self._convert_to_string(use_cursor)
         pay_with_bank_transfer = self._convert_to_string(pay_with_bank_transfer)
         pay_with_bank = self._convert_to_string(pay_with_bank)
         enabled_for_verification = self._convert_to_string(enabled_for_verification)
@@ -73,27 +73,27 @@
             "previous": previous_cursor,
             "gateway": gateway,
             "type": channel_type,
             "currency": currency,
         }
         return await self._get_request("/bank", params=params)
 
-    async def list_countries(self) -> Response:
+    async def list_countries(self) -> PayStackResponse:
         """
         Get a list of all supported countries and their properties
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request("/country")
 
-    async def list_states(self, country: str) -> Response:
+    async def list_states(self, country: str) -> PayStackResponse:
         """
         Get a list of all supported states and their properties
 
         :param: country: The country code from which to obtain the list of supported states
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {"country": country}
         return await self._get_request("/address_verification/states", params=params)
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/apayment_pages.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/payment_pages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,157 +1,157 @@
 """
-Wrapper for Asynchronous Paystack Payment Pages API.
+Wrapper for Paystack Payment Pages API.
 
 The Payment Pages API provides a quick and secure way to collect payment for products.
 """
 
 from datetime import date
 from typing import Optional, Dict, List, Any, Union
-from paystackease._utils import Response
-from paystackease._abase import AsyncPayStackBaseClientAPI
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
 
-class AsyncPaymentPagesClientAPI(AsyncPayStackBaseClientAPI):
+
+class PaymentPagesClientAPI(SyncRequestAPI):
     """
     Paystack Payment Pages API
     Reference: https://paystack.com/docs/api/page/
     """
 
-    async def create_payment_page(
+    def create_payment_page(
             self,
             name: str,
             description: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             split_code: Optional[Union[str, None]] = None,
             page_slug: Optional[Union[str, None]] = None,
             redirect_url: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, Any], None]] = None,
             custom_fields: Optional[Union[List[Dict[str, Any]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a payment page
 
         :param: name: Name of the page
         :param: description: Description of the page
         :param: amount: Amount of the page
         :param: split_code: Split code of the transaction split
         :param: page_slug: URL slug you would like to be associated with this page.
-
+        
         note::
 
             Page will be accessible at https://paystack.com/pay/page_slug
 
         :param: redirect_url: If you would like Paystack to redirect someplace
                                 upon successful payment, specify the URL here.
         :param: metadata: Extra data to configure the payment page including subaccount,logo image, transaction charge
         :param: custom_fields: If you would like to accept custom fields, specify them here.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "name": name,
             "description": description,
             "amount": amount,
             "split_code": split_code,
             "slug": page_slug,
             "redirect_url": redirect_url,
             "metadata": metadata,
             "custom_fields": custom_fields,
         }
-        return await self._post_request("/page", data=data)
+        return self._post_request("/page", data=data)
 
-    async def list_payment_pages(
+    def list_payment_pages(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the payment pages
 
         :param: per_page: Number of records to return
         :param: page: number to return
         :param: from_date: A timestamp from which to start listing page
         :param: to_date: A timestamp from which to start listing page
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
 
         note::
             Date Time value is in this format: 2016-09-24T00:00:05.000Z, 2016-09-21
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/page", params=params)
+        return self._get_request("/page", params=params)
 
-    async def fetch_payment_page(self, page_id_or_slug: str) -> Response:
+    def fetch_payment_page(self, page_id_or_slug: str) -> PayStackResponse:
         """
         Get details of a payment page
 
         :param: page_id_or_slug: ID or slug of the payment page
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/page/{page_id_or_slug}")
+        return self._get_request(f"/page/{page_id_or_slug}")
 
-    async def update_payment_page(
+    def update_payment_page(
             self,
             page_id_or_slug: str,
             name: Optional[Union[str, None]] = None,
             description: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             active: Optional[Union[bool, None]] = True,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a payment page detail
 
         :param: page_id_or_slug: ID or slug of the payment page
         :param: name: Name of the page
         :param: description: Description of the page
         :param: amount: Amount of the page
         :param: active: Set false to deactivate the page url
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "name": name,
             "description": description,
             "amount": amount,
             "active": active,
         }
-        return await self._put_request(f"/page/{page_id_or_slug}", data=data)
+        return self._put_request(f"/page/{page_id_or_slug}", data=data)
 
-    async def check_slug_available(self, page_slug: str) -> Response:
+    def check_slug_available(self, page_slug: str) -> PayStackResponse:
         """
         Check if a slug is available
 
         :param: page_slug: URL slug you would like to be associated with this page.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/page/check_slug_availability/{page_slug}")
+        return self._get_request(f"/page/check_slug_availability/{page_slug}")
 
-    async def add_products(self, payment_id: int, product: List[int]) -> Response:
+    def add_products(self, payment_id: int, product: List[int]) -> PayStackResponse:
         """
         Add products to a payment page
 
         :param: payment_id: ID of the payment page
         :param: product: List of IDS of all the products
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"product": product}
-        return await self._post_request(f"/page/{payment_id}/product", data=data)
+        return self._post_request(f"/page/{payment_id}/product", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/apayment_requests.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/payment_requests.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
-Wrapper for Asynchronous Paystack Payment Requests API.
+Wrapper for Paystack Payment Requests API.
 
 The Payment Requests API allows you manage requests for payment of goods and services.
 """
 
 from datetime import date
 from typing import Optional, List, Dict, Any, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import PayMentRequestStatus, Currency
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import PayMentRequestStatus, Currency
 
-class AsyncPaymentRequestClientAPI(AsyncPayStackBaseClientAPI):
+
+class PaymentRequestClientAPI(SyncRequestAPI):
     """
     Paystack Payment Request API
     Reference: https://paystack.com/docs/api/payment-request/
     """
 
-    async def create_payment_request(
+    def create_payment_request(
             self,
             customer: str,
             amount: int,
             draft: bool,
             has_invoice: bool,
             send_notification: bool,
             due_date: Optional[Union[date, None]] = None,
             description: Optional[Union[str, Any]] = None,
             line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
             tax: Optional[Union[List[Dict[str, Any]], None]] = None,
             currency: Optional[Union[Currency, Any]] = None,
             invoice_number: Optional[Union[int, Any]] = None,
             split_code: Optional[Union[str, Any]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a payment request for a transaction
 
         :param: customer: Customer ID of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
         :param: description: Description of the payment request
@@ -44,16 +44,16 @@
         :param: currency: Currency of the payment request
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: has_invoice: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request
         :param: split_code: split code of the transaction split
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
         draft = self._convert_to_string(draft)
         has_invoice = self._convert_to_string(has_invoice)
         send_notification = self._convert_to_string(send_notification)
 
@@ -67,41 +67,41 @@
             "currency": currency,
             "send_notification": send_notification,
             "draft": draft,
             "has_invoice": has_invoice,
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
-        return await self._post_request("/paymentrequest", data=data)
+        return self._post_request("/paymentrequest", data=data)
 
-    async def list_payment_requests(
+    def list_payment_requests(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[str, None]] = None,
             status: Optional[Union[PayMentRequestStatus, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             include_archive: Optional[Union[bool, None]] = True,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the payment requests
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: customer: Filter by customer ID
         :param: status: Filter by payment request status
         :param: currency:
         :param: include_archive: Show archived payment requests
         :param: from_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
         :param: to_date: A timestamp from which to get payment requests {2016-09-24T00:00:05.000Z, 2016-09-21}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
         include_archive = self._convert_to_string(include_archive)
 
@@ -111,89 +111,89 @@
             "customer": customer,
             "status": status,
             "currency": currency,
             "include_archive": include_archive,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/paymentrequest", params=params)
+        return self._get_request("/paymentrequest", params=params)
 
-    async def fetch_payment_request(self, id_or_code: str) -> Response:
+    def fetch_payment_request(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a payment request on your integration
 
         :param: id_or_code: ID or Code of the payment request
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/paymentrequest/{id_or_code}")
+        return self._get_request(f"/paymentrequest/{id_or_code}")
 
-    async def verify_payment_request(self, code: str) -> Response:
+    def verify_payment_request(self, code: str) -> PayStackResponse:
         """
         Verify details of a payment request on your integration
 
         :param: code: Payment request code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/paymentrequest/verify/{code}")
+        return self._get_request(f"/paymentrequest/verify/{code}")
 
-    async def send_notification(self, code: str) -> Response:
+    def send_notification(self, code: str) -> PayStackResponse:
         """
         Send notification of a payment request to a customer
 
         :param: code: Payment request code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._post_request(f"/paymentrequest/notify/{code}")
+        return self._post_request(f"/paymentrequest/notify/{code}")
 
-    async def payment_request_total(self) -> Response:
+    def payment_request_total(self) -> PayStackResponse:
         """
         Get total of a payment request metric
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request("/paymentrequest/totals")
+        return self._get_request("/paymentrequest/totals")
 
-    async def finalize_payment_request(self, code: str, send_notification: bool) -> Response:
+    def finalize_payment_request(self, code: str, send_notification: bool) -> PayStackResponse:
         """
         Finalize a draft payment request
 
         :param: code: Payment request code
         :param: send_notification: Set true if you want to send a notification to the customer email
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert to strings
         send_notification = self._convert_to_string(send_notification)
 
         data = {"send_notification": send_notification}
-        return await self._post_request(f"/paymentrequest/finalize/{code}", data=data)
+        return self._post_request(f"/paymentrequest/finalize/{code}", data=data)
 
-    async def update_payment_request(
+    def update_payment_request(
             self,
             id_or_code: str,
             customer: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             description: Optional[Union[str, None]] = None,
             line_items: Optional[Union[List[Dict[str, Any]], None]] = None,
             tax: Optional[Union[List[Dict[str, Any]], None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             due_date: Optional[Union[date, None]] = None,
             send_notification: Optional[Union[bool, None]] = True,
             draft: Optional[Union[bool, None]] = True,
             invoice_number: Optional[Union[int, None]] = None,
             split_code: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a payment request
 
         :param: id_or_code: ID or Code of the payment request
         :param: customer: Customer ID or code of the customer
         :param: amount: Amount of the payment request
         :param: due_date: Due date of the payment request
@@ -202,16 +202,16 @@
         :param: tax: Array of tax int the format [{"name":"VAT", "amount":200}]
         :param: currency: Currency of the payment request
         :param: send_notification: Set true if you want to send a notification to the customer email
         :param: draft: Set true if you want to create a draft payment request
         :param: invoice_number: Invoice number of the payment request starts from 1 and autoincrement
         :param: split_code: split code of the transaction split
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         due_date = self._convert_to_string(due_date)
         draft = self._convert_to_string(draft)
         send_notification = self._convert_to_string(send_notification)
 
@@ -224,19 +224,19 @@
             "tax": tax,
             "currency": currency,
             "send_notification": send_notification,
             "draft": draft,
             "invoice_number": invoice_number,
             "split_code": split_code,
         }
-        return await self._put_request(f"/paymentrequest/{id_or_code}", data=data)
+        return self._put_request(f"/paymentrequest/{id_or_code}", data=data)
 
-    async def archive_payment_request(self, code: str) -> Response:
+    def archive_payment_request(self, code: str) -> PayStackResponse:
         """
         Archive a payment request
 
         :param: code: Payment request code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._post_request(f"/paymentrequest/archive/{code}")
+        return self._post_request(f"/paymentrequest/archive/{code}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/aplans.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/plans.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 """
-Wrapper for Asynchronous Paystack Plans API
+Wrapper for Paystack Plans API
 
 The Plans API allows you to create and manage installment payment options on your integration.
 """
 
 from typing import Optional, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import Interval
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Interval
 
-class AsyncPlanClientAPI(AsyncPayStackBaseClientAPI):
+
+class PlanClientAPI(SyncRequestAPI):
     """
     Paystack Plan API
     Reference: https://paystack.com/docs/api/plan/
     """
 
-    async def create_plan(
+    def create_plan(
             self,
             name: str,
             amount: int,
             interval: Interval,
             currency: str,
             invoice_limit: int,
             send_invoices: bool,
             send_sms: bool,
             description: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a plan
 
         :param: name: Name of the plan
         :param: amount: Amount of the plan
         :param: interval: Interval of the plan. Values [Interval.value.value]
         :param: description: Description of the plan
         :param: send_invoices: Send invoices to customer
         :param: send_sms: Send SMS to customer
         :param: currency: Currency of the plan
         :param: invoice_limit: Invoice limit of the plan
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert to strings
         send_invoices = self._convert_to_string(send_invoices)
         send_sms = self._convert_to_string(send_sms)
 
         data = {
             "name": name,
@@ -52,83 +52,83 @@
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
             "currency": currency,
             "invoice_limit": invoice_limit,
         }
-        return await self._post_request("/plan", data=data)
+        return self._post_request("/plan", data=data)
 
-    async def list_plans(
+    def list_plans(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             status: Optional[Union[str, None]] = None,
             interval: Optional[Union[Interval, None]] = None,
             amount: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the plans
 
         :param: per_page: Number of records to return
         :param: page:  number to return
         :param: status: Filter list by plans with specified status
         :param: interval: Filter list by plans with specified interval
         :param: amount
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {
             "perPage": per_page,
             "page": page,
             "status": status,
             "interval": interval,
             "amount": amount,
         }
-        return await self._get_request("/plan", params=params)
+        return self._get_request("/plan", params=params)
 
-    async def fetch_plan(self, id_or_code: str) -> Response:
+    def fetch_plan(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a plan
 
         :param: id_or_code: ID or Code of the plan
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/plan/{id_or_code}")
+        return self._get_request(f"/plan/{id_or_code}")
 
-    async def update_plan(
+    def update_plan(
             self,
             id_or_code: str,
             name: str,
             amount: int,
             interval: Interval,
             send_invoices: bool,
             send_sms: bool,
             currency: str,
             invoice_limit: int,
             description: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a plan detail
 
         :param: id_or_code: ID or Code of the plan
         :param: name: Name of the plan
         :param: amount: Amount of the plan
         :param: interval: Interval of the plan. [Interval.value.value]
         :param: description:
         :param: send_invoices:
         :param: send_sms:
         :param: currency:
         :param: invoice_limit:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         # convert to strings
         send_invoices = self._convert_to_string(send_invoices)
         send_sms = self._convert_to_string(send_sms)
 
         data = {
             "name": name,
@@ -136,8 +136,8 @@
             "interval": interval,
             "description": description,
             "send_invoices": send_invoices,
             "send_sms": send_sms,
             "currency": currency,
             "invoice_limit": invoice_limit,
         }
-        return await self._put_request(f"/plan/{id_or_code}", data=data)
+        return self._put_request(f"/plan/{id_or_code}", data=data)
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/asettlements.py` & `paystackease-2.0.0/paystackease/apis/async_apis/asettlements.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 Wrapper for Asynchronous Paystack Settlements API
 
 The Settlements API allows you to gain insights into payouts made by Paystack to your bank account.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._utils import Response
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease.helpers.tool_kit import STATUS
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import STATUS
 
-class AsyncSettlementClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncSettlementClientAPI(AsyncRequestAPI):
     """
     Paystack Settlement API
     Reference: https://paystack.com/docs/api/settlement/
     """
 
     async def list_settlements(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             status: Optional[Union[STATUS, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List settlements made to your settlement accounts
 
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: status: Value can be one of success, processing, pending or failed.
         :param: subaccount:
         :param: from_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date: A timestamp from which to start listing settlements e.g. 2016-09-24T00:00:05.000Z, 2016-09-21
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -57,26 +57,26 @@
     async def list_settlement_transactions(
             self,
             settlement_id: int,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Get the transactions that make up a particular settlement
 
         :param: settlement_id: The id of the settlement.
         :param: per_page: The number of records to return per page.
         :param: page: the number to retrieve.
         :param: from_date: A timestamp from which to start listing settlements
         :param: to_date: A timestamp from which to start listing settlements
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
 
         note::
 
             Date and time format: 2016-09-24T00:00:05.000Z, 2016-09-21
 
         """
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/asubaccounts.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/subaccounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 """
-Wrapper for Asynchronous Paystack SubAccounts API
+Wrapper for Paystack SubAccounts API
 
 The Subaccounts API allows you to create and manage subaccounts on your integration.
 Subaccounts can be used to split payment between two accounts (your main account and a subaccount).
 """
 
 from datetime import date
 from typing import Optional, Dict, List, Any, Union
-from paystackease._utils import Response
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease.helpers.tool_kit import SettlementSchedule
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import SettlementSchedule
 
-class AsyncSubAccountClientAPI(AsyncPayStackBaseClientAPI):
+
+class SubAccountClientAPI(SyncRequestAPI):
     """
     Paystack SubAccount API
     Reference: https://paystack.com/docs/api/subaccount/
     """
 
-    async def create_subaccount(
+    def create_subaccount(
             self,
             business_name: str,
             settlement_bank: str,
             account_number: str,
             percentage_charge: float,
             description: str,
             primary_contact_email: Optional[Union[str, None]] = None,
             primary_contact_name: Optional[Union[str, None]] = None,
             primary_contact_phone: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a subaccount
 
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: Bank Code for the bank
         :param: account_number: The account number of the subaccount.
         :param: percentage_charge: The percentage charge receives from each payment made to the subaccount
         :param: description: The description of the subaccount.
         :param: primary_contact_email: A contact email for the subaccount
         :param: primary_contact_name: A name for the contact person for this subaccount
         :param: primary_contact_phone: A phone number to call for this subaccount
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "business_name": business_name,
             "settlement_bank": settlement_bank,
             "account_number": account_number,
             "percentage_charge": percentage_charge,
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "metadata": metadata,
         }
-        return await self._post_request("/subaccount", data=data)
+        return self._post_request("/subaccount", data=data)
 
-    async def update_subaccount(
+    def update_subaccount(
             self,
             id_or_code: str,
             business_name: str,
             settlement_bank: str,
             account_number: str,
             active: Optional[Union[bool, None]] = True,
             percentage_charge: Optional[Union[float, None]] = None,
             description: Optional[Union[str, None]] = None,
             primary_contact_email: Optional[Union[str, None]] = None,
             primary_contact_name: Optional[Union[str, None]] = None,
             primary_contact_phone: Optional[Union[str, None]] = None,
             settlement_schedule: Optional[Union[SettlementSchedule, None]] = SettlementSchedule.AUTO.value,
             metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a subaccount
 
         :param: id_or_code: The id or code of the subaccount.
         :param: business_name: The business name of the subaccount.
         :param: settlement_bank: The settlement bank of the subaccount.
         :param: account_number
@@ -87,20 +87,20 @@
         :param: primary_contact_email
         :param: primary_contact_name
         :param: primary_contact_phone
         :param: settlement_schedule: Values: [ auto, weekly, `monthly`, `manual` ].
 
         note::
             Auto means payout is T+1
-            Manual means payout to the subaccount should only be made when requested. async defaults to auto
+            Manual means payout to the subaccount should only be made when requested. Defaults to auto
 
         :param: metadata: Stringified JSON object. {"custom_fields": [{"name": "value"}]}
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "business_name": business_name,
@@ -111,45 +111,45 @@
             "description": description,
             "primary_contact_email": primary_contact_email,
             "primary_contact_name": primary_contact_name,
             "primary_contact_phone": primary_contact_phone,
             "settlement_schedule": settlement_schedule,
             "metadata": metadata,
         }
-        return await self._put_request(f"/subaccount/{id_or_code}", data=data)
+        return self._put_request(f"/subaccount/{id_or_code}", data=data)
 
-    async def list_subaccounts(
+    def list_subaccounts(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all subaccounts
 
         :param: per_page: The number of records to return per page.
         :param: page: The number to retrieve.
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
-        return await self._get_request("/subaccount", params=params)
+        return self._get_request("/subaccount", params=params)
 
-    async def fetch_subaccount(self, id_or_code: str) -> Response:
+    def fetch_subaccount(self, id_or_code: str) -> PayStackResponse:
         """
         Fetch details of a specific subaccount
 
         :param: id_or_code: The id or code of the subaccount.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/subaccount/{id_or_code}")
+        return self._get_request(f"/subaccount/{id_or_code}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/asubscriptions.py` & `paystackease-2.0.0/paystackease/apis/async_apis/asubscriptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 Wrapper for Paystack Subscriptions API
 
 The Subscriptions API allows you to create and manage recurring payment on your integration.
 """
 
 from datetime import date
 from typing import Optional, Union
-from paystackease._utils import Response
-from paystackease._abase import AsyncPayStackBaseClientAPI
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
 
-class AsyncSubscriptionClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncSubscriptionClientAPI(AsyncRequestAPI):
     """
     Paystack Subscription API
     Reference: https://paystack.com/docs/api/subscription/
     """
 
     async def create_subscription(
             self,
             customer: str,
             plan_code: str,
             authorization: str,
             start_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a subscription
 
         :param: customer: Email or Code of the customer
         :param: plan_code: Code of the plan
         :param: authorization: Code of the authorization
         :param: start_date: Start date of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         start_date = self._convert_to_string(start_date)
 
         data = {
             "customer": customer,
@@ -48,85 +48,85 @@
 
     async def list_subscriptions(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[int, None]] = None,
             plan_code: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the subscriptions
 
         :param: per_page: Number of records to return per page.
         :param: page: THe number to return
         :param: customer:
         :param: plan_code:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {
             "perPage": per_page,
             "page": page,
             "customer": customer,
             "plan": plan_code,
         }
         return await self._get_request("/subscription", params=params)
 
-    async def fetch_subscription(self, id_or_code: str) -> Response:
+    async def fetch_subscription(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a subscription
 
         :param: id_or_code: ID or Code of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request(f"/subscription/{id_or_code}")
 
-    async def enable_subscription(self, subscription_code: str, token: str) -> Response:
+    async def enable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
         """
         Enable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"code": subscription_code, "token": token}
         return await self._post_request("/subscription/enable", data=data)
 
-    async def disable_subscription(self, subscription_code: str, token: str) -> Response:
+    async def disable_subscription(self, subscription_code: str, token: str) -> PayStackResponse:
         """
         Disable a subscription
 
         :param: subscription_code: Code of the subscription
         :param: token: Email token of the customer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"code": subscription_code, "token": token}
         return await self._post_request("/subscription/disable", data=data)
 
-    async def generate_update_subscription(self, subscription_code: str) -> Response:
+    async def generate_update_subscription(self, subscription_code: str) -> PayStackResponse:
         """
         Generate a link for updating the card on subscription
 
         :param: subscription_code: Code of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._post_request(f"/subscription/{subscription_code}/manage/link")
 
-    async def send_update_subscription_link(self, subscription_code: str) -> Response:
+    async def send_update_subscription_link(self, subscription_code: str) -> PayStackResponse:
         """
         Email a customer a link for updating the card on their subscription
 
         :param: subscription_code: Code of the subscription
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._post_request(f"/subscription/{subscription_code}/manage/email")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/atransaction_splits.py` & `paystackease-2.0.0/paystackease/apis/async_apis/atransaction_splits.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,106 +2,107 @@
 Wrapper for Asynchronous Paystack Transaction Splits APIs
 
 The Transaction Splits API enables merchants split the settlement for a transaction
 across their payout account, and one or more subaccounts.
 """
 from datetime import date
 from typing import Optional, List, Dict, Any, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
 
-class AsyncTransactionSplitClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncTransactionSplitClientAPI(AsyncRequestAPI):
     """
     Paystack Transaction Split API
     Reference: https://paystack.com/docs/api/split/
     """
 
     async def create_split(
             self,
             transaction_split_name: str,
             transaction_split_type: str,
-            currency: str,
+            currency: Currency,
             subaccounts: List[Dict[str, Any]],
             bearer_type: str,
             bearer_subaccount: str,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a split payment on your integration
 
         :param: transaction_split_name: Name of the transaction split
         :param: transaction_split_type: The type of transaction split you want to create [ percentage | flat ]
         :param: currency: [ Currency.value.value ]
         :param: subaccounts: A list of object containing subaccount code and number of shares
                             [{subaccount: ‘ACT_xxxxxxxxxx’, share: xxx},{...}]
         :param: bearer_type: Any of subaccount | account | all-proportional | all
         :param: bearer_subaccount: Subaccount code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "name": transaction_split_name,
             "type": transaction_split_type,
             "currency": currency,
             "subaccounts": subaccounts,
             "bearer_type": bearer_type,
             "bearer_subaccount": bearer_subaccount,
         }
         return await self._post_request("/split", data=data)
 
     async def add_or_update_subaccount_split(
             self, split_id: str, subaccount: str, transaction_share: int
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Add a Subaccount to a Transaction Split, or update the share of
         an existing Subaccount in a Transaction Split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
         :param: transaction_share: The number of shares
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"subaccount": subaccount, "share": transaction_share}
         return await self._post_request(f"/split/{split_id}/subaccount/add", data=data)
 
-    async def remove_sub_account_split(self, split_id: str, subaccount: str) -> Response:
+    async def remove_sub_account_split(self, split_id: str, subaccount: str) -> PayStackResponse:
         """
         Remove a Sub Account from a transaction split
 
         :param: split_id: The split ID
         :param: subaccount: The subaccount code
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"subaccount": subaccount}
         return await self._post_request(f"/split/{split_id}/subaccount/remove", data=data)
 
     async def update_split(
             self,
             split_id: str,
             transaction_split_name: str,
             active: bool,
             bearer_type: Optional[Union[str, None]] = None,
             bearer_subaccount: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a specific transaction split details
 
         :param: split_id: The split ID
         :param: transaction_split_name: Name of the transaction split
         :param: active: True or False
         :param: bearer_type:
         :param: bearer_subaccount:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         active = self._convert_to_string(active)
 
         data = {
             "name": transaction_split_name,
@@ -116,28 +117,28 @@
             split_name: Optional[Union[str, None]] = None,
             active: Optional[Union[bool, None]] = True,
             sort_by: Optional[Union[str, None]] = None,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all the transaction splits
 
         :param: split_name: Name of the transaction split
         :param: active: True or False
         :param: sort_by: Sort by name, async defaults to createdAt date,
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         active = self._convert_to_string(active)
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
@@ -148,17 +149,17 @@
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
         return await self._get_request("/split", params=params)
 
-    async def fetch_split(self, split_id: str) -> Response:
+    async def fetch_split(self, split_id: str) -> PayStackResponse:
         """
         Fetch details of a specific transaction split
 
         :param: split_id: The split ID
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request(f"/split/{split_id}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/atransactions.py` & `paystackease-2.0.0/paystackease/apis/sync_apis/transactions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 """
-Wrapper for Asynchronous Paystack Transactions API
+Wrapper for Paystack Transactions API
 
 The Transactions API allows you to create and manage payments on your integration.
 """
 
 from datetime import date
 from typing import List, Optional, Dict, Any, Union
-from paystackease.helpers.tool_kit import TransactionStatus, Channels, Bearer, Currency
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
 
+from paystackease.core import PayStackResponse, SyncRequestAPI
+from paystackease.helpers import Channels, Currency, Bearer, TransactionStatus
 
-class AsyncTransactionClientAPI(AsyncPayStackBaseClientAPI):
+
+class TransactionClientAPI(SyncRequestAPI):
     """
     Paystack Transaction API
     Reference: https://paystack.com/docs/api/transaction/
     """
 
-    async def initialize(
+    def initialize(
             self,
             email: str,
             amount: int,
             currency: Optional[Union[Currency, None]] = Currency.NGN.value,
             reference: Optional[Union[str, None]] = None,
             callback_url: Optional[Union[str, None]] = None,
             plan: Optional[Union[str, None]] = None,
             invoice_limit: Optional[Union[int, None]] = None,
             channels: Optional[Union[List[Channels], None]] = None,
             split_code: Optional[Union[str, None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             transaction_charge: Optional[Union[int, None]] = None,
             bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
             metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Initialize a transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # Currency.value.value
         :param: reference:
         :param: callback_url: # Use this to override the callback url provided on the  dashboard
-                                # https://example.com/callback
-        :param: plan:  # If transaction is to create a subscription to a preasync defined plan, provide plan code here.
+                            # https://example.com/callback
+        :param: plan:  # If transaction is to create a subscription to a predefined plan, provide plan code here.
         :param: invoice_limit:  # Number of times to charge customer during subscription to plan
         :param: channels:  # [Channels.value.value, Channels.value.value, ...]
         :param: split_code:  # The split code of the transaction split. e.g. SPL_98WF13Eb3w
         :param: subaccount:  # The code for the subaccount that owns the payment. e.g. ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge: # An amount used to override the split configuration for a
                                     # single split payment
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "callback_url": callback_url,
@@ -67,30 +67,30 @@
             "channels": channels,
             "split_code": split_code,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "metadata": metadata,
         }
-        return await self._post_request("/transaction/initialize", data=data)
+        return self._post_request("/transaction/initialize", data=data)
 
-    async def charge_authorization(
+    def charge_authorization(
             self,
             email: str,
             amount: int,
             authorization_code: str,
             reference: Optional[Union[str, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             channels: Optional[Union[List[Channels], None]] = None,
             subaccount: Optional[Union[str, None]] = None,
             transaction_charge: Optional[int] = None,
             bearer: Optional[Union[Bearer, None]] = Bearer.ACCOUNT.value,
             queue: Optional[Union[bool, None]] = True,
             metadata: Optional[Union[Dict[str, List[Dict[str, Any]]], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Charge an authorization transaction
 
         :param: email:
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: authorization_code:  # value = AUTH_1234234WRFW
@@ -99,16 +99,16 @@
         :param: channels:  # [Channels.value.value, Channels.value.value, ...]
         :param: subaccount:  # value = ACCT_8f4s1eq7ml6rlzj
         :param: transaction_charge:
         :param: bearer:  # Who bears Paystack charges? Two options: account, subaccount
         :param: queue:  # If set to true, the transaction will be queued for processing
         :param: metadata:  # Stringified JSON object of custom data. {"foo": "bar" }
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert bool to string
         queue = self._convert_to_string(queue)
 
         data = {
             "email": email,
@@ -119,74 +119,74 @@
             "channels": channels,
             "subaccount": subaccount,
             "transaction_charge": transaction_charge,
             "bearer": bearer,
             "queue": queue,
             "metadata": metadata,
         }
-        return await self._post_request("/transaction/charge_authorization", data=data)
+        return self._post_request("/transaction/charge_authorization", data=data)
 
-    async def partial_debit(
+    def partial_debit(
             self,
             email: str,
             authorization_code: str,
             amount: int,
             currency: str,
             reference: Optional[Union[str, None]] = None,
             at_least: Optional[Union[int, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Charge a partial debit transaction
 
         :param: email:
         :param: authorization_code:  # value = AUTH_1234234WRFW
         :param: amount: amount should be in subunit in this case 10000 kobo = 100 naira.
                         Use convert_currency() to convert to subunit
         :param: currency:  # value = Currency.value.value
         :param: reference:  # Unique transaction reference.
         :param: at_least:  # Minimum amount to charge
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "email": email,
             "authorization_code": authorization_code,
             "amount": amount,
             "currency": currency,
             "reference": reference,
             "at_least": at_least,
         }
-        return await self._post_request("/transaction/partial_debit", data=data)
+        return self._post_request("/transaction/partial_debit", data=data)
 
-    async def list_transactions(
+    def list_transactions(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[int, None]] = None,
             terminal_id: Optional[Union[str, None]] = None,
             amount: Optional[Union[int, None]] = None,
             status: Optional[Union[TransactionStatus, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List all transactions
 
         :param: per_page:  # Specify how many records you want to retrieve per page.
         :param: page:  # Specify a page number to retrieve
         :param: customer:  # Specify an ID for the customer whose transactions you want to retrieve
         :param: terminal_id:  # Specify an ID for the terminal whose transactions you want to retrieve
         :param: amount:  # Specify an amount for the transactions you want to retrieve
         :param: status:  # Specify a status for the transactions you want to retrieve [success, failed, abandoned]
         :param: from_date:  # A timestamp from which to start listing transaction 2016-09-24T00:00:05.000Z, 2016-09-21
         :param: to_date:  # A timestamp at which to stop listing transaction 2016-09-24T00:00:05.000Z
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -195,94 +195,94 @@
             "customer": customer,
             "terminalid": terminal_id,
             "amount": amount,
             "status": status,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/transaction", params=params)
+        return self._get_request("/transaction", params=params)
 
-    async def verify_transaction(self, reference: str) -> Response:
+    def verify_transaction(self, reference: str) -> PayStackResponse:
         """
         Verify a transaction by reference
 
         :param: reference:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/transaction/verify/{reference}")
+        return self._get_request(f"/transaction/verify/{reference}")
 
-    async def fetch_transaction(self, transaction_id: int) -> Response:
+    def fetch_transaction(self, transaction_id: int) -> PayStackResponse:
         """
         Fetch details of a specific transaction
 
         :param: transaction_id:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/transaction/{transaction_id}")
+        return self._get_request(f"/transaction/{transaction_id}")
 
-    async def transaction_timeline(self, id_or_reference: str) -> Response:
+    def transaction_timeline(self, id_or_reference: str) -> PayStackResponse:
         """
         Get the timeline of a transaction
 
         :param: id_or_reference:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
-        return await self._get_request(f"/transaction/timeline/{id_or_reference}")
+        return self._get_request(f"/transaction/timeline/{id_or_reference}")
 
-    async def transaction_totals(
+    def transaction_totals(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Get totals of all transactions
 
         :param: per_page:
         :param: page:
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
             "perPage": per_page,
             "page": page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/transaction/totals", params=params)
+        return self._get_request("/transaction/totals", params=params)
 
-    async def export_transactions(
+    def export_transactions(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer: Optional[Union[int, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             amount: Optional[Union[int, None]] = None,
             status: Optional[Union[TransactionStatus, None]] = None,
             settled: Optional[Union[bool, None]] = True,
             settlement: Optional[Union[int, None]] = None,
             payment_page: Optional[Union[int, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Export transactions
 
         :param: per_page:
         :param: page:
         :param: customer:
         :param: currency:  # value = Currency.value.value
@@ -290,16 +290,16 @@
         :param: status:
         :param: settled:  # true or false
         :param: settlement:
         :param: payment_page:
         :param: from_date:  # 2016-09-24T00:00:05.000Z
         :param: to_date:  # 2016-09-24T00:00:05.000Z
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date and bool to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
         settled = self._convert_to_string(settled)
 
@@ -312,8 +312,8 @@
             "status": status,
             "settled": settled,
             "settlement": settlement,
             "payment_page": payment_page,
             "from": from_date,
             "to": to_date,
         }
-        return await self._get_request("/transaction/export", params=params)
+        return self._get_request("/transaction/export", params=params)
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/atransfer_recipients.py` & `paystackease-2.0.0/paystackease/apis/async_apis/atransfer_recipients.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Wrapper for Asynchronous Paystack Transfer Recipient APIs
 
 The Transfer Recipients API allows you to create and manage beneficiaries that you send money to.
 """
 
 from datetime import date
 from typing import Optional, Dict, List, Any, Union
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import Currency
 
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
 
-class AsyncTransferRecipientsClientAPI(AsyncPayStackBaseClientAPI):
+
+class AsyncTransferRecipientsClientAPI(AsyncRequestAPI):
     """
     Paystack Transfer Recipients API
     Reference: https://paystack.com/docs/api/transfer-recipient/
     """
 
     async def create_transfer_recipients(
             self,
@@ -23,115 +23,115 @@
             recipient_name: str,
             account_number: str,
             bank_code: str,
             description: Optional[Union[str, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             authorization_code: Optional[Union[str, None]] = None,
             metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Create a transfer recipient
 
         :param: recipient_type: The type of transfer recipient:[ nuban | ghipss | mobile_money | basa ]
         :param: recipient_name: The name of the transfer recipient according to their account registration
         :param: account_number: transfer recipient's account number.
                                 Required for all recipient types except authorization
         :param: bank_code: transfer recipient's bank code. Required for all recipient types except authorization
         :param: description:
         :param: currency: transfer recipient's currency. [Currency.value.value ]
         :param: authorization_code: transfer recipient's authorization code from previous transaction
         :param: metadata: transfer recipient's metadata
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "type": recipient_type,
             "name": recipient_name,
             "account_number": account_number,
             "bank_code": bank_code,
             "description": description,
             "currency": currency,
             "authorization_code": authorization_code,
             "metadata": metadata,
         }
         return await self._post_request("/transferrecipient", data=data)
 
-    async def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> Response:
+    async def bulk_create_transfer_recipient(self, batch: List[Dict[str, Any]]) -> PayStackResponse:
         """
         Create multiple transfer recipients in batches.
 
         :param: batch: A list of transfer recipient object
                         keys [ { type, name, account_number, bank_code, currency etc. }]
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"batch": batch}
         return await self._post_request("/transferrecipient/bulk", data=data)
 
     async def list_transfer_recipients(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List transfer recipients
 
         :param: per_page: The number of records to return per page.
         :param: page: The page number to retrieve.
         :param: from_date:
         :param: to_date:
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to strings
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {"perPage": per_page, "page": page, "from": from_date, "to": to_date}
         return await self._get_request("/transferrecipient", params=params)
 
-    async def fetch_transfer_recipient(self, id_or_code: str) -> Response:
+    async def fetch_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
         """
         Fetch details of a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request(f"/transferrecipient/{id_or_code}")
 
     async def update_transfer_recipient(
             self,
             id_or_code: str,
             recipient_name: str,
             recipient_email: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Update a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
         :param: recipient_name: The name of the transfer recipient
         :param: recipient_email: The email of the transfer recipient
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"name": recipient_name, "email": recipient_email}
         return await self._put_request(f"/transferrecipient/{id_or_code}", data=data)
 
-    async def delete_transfer_recipient(self, id_or_code: str) -> Response:
+    async def delete_transfer_recipient(self, id_or_code: str) -> PayStackResponse:
         """
         Delete a transfer recipient
 
         :param: id_or_code: The id or code of the transfer recipient
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._delete_request(f"/transferrecipient/{id_or_code}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/atransfers.py` & `paystackease-2.0.0/paystackease/apis/async_apis/atransfers.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,105 +3,104 @@
 
 The Transfers API allows you to automate sending money to your customers.
 """
 
 from datetime import date
 from typing import Optional, List, Dict, Any, Union
 
-from paystackease._utils import Response
-from paystackease.helpers.tool_kit import Currency
-from paystackease._abase import AsyncPayStackBaseClientAPI
+from paystackease.core import AsyncRequestAPI, PayStackResponse
+from paystackease.helpers import Currency
 
 
-class AsyncTransfersClientAPI(AsyncPayStackBaseClientAPI):
+class AsyncTransfersClientAPI(AsyncRequestAPI):
     """
     Paystack Transfers API
     Reference: https://paystack.com/docs/api/transfer/
     """
 
     async def initiate_transfer(
             self,
             transfer_source: str,
             amount: int,
             transfer_recipient: str,
             reason: Optional[Union[str, None]] = None,
             currency: Optional[Union[Currency, None]] = None,
             reference: Optional[Union[str, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Initiate a transfer. Upgrade your business to a Registered Business to use
 
         :param: transfer_source: Where should we transfer from? Only balance for now
         :param: amount: Amount to transfer in kobo if currency is NGN and pesewas if currency is GHS.
         :param: transfer_recipient: The code of the recipient
         :param: currency: The currency of the transfer
         :param: reason: The reason for the transfer
         :param: reference: If specified, the field should be a unique identifier (in lowercase) for the object.
                             Only -,_ and alphanumeric characters allowed.
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "source": transfer_source,
             "amount": amount,
             "recipient": transfer_recipient,
             "reason": reason,
             "currency": currency,
             "reference": reference,
         }
         return await self._post_request("/transfer", data=data)
 
-    async def finalize_transfer(self, transfer_code: str, otp: str) -> Response:
+    async def finalize_transfer(self, transfer_code: str, otp: str) -> PayStackResponse:
         """
         Finalize an initiated transfer
 
         :param: transfer_code: The code of the transfer to finalize
         :param: otp: The OTP sent to the business phone to verify transfer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"transfer_code": transfer_code, "otp": otp}
         return await self._post_request("/transfer/finalize_transfer", data=data)
 
     async def initiate_bulk_transfer(
             self, transfer_source: str, transfers: List[Dict[str, Any]]
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Batch multiple transfers in a single request
 
         :param: transfer_source: Where should we transfer from? Only balance for now
         :param: transfers: A list of transfer objects keys [ { amount | recipient | reference | reason } ]
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"source": transfer_source, "transfers": transfers}
         return await self._post_request("/transfer/bulk", data=data)
 
     async def list_transfers(
             self,
             per_page: Optional[Union[int, None]] = 50,
             page: Optional[Union[int, None]] = 1,
             customer_id: Optional[Union[str, None]] = None,
             from_date: Optional[Union[date, None]] = None,
             to_date: Optional[Union[date, None]] = None,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         List transfers
 
         :param: per_page: The number of records to return per page.
         :param: page: The page number to retrieve.
         :param: customer_id
         :param: from_date
         :param: to_date
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
 
         # convert date to string
         from_date = self._convert_to_string(from_date)
         to_date = self._convert_to_string(to_date)
 
         params = {
@@ -109,28 +108,28 @@
             "page": page,
             "customer": customer_id,
             "from": from_date,
             "to": to_date,
         }
         return await self._get_request("/transfer", params=params)
 
-    async def fetch_transfer(self, id_or_code: str) -> Response:
+    async def fetch_transfer(self, id_or_code: str) -> PayStackResponse:
         """
         Get details of a transfer
 
         :param: id_or_code: The id or code of the transfer
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request(f"/transfer/{id_or_code}")
 
-    async def verify_transfer(self, reference: str) -> Response:
+    async def verify_transfer(self, reference: str) -> PayStackResponse:
         """
         Verify a transfer
 
         :param: reference: The reference of the transfer to verify
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._post_request(f"/transfer/verify/{reference}")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/atransfers_control.py` & `paystackease-2.0.0/paystackease/apis/async_apis/atransfers_control.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,78 @@
 """
 Wrapper for Asynchronous Paystack Transfer Control APIs
 
 The Transfers Control API allows you manage settings of your transfers.
 """
 
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
+from paystackease.core import AsyncRequestAPI, PayStackResponse
 
 
-class AsyncTransferControlClientAPI(AsyncPayStackBaseClientAPI):
+class AsyncTransferControlClientAPI(AsyncRequestAPI):
     """
     Paystack Transfers Control API
     Reference: https://paystack.com/docs/api/transfer-control/
     """
 
-    async def check_balance(self) -> Response:
+    async def check_balance(self) -> PayStackResponse:
         """
         Get the available balance
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request("/balance")
 
-    async def fetch_balance_ledger(self) -> Response:
+    async def fetch_balance_ledger(self) -> PayStackResponse:
         """
         Fetch all pay-ins and pay-outs that occurred on your integration
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request("/balance/ledger")
 
-    async def resend_otp(self, transfer_code: str, reason: str) -> Response:
+    async def resend_otp(self, transfer_code: str, reason: str) -> PayStackResponse:
         """
         Generates a new OTP and sends to customer in the event
         they are having trouble receiving one.
 
         :param: transfer_code: The code of the transfer to finalize
         :param: reason: Either resend_otp or transfer as the value of this field
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"transfer_code": transfer_code, "reason": reason}
         return await self._post_request("/transfer/resend_otp", data=data)
 
-    async def disable_otp(self) -> Response:
+    async def disable_otp(self) -> PayStackResponse:
         """
         This is used in the event that you want to be able to
          complete transfers programmatically without use of OTPs
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._post_request("/transfer/disable_otp")
 
-    async def finalize_disable_otp(self, otp: str) -> Response:
+    async def finalize_disable_otp(self, otp: str) -> PayStackResponse:
         """
         Finalize the request to disable OTP on your transfers.
 
         :param: otp: The OTP sent to the business phone to verify disabling of OTP
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {"otp": otp}
         return await self._post_request("/transfer/disable_otp_finalize", data=data)
 
-    async def enable_otp(self) -> Response:
+    async def enable_otp(self) -> PayStackResponse:
         """
         This is used in the event that you want to stop
         being able to complete transfers programmatically with use of OTPs
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._post_request("/transfer/enable_otp")
```

### Comparing `paystackease-1.0.0/paystackease/async_apis/averification.py` & `paystackease-2.0.0/paystackease/apis/async_apis/averification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 """
 Wrapper for Asynchronous Paystack Verification APIs
 
 The Verification API allows you to perform KYC processes.
 """
 
-from paystackease._abase import AsyncPayStackBaseClientAPI
-from paystackease._utils import Response
+from paystackease.core import AsyncRequestAPI, PayStackResponse
 
 
-class AsyncVerificationClientAPI(AsyncPayStackBaseClientAPI):
+class AsyncVerificationClientAPI(AsyncRequestAPI):
     """
     Paystack Verification API
     Reference: https://paystack.com/docs/api/verification/
     """
 
-    async def resolve_account(self, account_number: str, bank_code: str) -> Response:
+    async def resolve_account(self, account_number: str, bank_code: str) -> PayStackResponse:
         """
         Confirm an account belongs to the right customer.
         This feature is available to business in Nigeria and Ghana.
 
         :param: account_number: The account number to verify
         :param: bank_code: The bank code to verify
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         params = {"account_number": account_number, "bank_code": bank_code}
         return await self._get_request("/bank/resolve", params=params)
 
     async def validate_account(
             self,
             account_name: str,
             account_number: str,
             account_type: str,
             bank_code: str,
             country_code: str,
             document_type: str,
             document_number: str,
-    ) -> Response:
+    ) -> PayStackResponse:
         """
         Confirm the authenticity of a customer's account number before sending money.
         This feature is only available to businesses in South Africa.
 
         :param: account_name: The account name to validate: first and last name
         :param: account_number: The account number to validate
         :param: account_type: The account type to validate: personal or business
         :param: bank_code: The bank code to validate
         :param: country_code: The country code to validate
         :param: document_type: The customer's mode of identity:
                                 identityNumber, passportNumber or businessRegistrationNumber
         :param: document_number: The customer's document number
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         data = {
             "account_name": account_name,
             "account_number": account_number,
             "account_type": account_type,
             "bank_code": bank_code,
             "country_code": country_code,
             "document_type": document_type,
             "document_number": document_number,
         }
         return await self._post_request("/bank/validate", data=data)
 
-    async def resolve_card_bin(self, bin_code: str) -> Response:
+    async def resolve_card_bin(self, bin_code: str) -> PayStackResponse:
         """
         Resolve a card BIN
 
         :param: bin_code: First 6 characters of card
 
-        :return: The response from the API
-        :rtype: Response object
+        :return: The PayStackResponse from the API
+        :rtype: PayStackResponse object
         """
         return await self._get_request(f"/decision/bin/{bin_code}")
```

### Comparing `paystackease-1.0.0/paystackease/helpers/__init__.py` & `paystackease-2.0.0/paystackease/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `paystackease-1.0.0/paystackease/helpers/convert.py` & `paystackease-2.0.0/paystackease/helpers/convert.py`

 * *Files identical despite different names*

### Comparing `paystackease-1.0.0/paystackease/helpers/tool_kit.py` & `paystackease-2.0.0/paystackease/helpers/tool_kit.py`

 * *Files identical despite different names*

### Comparing `paystackease-1.0.0/paystackease/paystack.py` & `paystackease-2.0.0/paystackease/paystack.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     transaction_splits,
     transactions,
     transfer_recipients,
     transfers,
     transfers_control,
     verification,
 )
-from paystackease._base import PayStackBaseClientAPI
+from paystackease.core import SyncRequestAPI
 
 
-class PayStackBase(PayStackBaseClientAPI):
+class PayStackBase(SyncRequestAPI):
     """PayStackBase acts as a wrapper around various client APIs to
     interact with the PayStack API
     """
 
     # pylint: disable=too-many-instance-attributes
     def __init__(self, secret_key=None):
         super().__init__(secret_key)
```

### Comparing `paystackease-1.0.0/pyproject.toml` & `paystackease-2.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 [tool.poetry]
 name = "paystackease"
-version = "1.0.0"
-description = "This is a simple api wrapper for paystack"
+version = "2.0.0"
+description = "This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs."
 authors = ["Peter Mbachu <doublep098@gmail.com>"]
-maintainers = [
-    "petermbachu.bincom <petermbachu.bincom@gmail.com>",
-]
+maintainers = []
 license = "MIT"
 readme = "README.md"
 keywords = ["paystack", "paystackease", "python", "api", "payment integration"]
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `paystackease-1.0.0/PKG-INFO` & `paystackease-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: paystackease
-Version: 1.0.0
-Summary: This is a simple api wrapper for paystack
+Version: 2.0.0
+Summary: This is a simple api wrapper that implements both asynchronous and synchronous http requests to interact with Paystack APIs.
 License: MIT
 Keywords: paystack,paystackease,python,api,payment integration
 Author: Peter Mbachu
 Author-email: doublep098@gmail.com
-Maintainer: petermbachu.bincom
-Maintainer-email: petermbachu.bincom@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -27,17 +25,17 @@
 Project-URL: Documentation, https://paystackease.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/cla-bit/PayStackEase
 Project-URL: Source Code, https://github.com/cla-bit/PayStackEase
 Description-Content-Type: text/markdown
 
 # PayStackEase Library  
 
-------
+--------------
 
-![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
+![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue) ![License](https://img.shields.io/pypi/l/paystackease.svg) ![pypi](https://img.shields.io/pypi/v/paystackease.svg)
 
 
 **PayStackEase API Library**  is a Python library that simplifies interacting with the Paystack API. 
 It provides both asynchronous and synchronous wrappers for various Paystack functionalities, 
 making it easier to integrate payment processing into your Python projects.
 
 > 📝: Read more on paystack api documentation: [Paystack API DOCUMENTATION](https://paystack.com/docs/api/)
@@ -67,15 +65,15 @@
        ```
     * Activate the virtual environment
 
         ```
             <environment_name>\Scripts\activate
        ```
 
-2. For Unix/MacOS
+2. For Unix/macOS
 
     * Create virtual environment
 
         ```
             python3 -m venv <environment_name>
        ```
     * Activate the virtual environment
@@ -102,24 +100,24 @@
 > poetry add paystackease
 
 
 ## If you want to download the sdist packages directly:
 
 Download the wheel distribution file and install using pip
 
->  pip install paystackease-1.0.0-py3-none-any.whl 
+>  pip install paystackease-2.0.0-py3-none-any.whl 
 
 Download the source distribution file, and install using pip
 
-> pip install paystackease-1.0.0.tar.gz 
+> pip install paystackease-2.0.0.tar.gz 
 
 
 ## To get a development version of paystackease
 
-Clone from the ``dev`` branch github repository, unzip and install:
+Clone from the ``dev`` branch GitHub repository, unzip and install:
 
 > git clone -b dev https://github.com/cla-bit/PayStackEase.git
 
 > cd PayStackEase
 
 > pip install paystackease
 
@@ -154,15 +152,15 @@
     create_transaction = paystack_client.transactions.initialize(
         email="johndoe@email.com",
         amount=10000000)
     
     print(f"Transaction Created: {create_transaction}")
 ```
 
-> ✅: **Good**: You can check your Paystack account, go to the Transaction page and you will see the transaction just created.
+> ✅: **Good**: You can check your Paystack account, go to the Transaction page, and you will see the transaction just created.
 
 
 # Other Tools
 Similar to calling the PayStackBase, you can also call other tools to make your work easy. For example:
 
 * ### Account Type
 ```apacheconf
```

