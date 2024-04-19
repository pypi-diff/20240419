# Comparing `tmp/flagright-1.5.1.tar.gz` & `tmp/flagright-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagright-1.5.1.tar", max compression
+gzip compressed data, was "flagright-1.5.2.tar", max compression
```

## Comparing `flagright-1.5.1.tar` & `flagright-1.5.2.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0      829 2024-04-17 10:00:50.395231 flagright-1.5.1/README.md
--rw-r--r--   0        0        0      404 2024-04-17 10:00:50.395231 flagright-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     9667 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/__init__.py
--rw-r--r--   0        0        0     3441 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/client.py
--rw-r--r--   0        0        0      519 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/core/api_error.py
--rw-r--r--   0        0        0     1078 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      168 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/environment.py
--rw-r--r--   0        0        0      358 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/errors/forbidden_error.py
--rw-r--r--   0        0        0      253 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      250 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/py.typed
--rw-r--r--   0        0        0      647 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/resources/business_user_events/__init__.py
--rw-r--r--   0        0        0    70170 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/resources/business_user_events/client.py
--rw-r--r--   0        0        0      155 2024-04-17 10:00:50.395231 flagright-1.5.1/src/flagright/resources/business_users/__init__.py
--rw-r--r--   0        0        0    38466 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/business_users/client.py
--rw-r--r--   0        0        0      180 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/business_users/types/__init__.py
--rw-r--r--   0        0        0      910 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/business_users/types/business_users_create_response.py
--rw-r--r--   0        0        0       65 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/consumer_user_events/__init__.py
--rw-r--r--   0        0        0    23686 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/consumer_user_events/client.py
--rw-r--r--   0        0        0      155 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/consumer_users/__init__.py
--rw-r--r--   0        0        0    20900 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/consumer_users/client.py
--rw-r--r--   0        0        0      180 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/consumer_users/types/__init__.py
--rw-r--r--   0        0        0      910 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/consumer_users/types/consumer_users_create_response.py
--rw-r--r--   0        0        0       65 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/transaction_events/__init__.py
--rw-r--r--   0        0        0    16377 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/transaction_events/client.py
--rw-r--r--   0        0        0      153 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/transactions/__init__.py
--rw-r--r--   0        0        0    19718 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/transactions/client.py
--rw-r--r--   0        0        0      176 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/transactions/types/__init__.py
--rw-r--r--   0        0        0      927 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/resources/transactions/types/transactions_verify_response.py
--rw-r--r--   0        0        0    12255 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/__init__.py
--rw-r--r--   0        0        0     1947 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/ach_details.py
--rw-r--r--   0        0        0      143 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/ach_payment_method.py
--rw-r--r--   0        0        0     1167 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/acquisition_channel.py
--rw-r--r--   0        0        0     1637 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/address.py
--rw-r--r--   0        0        0     1667 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/alert_closed_details.py
--rw-r--r--   0        0        0     1160 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/amount.py
--rw-r--r--   0        0        0      448 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/boolean_string.py
--rw-r--r--   0        0        0     3230 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business.py
--rw-r--r--   0        0        0     1296 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_base.py
--rw-r--r--   0        0        0     1080 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_entity_link.py
--rw-r--r--   0        0        0     3090 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_optional.py
--rw-r--r--   0        0        0     3143 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_optional_saved_payment_details_item.py
--rw-r--r--   0        0        0     1658 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_user_event.py
--rw-r--r--   0        0        0     1282 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_user_segment.py
--rw-r--r--   0        0        0     1546 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_users_response.py
--rw-r--r--   0        0        0     1470 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/business_with_rules_result.py
--rw-r--r--   0        0        0     1247 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/card_brand.py
--rw-r--r--   0        0        0     3079 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/card_details.py
--rw-r--r--   0        0        0      920 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/card_expiry.py
--rw-r--r--   0        0        0      661 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/card_funding.py
--rw-r--r--   0        0        0     1200 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/card_merchant_details.py
--rw-r--r--   0        0        0      145 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/card_payment_method.py
--rw-r--r--   0        0        0      497 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/card_type.py
--rw-r--r--   0        0        0     1357 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/case_closed_details.py
--rw-r--r--   0        0        0     2130 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/case_management_event.py
--rw-r--r--   0        0        0      558 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/case_management_event_case_status.py
--rw-r--r--   0        0        0     1174 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/case_management_event_case_status_reason.py
--rw-r--r--   0        0        0     1169 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/case_opened_details.py
--rw-r--r--   0        0        0     1133 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/check_delivery_status.py
--rw-r--r--   0        0        0     1608 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/check_details.py
--rw-r--r--   0        0        0      147 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/check_payment_method.py
--rw-r--r--   0        0        0     1420 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/company_financial_details.py
--rw-r--r--   0        0        0     2026 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/company_general_details.py
--rw-r--r--   0        0        0     1878 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/company_registration_details.py
--rw-r--r--   0        0        0     1272 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/consumer_name.py
--rw-r--r--   0        0        0     1646 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/consumer_user_event.py
--rw-r--r--   0        0        0      511 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/consumer_user_segment.py
--rw-r--r--   0        0        0     1546 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/consumer_users_response.py
--rw-r--r--   0        0        0     1731 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/contact_details.py
--rw-r--r--   0        0        0    29271 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/country_code.py
--rw-r--r--   0        0        0    56920 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/currency_code.py
--rw-r--r--   0        0        0     1066 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/date.py
--rw-r--r--   0        0        0     2967 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/device_data.py
--rw-r--r--   0        0        0       79 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/email_id.py
--rw-r--r--   0        0        0     1685 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/employment_status.py
--rw-r--r--   0        0        0     1771 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/executed_rules_result.py
--rw-r--r--   0        0        0     1426 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/failed_rules_result.py
--rw-r--r--   0        0        0     1049 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/false_positive_details.py
--rw-r--r--   0        0        0      584 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/gender.py
--rw-r--r--   0        0        0      175 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/general_bank_account_payment_method.py
--rw-r--r--   0        0        0     2340 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/generic_bank_account_details.py
--rw-r--r--   0        0        0     1709 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/hit_rules_details.py
--rw-r--r--   0        0        0     2249 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/iban_details.py
--rw-r--r--   0        0        0      145 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/iban_payment_method.py
--rw-r--r--   0        0        0     1575 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/kyc_status.py
--rw-r--r--   0        0        0     1078 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/kyc_status_details.py
--rw-r--r--   0        0        0     2153 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/legal_document.py
--rw-r--r--   0        0        0     1939 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/legal_entity.py
--rw-r--r--   0        0        0     1115 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_data.py
--rw-r--r--   0        0        0     1162 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_existed.py
--rw-r--r--   0        0        0     1275 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_header.py
--rw-r--r--   0        0        0      958 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_item.py
--rw-r--r--   0        0        0      127 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_key_metadata.py
--rw-r--r--   0        0        0     1084 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_metadata.py
--rw-r--r--   0        0        0     2152 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_subtype.py
--rw-r--r--   0        0        0      697 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/list_type.py
--rw-r--r--   0        0        0     1006 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/mcc_details.py
--rw-r--r--   0        0        0     1573 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/mpesa_details.py
--rw-r--r--   0        0        0      147 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/mpesa_payment_method.py
--rw-r--r--   0        0        0     1312 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/mpesa_transaction_type.py
--rw-r--r--   0        0        0     1465 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/payment_method.py
--rw-r--r--   0        0        0     1029 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/pep_status.py
--rw-r--r--   0        0        0     1781 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/person.py
--rw-r--r--   0        0        0      884 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/risk_level.py
--rw-r--r--   0        0        0      921 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/rule_action.py
--rw-r--r--   0        0        0     1121 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/rule_failure_exception.py
--rw-r--r--   0        0        0      497 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/rule_hit_direction.py
--rw-r--r--   0        0        0     1562 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/rule_hit_meta.py
--rw-r--r--   0        0        0     2235 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/rule_labels.py
--rw-r--r--   0        0        0      735 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/rule_nature.py
--rw-r--r--   0        0        0     1293 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/rules_results.py
--rw-r--r--   0        0        0     1172 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/sanctions_details.py
--rw-r--r--   0        0        0     1694 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/sanctions_details_entity_type.py
--rw-r--r--   0        0        0     2433 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/source_of_funds.py
--rw-r--r--   0        0        0     2071 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/swift_details.py
--rw-r--r--   0        0        0      147 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/swift_payment_method.py
--rw-r--r--   0        0        0     1156 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/tag.py
--rw-r--r--   0        0        0      907 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction.py
--rw-r--r--   0        0        0     1291 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_amount_details.py
--rw-r--r--   0        0        0     1028 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_amount_limit.py
--rw-r--r--   0        0        0     1616 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_base.py
--rw-r--r--   0        0        0      996 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_count_limit.py
--rw-r--r--   0        0        0     1923 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_event.py
--rw-r--r--   0        0        0     1260 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_event_monitoring_result.py
--rw-r--r--   0        0        0     1408 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_limit.py
--rw-r--r--   0        0        0     1947 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_limits.py
--rw-r--r--   0        0        0     1686 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_limits_payment_method_limits.py
--rw-r--r--   0        0        0     1332 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_monitoring_result.py
--rw-r--r--   0        0        0     1122 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_risk_scoring_result.py
--rw-r--r--   0        0        0     1669 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_state.py
--rw-r--r--   0        0        0     1100 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_status_details.py
--rw-r--r--   0        0        0     1140 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_type.py
--rw-r--r--   0        0        0     3339 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_updatable.py
--rw-r--r--   0        0        0     3257 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_updatable_destination_payment_details.py
--rw-r--r--   0        0        0     3162 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_updatable_origin_payment_details.py
--rw-r--r--   0        0        0     1534 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/transaction_with_rules_result.py
--rw-r--r--   0        0        0     1635 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/upi_details.py
--rw-r--r--   0        0        0      143 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/upi_payment_method.py
--rw-r--r--   0        0        0      899 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user.py
--rw-r--r--   0        0        0     1141 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_base.py
--rw-r--r--   0        0        0     1476 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_details.py
--rw-r--r--   0        0        0     3056 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_optional.py
--rw-r--r--   0        0        0      540 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_registration_status.py
--rw-r--r--   0        0        0     1279 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_risk_score_details.py
--rw-r--r--   0        0        0     1232 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_state.py
--rw-r--r--   0        0        0     1060 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_state_details.py
--rw-r--r--   0        0        0     1459 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/user_with_rules_result.py
--rw-r--r--   0        0        0     2286 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/wallet_details.py
--rw-r--r--   0        0        0     4132 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/wallet_details_network.py
--rw-r--r--   0        0        0      149 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/wallet_payment_method.py
--rw-r--r--   0        0        0      987 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/webhook_event.py
--rw-r--r--   0        0        0     1387 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/webhook_event_base.py
--rw-r--r--   0        0        0      562 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/webhook_event_base_triggered_by.py
--rw-r--r--   0        0        0      578 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/webhook_event_data.py
--rw-r--r--   0        0        0     1201 2024-04-17 10:00:50.399231 flagright-1.5.1/src/flagright/types/webhook_event_type.py
--rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 flagright-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      829 2024-04-19 15:19:49.417884 flagright-1.5.2/README.md
+-rw-r--r--   0        0        0      404 2024-04-19 15:19:49.417884 flagright-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9653 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/client.py
+-rw-r--r--   0        0        0      519 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/api_error.py
+-rw-r--r--   0        0        0     1078 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      168 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/environment.py
+-rw-r--r--   0        0        0      358 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/forbidden_error.py
+-rw-r--r--   0        0        0      253 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      250 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/py.typed
+-rw-r--r--   0        0        0      647 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_user_events/__init__.py
+-rw-r--r--   0        0        0    70170 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_user_events/client.py
+-rw-r--r--   0        0        0      155 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/__init__.py
+-rw-r--r--   0        0        0    38466 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/client.py
+-rw-r--r--   0        0        0      180 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/types/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/business_users/types/business_users_create_response.py
+-rw-r--r--   0        0        0       65 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_user_events/__init__.py
+-rw-r--r--   0        0        0    23686 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_user_events/client.py
+-rw-r--r--   0        0        0      155 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/__init__.py
+-rw-r--r--   0        0        0    20900 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/client.py
+-rw-r--r--   0        0        0      180 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/types/__init__.py
+-rw-r--r--   0        0        0      910 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/consumer_users/types/consumer_users_create_response.py
+-rw-r--r--   0        0        0       65 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transaction_events/__init__.py
+-rw-r--r--   0        0        0    16377 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transaction_events/client.py
+-rw-r--r--   0        0        0      153 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    19718 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/client.py
+-rw-r--r--   0        0        0      176 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/types/__init__.py
+-rw-r--r--   0        0        0      927 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/resources/transactions/types/transactions_verify_response.py
+-rw-r--r--   0        0        0    12233 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/ach_details.py
+-rw-r--r--   0        0        0      143 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/ach_payment_method.py
+-rw-r--r--   0        0        0     1167 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/acquisition_channel.py
+-rw-r--r--   0        0        0     1637 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/address.py
+-rw-r--r--   0        0        0     1667 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/alert_closed_details.py
+-rw-r--r--   0        0        0     1160 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/amount.py
+-rw-r--r--   0        0        0      448 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/boolean_string.py
+-rw-r--r--   0        0        0     3230 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business.py
+-rw-r--r--   0        0        0     1296 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_base.py
+-rw-r--r--   0        0        0     1080 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_entity_link.py
+-rw-r--r--   0        0        0     3090 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_optional.py
+-rw-r--r--   0        0        0     3143 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_optional_saved_payment_details_item.py
+-rw-r--r--   0        0        0     1658 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_user_event.py
+-rw-r--r--   0        0        0     1282 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_user_segment.py
+-rw-r--r--   0        0        0     1546 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_users_response.py
+-rw-r--r--   0        0        0     1470 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/business_with_rules_result.py
+-rw-r--r--   0        0        0     1247 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_brand.py
+-rw-r--r--   0        0        0     3079 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_details.py
+-rw-r--r--   0        0        0      920 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_expiry.py
+-rw-r--r--   0        0        0      661 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_funding.py
+-rw-r--r--   0        0        0     1200 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_merchant_details.py
+-rw-r--r--   0        0        0      145 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_payment_method.py
+-rw-r--r--   0        0        0      497 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/card_type.py
+-rw-r--r--   0        0        0     1357 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_closed_details.py
+-rw-r--r--   0        0        0     2130 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_management_event.py
+-rw-r--r--   0        0        0      558 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_management_event_case_status.py
+-rw-r--r--   0        0        0     1174 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_management_event_case_status_reason.py
+-rw-r--r--   0        0        0     1169 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/case_opened_details.py
+-rw-r--r--   0        0        0     1133 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/check_delivery_status.py
+-rw-r--r--   0        0        0     1608 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/check_details.py
+-rw-r--r--   0        0        0      147 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/check_payment_method.py
+-rw-r--r--   0        0        0     1420 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/company_financial_details.py
+-rw-r--r--   0        0        0     2026 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/company_general_details.py
+-rw-r--r--   0        0        0     1878 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/company_registration_details.py
+-rw-r--r--   0        0        0     1272 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_name.py
+-rw-r--r--   0        0        0     1646 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_user_event.py
+-rw-r--r--   0        0        0      511 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_user_segment.py
+-rw-r--r--   0        0        0     1546 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/consumer_users_response.py
+-rw-r--r--   0        0        0     1731 2024-04-19 15:19:49.417884 flagright-1.5.2/src/flagright/types/contact_details.py
+-rw-r--r--   0        0        0    29271 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/country_code.py
+-rw-r--r--   0        0        0    56920 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/currency_code.py
+-rw-r--r--   0        0        0     1066 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/date.py
+-rw-r--r--   0        0        0     2967 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/device_data.py
+-rw-r--r--   0        0        0       79 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/email_id.py
+-rw-r--r--   0        0        0     1685 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/employment_status.py
+-rw-r--r--   0        0        0     1771 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/executed_rules_result.py
+-rw-r--r--   0        0        0     1426 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/failed_rules_result.py
+-rw-r--r--   0        0        0     1049 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/false_positive_details.py
+-rw-r--r--   0        0        0      584 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/gender.py
+-rw-r--r--   0        0        0      175 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/general_bank_account_payment_method.py
+-rw-r--r--   0        0        0     2340 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/generic_bank_account_details.py
+-rw-r--r--   0        0        0     1709 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/hit_rules_details.py
+-rw-r--r--   0        0        0     2249 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/iban_details.py
+-rw-r--r--   0        0        0      145 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/iban_payment_method.py
+-rw-r--r--   0        0        0     1575 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/kyc_status.py
+-rw-r--r--   0        0        0     1078 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/kyc_status_details.py
+-rw-r--r--   0        0        0     2153 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/legal_document.py
+-rw-r--r--   0        0        0     1939 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/legal_entity.py
+-rw-r--r--   0        0        0     1115 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_data.py
+-rw-r--r--   0        0        0     1162 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_existed.py
+-rw-r--r--   0        0        0     1275 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_header.py
+-rw-r--r--   0        0        0      958 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_item.py
+-rw-r--r--   0        0        0      127 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_key_metadata.py
+-rw-r--r--   0        0        0     1084 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_metadata.py
+-rw-r--r--   0        0        0     2152 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_subtype.py
+-rw-r--r--   0        0        0      697 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/list_type.py
+-rw-r--r--   0        0        0     1006 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mcc_details.py
+-rw-r--r--   0        0        0     1573 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mpesa_details.py
+-rw-r--r--   0        0        0      147 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mpesa_payment_method.py
+-rw-r--r--   0        0        0     1312 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/mpesa_transaction_type.py
+-rw-r--r--   0        0        0     1465 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/payment_method.py
+-rw-r--r--   0        0        0     1029 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/pep_status.py
+-rw-r--r--   0        0        0     1781 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/person.py
+-rw-r--r--   0        0        0      884 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/risk_level.py
+-rw-r--r--   0        0        0      921 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_action.py
+-rw-r--r--   0        0        0     1121 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_failure_exception.py
+-rw-r--r--   0        0        0      497 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_hit_direction.py
+-rw-r--r--   0        0        0     1562 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_hit_meta.py
+-rw-r--r--   0        0        0     2235 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_labels.py
+-rw-r--r--   0        0        0      735 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rule_nature.py
+-rw-r--r--   0        0        0     1293 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/rules_results.py
+-rw-r--r--   0        0        0     1172 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/sanctions_details.py
+-rw-r--r--   0        0        0     1694 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/sanctions_details_entity_type.py
+-rw-r--r--   0        0        0     2433 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/source_of_funds.py
+-rw-r--r--   0        0        0     2071 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/swift_details.py
+-rw-r--r--   0        0        0      147 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/swift_payment_method.py
+-rw-r--r--   0        0        0     1156 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/tag.py
+-rw-r--r--   0        0        0      907 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction.py
+-rw-r--r--   0        0        0     1291 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_amount_details.py
+-rw-r--r--   0        0        0     1028 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_amount_limit.py
+-rw-r--r--   0        0        0     1616 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_base.py
+-rw-r--r--   0        0        0      996 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_count_limit.py
+-rw-r--r--   0        0        0     1923 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_event.py
+-rw-r--r--   0        0        0     1260 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_event_monitoring_result.py
+-rw-r--r--   0        0        0     1408 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_limit.py
+-rw-r--r--   0        0        0     1947 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_limits.py
+-rw-r--r--   0        0        0     1686 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_limits_payment_method_limits.py
+-rw-r--r--   0        0        0     1332 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_monitoring_result.py
+-rw-r--r--   0        0        0     1122 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_risk_scoring_result.py
+-rw-r--r--   0        0        0     1669 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_state.py
+-rw-r--r--   0        0        0     1100 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_status_details.py
+-rw-r--r--   0        0        0     1140 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_type.py
+-rw-r--r--   0        0        0     3339 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_updatable.py
+-rw-r--r--   0        0        0     3257 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_updatable_destination_payment_details.py
+-rw-r--r--   0        0        0     3162 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_updatable_origin_payment_details.py
+-rw-r--r--   0        0        0     1534 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/transaction_with_rules_result.py
+-rw-r--r--   0        0        0     1635 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/upi_details.py
+-rw-r--r--   0        0        0      143 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/upi_payment_method.py
+-rw-r--r--   0        0        0      899 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user.py
+-rw-r--r--   0        0        0     1141 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_base.py
+-rw-r--r--   0        0        0     1476 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_details.py
+-rw-r--r--   0        0        0     3056 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_optional.py
+-rw-r--r--   0        0        0      540 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_registration_status.py
+-rw-r--r--   0        0        0     1279 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_risk_score_details.py
+-rw-r--r--   0        0        0     1232 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_state.py
+-rw-r--r--   0        0        0     1060 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_state_details.py
+-rw-r--r--   0        0        0     1459 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/user_with_rules_result.py
+-rw-r--r--   0        0        0     2210 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/wallet_details.py
+-rw-r--r--   0        0        0     3957 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/wallet_network.py
+-rw-r--r--   0        0        0      149 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/wallet_payment_method.py
+-rw-r--r--   0        0        0      987 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event.py
+-rw-r--r--   0        0        0     1387 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_base.py
+-rw-r--r--   0        0        0      562 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_base_triggered_by.py
+-rw-r--r--   0        0        0      578 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_data.py
+-rw-r--r--   0        0        0     1201 2024-04-19 15:19:49.421884 flagright-1.5.2/src/flagright/types/webhook_event_type.py
+-rw-r--r--   0        0        0     1335 1970-01-01 00:00:00.000000 flagright-1.5.2/PKG-INFO
```

### Comparing `flagright-1.5.1/README.md` & `flagright-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/__init__.py` & `flagright-1.5.2/src/flagright/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     UserOptional,
     UserRegistrationStatus,
     UserRiskScoreDetails,
     UserState,
     UserStateDetails,
     UserWithRulesResult,
     WalletDetails,
-    WalletDetailsNetwork,
+    WalletNetwork,
     WalletPaymentMethod,
     WebhookEvent,
     WebhookEventBase,
     WebhookEventBaseTriggeredBy,
     WebhookEventData,
     WebhookEventType,
 )
@@ -318,15 +318,15 @@
     "UserOptional",
     "UserRegistrationStatus",
     "UserRiskScoreDetails",
     "UserState",
     "UserStateDetails",
     "UserWithRulesResult",
     "WalletDetails",
-    "WalletDetailsNetwork",
+    "WalletNetwork",
     "WalletPaymentMethod",
     "WebhookEvent",
     "WebhookEventBase",
     "WebhookEventBaseTriggeredBy",
     "WebhookEventData",
     "WebhookEventType",
     "business_user_events",
```

### Comparing `flagright-1.5.1/src/flagright/client.py` & `flagright-1.5.2/src/flagright/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/core/__init__.py` & `flagright-1.5.2/src/flagright/core/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/core/client_wrapper.py` & `flagright-1.5.2/src/flagright/core/client_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "flagright",
-            "X-Fern-SDK-Version": "1.5.1",
+            "X-Fern-SDK-Version": "1.5.2",
         }
         headers["x-api-key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `flagright-1.5.1/src/flagright/core/datetime_utils.py` & `flagright-1.5.2/src/flagright/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/core/jsonable_encoder.py` & `flagright-1.5.2/src/flagright/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/__init__.py` & `flagright-1.5.2/src/flagright/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/business_user_events/client.py` & `flagright-1.5.2/src/flagright/resources/business_user_events/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/business_users/client.py` & `flagright-1.5.2/src/flagright/resources/business_users/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/business_users/types/business_users_create_response.py` & `flagright-1.5.2/src/flagright/resources/business_users/types/business_users_create_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/consumer_user_events/client.py` & `flagright-1.5.2/src/flagright/resources/consumer_user_events/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/consumer_users/client.py` & `flagright-1.5.2/src/flagright/resources/consumer_users/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/consumer_users/types/consumer_users_create_response.py` & `flagright-1.5.2/src/flagright/resources/consumer_users/types/consumer_users_create_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/transaction_events/client.py` & `flagright-1.5.2/src/flagright/resources/transaction_events/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/transactions/client.py` & `flagright-1.5.2/src/flagright/resources/transactions/client.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/resources/transactions/types/transactions_verify_response.py` & `flagright-1.5.2/src/flagright/resources/transactions/types/transactions_verify_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/__init__.py` & `flagright-1.5.2/src/flagright/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 from .user_optional import UserOptional
 from .user_registration_status import UserRegistrationStatus
 from .user_risk_score_details import UserRiskScoreDetails
 from .user_state import UserState
 from .user_state_details import UserStateDetails
 from .user_with_rules_result import UserWithRulesResult
 from .wallet_details import WalletDetails
-from .wallet_details_network import WalletDetailsNetwork
+from .wallet_network import WalletNetwork
 from .wallet_payment_method import WalletPaymentMethod
 from .webhook_event import WebhookEvent
 from .webhook_event_base import WebhookEventBase
 from .webhook_event_base_triggered_by import WebhookEventBaseTriggeredBy
 from .webhook_event_data import WebhookEventData
 from .webhook_event_type import WebhookEventType
 
@@ -301,15 +301,15 @@
     "UserOptional",
     "UserRegistrationStatus",
     "UserRiskScoreDetails",
     "UserState",
     "UserStateDetails",
     "UserWithRulesResult",
     "WalletDetails",
-    "WalletDetailsNetwork",
+    "WalletNetwork",
     "WalletPaymentMethod",
     "WebhookEvent",
     "WebhookEventBase",
     "WebhookEventBaseTriggeredBy",
     "WebhookEventData",
     "WebhookEventType",
 ]
```

### Comparing `flagright-1.5.1/src/flagright/types/ach_details.py` & `flagright-1.5.2/src/flagright/types/ach_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/acquisition_channel.py` & `flagright-1.5.2/src/flagright/types/acquisition_channel.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/address.py` & `flagright-1.5.2/src/flagright/types/address.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/alert_closed_details.py` & `flagright-1.5.2/src/flagright/types/alert_closed_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/amount.py` & `flagright-1.5.2/src/flagright/types/amount.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business.py` & `flagright-1.5.2/src/flagright/types/business.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_base.py` & `flagright-1.5.2/src/flagright/types/business_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_entity_link.py` & `flagright-1.5.2/src/flagright/types/business_entity_link.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_optional.py` & `flagright-1.5.2/src/flagright/types/business_optional.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_optional_saved_payment_details_item.py` & `flagright-1.5.2/src/flagright/types/business_optional_saved_payment_details_item.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_user_event.py` & `flagright-1.5.2/src/flagright/types/business_user_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_user_segment.py` & `flagright-1.5.2/src/flagright/types/business_user_segment.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_users_response.py` & `flagright-1.5.2/src/flagright/types/business_users_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/business_with_rules_result.py` & `flagright-1.5.2/src/flagright/types/business_with_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/card_brand.py` & `flagright-1.5.2/src/flagright/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/card_details.py` & `flagright-1.5.2/src/flagright/types/card_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/card_expiry.py` & `flagright-1.5.2/src/flagright/types/card_expiry.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/card_funding.py` & `flagright-1.5.2/src/flagright/types/card_funding.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/card_merchant_details.py` & `flagright-1.5.2/src/flagright/types/card_merchant_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/case_closed_details.py` & `flagright-1.5.2/src/flagright/types/case_closed_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/case_management_event.py` & `flagright-1.5.2/src/flagright/types/case_management_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/case_management_event_case_status.py` & `flagright-1.5.2/src/flagright/types/case_management_event_case_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/case_management_event_case_status_reason.py` & `flagright-1.5.2/src/flagright/types/case_management_event_case_status_reason.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/case_opened_details.py` & `flagright-1.5.2/src/flagright/types/case_opened_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/check_delivery_status.py` & `flagright-1.5.2/src/flagright/types/check_delivery_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/check_details.py` & `flagright-1.5.2/src/flagright/types/check_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/company_financial_details.py` & `flagright-1.5.2/src/flagright/types/company_financial_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/company_general_details.py` & `flagright-1.5.2/src/flagright/types/company_general_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/company_registration_details.py` & `flagright-1.5.2/src/flagright/types/company_registration_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/consumer_name.py` & `flagright-1.5.2/src/flagright/types/consumer_name.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/consumer_user_event.py` & `flagright-1.5.2/src/flagright/types/consumer_user_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/consumer_users_response.py` & `flagright-1.5.2/src/flagright/types/consumer_users_response.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/contact_details.py` & `flagright-1.5.2/src/flagright/types/contact_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/country_code.py` & `flagright-1.5.2/src/flagright/types/country_code.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/currency_code.py` & `flagright-1.5.2/src/flagright/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/date.py` & `flagright-1.5.2/src/flagright/types/date.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/device_data.py` & `flagright-1.5.2/src/flagright/types/device_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/employment_status.py` & `flagright-1.5.2/src/flagright/types/employment_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/executed_rules_result.py` & `flagright-1.5.2/src/flagright/types/executed_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/failed_rules_result.py` & `flagright-1.5.2/src/flagright/types/failed_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/false_positive_details.py` & `flagright-1.5.2/src/flagright/types/false_positive_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/gender.py` & `flagright-1.5.2/src/flagright/types/gender.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/generic_bank_account_details.py` & `flagright-1.5.2/src/flagright/types/generic_bank_account_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/hit_rules_details.py` & `flagright-1.5.2/src/flagright/types/hit_rules_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/iban_details.py` & `flagright-1.5.2/src/flagright/types/iban_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/kyc_status.py` & `flagright-1.5.2/src/flagright/types/kyc_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/kyc_status_details.py` & `flagright-1.5.2/src/flagright/types/kyc_status_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/legal_document.py` & `flagright-1.5.2/src/flagright/types/legal_document.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/legal_entity.py` & `flagright-1.5.2/src/flagright/types/legal_entity.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/list_data.py` & `flagright-1.5.2/src/flagright/types/list_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/list_existed.py` & `flagright-1.5.2/src/flagright/types/list_existed.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/list_header.py` & `flagright-1.5.2/src/flagright/types/list_header.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/list_item.py` & `flagright-1.5.2/src/flagright/types/list_item.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/list_metadata.py` & `flagright-1.5.2/src/flagright/types/list_metadata.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/list_subtype.py` & `flagright-1.5.2/src/flagright/types/list_subtype.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/list_type.py` & `flagright-1.5.2/src/flagright/types/list_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/mcc_details.py` & `flagright-1.5.2/src/flagright/types/mcc_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/mpesa_details.py` & `flagright-1.5.2/src/flagright/types/mpesa_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/mpesa_transaction_type.py` & `flagright-1.5.2/src/flagright/types/mpesa_transaction_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/payment_method.py` & `flagright-1.5.2/src/flagright/types/payment_method.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/pep_status.py` & `flagright-1.5.2/src/flagright/types/pep_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/person.py` & `flagright-1.5.2/src/flagright/types/person.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/risk_level.py` & `flagright-1.5.2/src/flagright/types/risk_level.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/rule_action.py` & `flagright-1.5.2/src/flagright/types/rule_action.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/rule_failure_exception.py` & `flagright-1.5.2/src/flagright/types/rule_failure_exception.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/rule_hit_meta.py` & `flagright-1.5.2/src/flagright/types/rule_hit_meta.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/rule_labels.py` & `flagright-1.5.2/src/flagright/types/rule_labels.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/rule_nature.py` & `flagright-1.5.2/src/flagright/types/rule_nature.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/rules_results.py` & `flagright-1.5.2/src/flagright/types/rules_results.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/sanctions_details.py` & `flagright-1.5.2/src/flagright/types/sanctions_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/sanctions_details_entity_type.py` & `flagright-1.5.2/src/flagright/types/sanctions_details_entity_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/source_of_funds.py` & `flagright-1.5.2/src/flagright/types/source_of_funds.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/swift_details.py` & `flagright-1.5.2/src/flagright/types/swift_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/tag.py` & `flagright-1.5.2/src/flagright/types/tag.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction.py` & `flagright-1.5.2/src/flagright/types/transaction.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_amount_details.py` & `flagright-1.5.2/src/flagright/types/transaction_amount_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_amount_limit.py` & `flagright-1.5.2/src/flagright/types/transaction_amount_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_base.py` & `flagright-1.5.2/src/flagright/types/transaction_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_count_limit.py` & `flagright-1.5.2/src/flagright/types/transaction_count_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_event.py` & `flagright-1.5.2/src/flagright/types/transaction_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_event_monitoring_result.py` & `flagright-1.5.2/src/flagright/types/transaction_event_monitoring_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_limit.py` & `flagright-1.5.2/src/flagright/types/transaction_limit.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_limits.py` & `flagright-1.5.2/src/flagright/types/transaction_limits.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_limits_payment_method_limits.py` & `flagright-1.5.2/src/flagright/types/transaction_limits_payment_method_limits.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_monitoring_result.py` & `flagright-1.5.2/src/flagright/types/transaction_monitoring_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_risk_scoring_result.py` & `flagright-1.5.2/src/flagright/types/transaction_risk_scoring_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_state.py` & `flagright-1.5.2/src/flagright/types/transaction_state.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_status_details.py` & `flagright-1.5.2/src/flagright/types/transaction_status_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_type.py` & `flagright-1.5.2/src/flagright/types/transaction_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_updatable.py` & `flagright-1.5.2/src/flagright/types/transaction_updatable.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_updatable_destination_payment_details.py` & `flagright-1.5.2/src/flagright/types/transaction_updatable_destination_payment_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_updatable_origin_payment_details.py` & `flagright-1.5.2/src/flagright/types/transaction_updatable_origin_payment_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/transaction_with_rules_result.py` & `flagright-1.5.2/src/flagright/types/transaction_with_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/upi_details.py` & `flagright-1.5.2/src/flagright/types/upi_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user.py` & `flagright-1.5.2/src/flagright/types/user.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_base.py` & `flagright-1.5.2/src/flagright/types/user_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_details.py` & `flagright-1.5.2/src/flagright/types/user_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_optional.py` & `flagright-1.5.2/src/flagright/types/user_optional.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_registration_status.py` & `flagright-1.5.2/src/flagright/types/user_registration_status.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_risk_score_details.py` & `flagright-1.5.2/src/flagright/types/user_risk_score_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_state.py` & `flagright-1.5.2/src/flagright/types/user_state.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_state_details.py` & `flagright-1.5.2/src/flagright/types/user_state_details.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/user_with_rules_result.py` & `flagright-1.5.2/src/flagright/types/user_with_rules_result.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/wallet_details.py` & `flagright-1.5.2/src/flagright/types/wallet_details.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .amount import Amount
 from .email_id import EmailId
 from .tag import Tag
-from .wallet_details_network import WalletDetailsNetwork
+from .wallet_network import WalletNetwork
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
@@ -33,15 +33,15 @@
     tags: typing.Optional[typing.List[Tag]] = pydantic.Field(
         description="Additional information that can be added via tags"
     )
     wallet_phone_number: typing.Optional[str] = pydantic.Field(
         alias="walletPhoneNumber", description="Phone number associated with the wallet, if any"
     )
     wallet_balance: typing.Optional[Amount] = pydantic.Field(alias="walletBalance")
-    network: typing.Optional[WalletDetailsNetwork] = pydantic.Field(description="Network of the wallet")
+    network: typing.Optional[WalletNetwork]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flagright-1.5.1/src/flagright/types/wallet_details_network.py` & `flagright-1.5.2/src/flagright/types/wallet_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class WalletDetailsNetwork(str, enum.Enum):
+class WalletNetwork(str, enum.Enum):
     """
     Network of the wallet
     """
 
     BITCOIN = "BITCOIN"
     ETHEREUM = "ETHEREUM"
     POLYGON = "POLYGON"
@@ -59,55 +59,55 @@
         dogecoin: typing.Callable[[], T_Result],
         optimism_mainnet: typing.Callable[[], T_Result],
         fantom: typing.Callable[[], T_Result],
         hedera: typing.Callable[[], T_Result],
         algorand: typing.Callable[[], T_Result],
         celestia: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is WalletDetailsNetwork.BITCOIN:
+        if self is WalletNetwork.BITCOIN:
             return bitcoin()
-        if self is WalletDetailsNetwork.ETHEREUM:
+        if self is WalletNetwork.ETHEREUM:
             return ethereum()
-        if self is WalletDetailsNetwork.POLYGON:
+        if self is WalletNetwork.POLYGON:
             return polygon()
-        if self is WalletDetailsNetwork.BNB_SMART_CHAIN:
+        if self is WalletNetwork.BNB_SMART_CHAIN:
             return bnb_smart_chain()
-        if self is WalletDetailsNetwork.BNB_BEACON_CHAIN:
+        if self is WalletNetwork.BNB_BEACON_CHAIN:
             return bnb_beacon_chain()
-        if self is WalletDetailsNetwork.ARBITRUM_L_2:
+        if self is WalletNetwork.ARBITRUM_L_2:
             return arbitrum_l_2()
-        if self is WalletDetailsNetwork.SOLANA:
+        if self is WalletNetwork.SOLANA:
             return solana()
-        if self is WalletDetailsNetwork.AVALANCHE_C_CHAIN:
+        if self is WalletNetwork.AVALANCHE_C_CHAIN:
             return avalanche_c_chain()
-        if self is WalletDetailsNetwork.LITECOIN:
+        if self is WalletNetwork.LITECOIN:
             return litecoin()
-        if self is WalletDetailsNetwork.BITCOIN_CASH:
+        if self is WalletNetwork.BITCOIN_CASH:
             return bitcoin_cash()
-        if self is WalletDetailsNetwork.RIPPLE:
+        if self is WalletNetwork.RIPPLE:
             return ripple()
-        if self is WalletDetailsNetwork.STELLAR:
+        if self is WalletNetwork.STELLAR:
             return stellar()
-        if self is WalletDetailsNetwork.EOS_PUBLIC:
+        if self is WalletNetwork.EOS_PUBLIC:
             return eos_public()
-        if self is WalletDetailsNetwork.TRON:
+        if self is WalletNetwork.TRON:
             return tron()
-        if self is WalletDetailsNetwork.CARDANO:
+        if self is WalletNetwork.CARDANO:
             return cardano()
-        if self is WalletDetailsNetwork.POLKADOT:
+        if self is WalletNetwork.POLKADOT:
             return polkadot()
-        if self is WalletDetailsNetwork.NEAR_PROTOCOL:
+        if self is WalletNetwork.NEAR_PROTOCOL:
             return near_protocol()
-        if self is WalletDetailsNetwork.COSMOS:
+        if self is WalletNetwork.COSMOS:
             return cosmos()
-        if self is WalletDetailsNetwork.DOGECOIN:
+        if self is WalletNetwork.DOGECOIN:
             return dogecoin()
-        if self is WalletDetailsNetwork.OPTIMISM_MAINNET:
+        if self is WalletNetwork.OPTIMISM_MAINNET:
             return optimism_mainnet()
-        if self is WalletDetailsNetwork.FANTOM:
+        if self is WalletNetwork.FANTOM:
             return fantom()
-        if self is WalletDetailsNetwork.HEDERA:
+        if self is WalletNetwork.HEDERA:
             return hedera()
-        if self is WalletDetailsNetwork.ALGORAND:
+        if self is WalletNetwork.ALGORAND:
             return algorand()
-        if self is WalletDetailsNetwork.CELESTIA:
+        if self is WalletNetwork.CELESTIA:
             return celestia()
```

### Comparing `flagright-1.5.1/src/flagright/types/webhook_event.py` & `flagright-1.5.2/src/flagright/types/webhook_event.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/webhook_event_base.py` & `flagright-1.5.2/src/flagright/types/webhook_event_base.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/webhook_event_base_triggered_by.py` & `flagright-1.5.2/src/flagright/types/webhook_event_base_triggered_by.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/webhook_event_data.py` & `flagright-1.5.2/src/flagright/types/webhook_event_data.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/src/flagright/types/webhook_event_type.py` & `flagright-1.5.2/src/flagright/types/webhook_event_type.py`

 * *Files identical despite different names*

### Comparing `flagright-1.5.1/PKG-INFO` & `flagright-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagright
-Version: 1.5.1
+Version: 1.5.2
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

