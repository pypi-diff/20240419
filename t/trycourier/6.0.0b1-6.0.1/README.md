# Comparing `tmp/trycourier-6.0.0b1.tar.gz` & `tmp/trycourier-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-6.0.0b1.tar", max compression
+gzip compressed data, was "trycourier-6.0.1.tar", max compression
```

## Comparing `trycourier-6.0.0b1.tar` & `trycourier-6.0.1.tar`

### file list

```diff
@@ -1,351 +1,366 @@
--rw-r--r--   0        0        0     1063 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/LICENSE
--rw-r--r--   0        0        0     5507 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/README.md
--rw-r--r--   0        0        0      406 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    13103 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/__init__.py
--rw-r--r--   0        0        0     9148 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/client.py
--rw-r--r--   0        0        0      519 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/__init__.py
--rw-r--r--   0        0        0      426 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/api_error.py
--rw-r--r--   0        0        0     1649 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      159 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/environment.py
--rw-r--r--   0        0        0        0 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/py.typed
--rw-r--r--   0        0        0    13286 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/__init__.py
--rw-r--r--   0        0        0      751 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/__init__.py
--rw-r--r--   0        0        0    12869 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/client.py
--rw-r--r--   0        0        0     1100 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/__init__.py
--rw-r--r--   0        0        0     1186 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience.py
--rw-r--r--   0        0        0      991 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_list_response.py
--rw-r--r--   0        0        0      959 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member.py
--rw-r--r--   0        0        0     1037 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_get_response.py
--rw-r--r--   0        0        0     1016 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_list_response.py
--rw-r--r--   0        0        0      921 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_update_response.py
--rw-r--r--   0        0        0      981 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/base_filter_config.py
--rw-r--r--   0        0        0     2042 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/comparison_operator.py
--rw-r--r--   0        0        0      249 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/filter.py
--rw-r--r--   0        0        0      255 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/filter_config.py
--rw-r--r--   0        0        0      438 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/logical_operator.py
--rw-r--r--   0        0        0     1069 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/nested_filter_config.py
--rw-r--r--   0        0        0      240 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/operator.py
--rw-r--r--   0        0        0     1236 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audiences/types/single_filter_config.py
--rw-r--r--   0        0        0      299 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/__init__.py
--rw-r--r--   0        0        0     4722 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/client.py
--rw-r--r--   0        0        0      453 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/__init__.py
--rw-r--r--   0        0        0      911 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/actor.py
--rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/audit_event.py
--rw-r--r--   0        0        0      973 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/get_audit_event_params.py
--rw-r--r--   0        0        0      899 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_params.py
--rw-r--r--   0        0        0     1003 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_response.py
--rw-r--r--   0        0        0      912 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/audit_events/types/target.py
--rw-r--r--   0        0        0      137 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/__init__.py
--rw-r--r--   0        0        0     3818 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/client.py
--rw-r--r--   0        0        0      152 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/types/__init__.py
--rw-r--r--   0        0        0      895 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/auth_tokens/types/issue_token_response.py
--rw-r--r--   0        0        0     1063 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/__init__.py
--rw-r--r--   0        0        0     7746 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/client.py
--rw-r--r--   0        0        0     1593 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/__init__.py
--rw-r--r--   0        0        0     1001 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation.py
--rw-r--r--   0        0        0      932 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_ad_hoc_invoke_params.py
--rw-r--r--   0        0        0      956 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_cancel_step.py
--rw-r--r--   0        0        0      942 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_delay_step.py
--rw-r--r--   0        0        0     1093 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_params.py
--rw-r--r--   0        0        0      963 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_response.py
--rw-r--r--   0        0        0      930 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_step.py
--rw-r--r--   0        0        0     1044 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_template_params.py
--rw-r--r--   0        0        0     1073 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_run_context.py
--rw-r--r--   0        0        0     1114 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_list_step.py
--rw-r--r--   0        0        0     1168 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_step.py
--rw-r--r--   0        0        0      994 2024-02-01 00:59:16.815857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step.py
--rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step_action.py
--rw-r--r--   0        0        0      723 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step_option.py
--rw-r--r--   0        0        0     1096 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_update_profile_step.py
--rw-r--r--   0        0        0      973 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/automation_v_2_send_step.py
--rw-r--r--   0        0        0      805 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/merge_algorithm.py
--rw-r--r--   0        0        0      101 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/automations/types/profile.py
--rw-r--r--   0        0        0      419 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/__init__.py
--rw-r--r--   0        0        0    13748 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/client.py
--rw-r--r--   0        0        0      579 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/__init__.py
--rw-r--r--   0        0        0     1694 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand.py
--rw-r--r--   0        0        0      961 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_colors.py
--rw-r--r--   0        0        0      983 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_get_all_response.py
--rw-r--r--   0        0        0     1115 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_parameters.py
--rw-r--r--   0        0        0     1051 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_settings.py
--rw-r--r--   0        0        0      964 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippet.py
--rw-r--r--   0        0        0      935 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippets.py
--rw-r--r--   0        0        0      978 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/brands/types/brands_response.py
--rw-r--r--   0        0        0     1059 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/__init__.py
--rw-r--r--   0        0        0    14009 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/client.py
--rw-r--r--   0        0        0     1603 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/__init__.py
--rw-r--r--   0        0        0      960 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_create_job_response.py
--rw-r--r--   0        0        0      955 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_params.py
--rw-r--r--   0        0        0      919 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_response.py
--rw-r--r--   0        0        0      993 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_params.py
--rw-r--r--   0        0        0     1042 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_response.py
--rw-r--r--   0        0        0      903 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_error.py
--rw-r--r--   0        0        0      975 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_params.py
--rw-r--r--   0        0        0      988 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_response.py
--rw-r--r--   0        0        0      805 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_job_status.py
--rw-r--r--   0        0        0      658 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_job_user_status.py
--rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_message_user_response.py
--rw-r--r--   0        0        0     1545 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_content_message.py
--rw-r--r--   0        0        0      967 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message.py
--rw-r--r--   0        0        0     1203 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_user.py
--rw-r--r--   0        0        0     1766 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_v_1.py
--rw-r--r--   0        0        0      310 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_v_2.py
--rw-r--r--   0        0        0     1198 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_template_message.py
--rw-r--r--   0        0        0     1066 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/bulk/types/job_details.py
--rw-r--r--   0        0        0     1127 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/__init__.py
--rw-r--r--   0        0        0      527 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      290 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/already_exists_error.py
--rw-r--r--   0        0        0      278 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      269 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/conflict_error.py
--rw-r--r--   0        0        0      299 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/message_not_found_error.py
--rw-r--r--   0        0        0      270 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      298 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/errors/payment_required_error.py
--rw-r--r--   0        0        0     1207 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      903 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/already_exists.py
--rw-r--r--   0        0        0      900 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/bad_request.py
--rw-r--r--   0        0        0      949 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/base_error.py
--rw-r--r--   0        0        0     1112 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/channel_classification.py
--rw-r--r--   0        0        0      955 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/channel_preference.py
--rw-r--r--   0        0        0      898 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/conflict.py
--rw-r--r--   0        0        0      896 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/email.py
--rw-r--r--   0        0        0      905 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/message_not_found.py
--rw-r--r--   0        0        0      898 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/not_found.py
--rw-r--r--   0        0        0     1143 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/notification_preference_details.py
--rw-r--r--   0        0        0      230 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/notification_preferences.py
--rw-r--r--   0        0        0      899 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/paging.py
--rw-r--r--   0        0        0      903 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/payment_required.py
--rw-r--r--   0        0        0      679 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/preference_status.py
--rw-r--r--   0        0        0     1044 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/recipient_preferences.py
--rw-r--r--   0        0        0      896 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/rule.py
--rw-r--r--   0        0        0     1182 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/commons/types/user_tenant_association.py
--rw-r--r--   0        0        0      739 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/__init__.py
--rw-r--r--   0        0        0    26745 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/client.py
--rw-r--r--   0        0        0     1086 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/__init__.py
--rw-r--r--   0        0        0      943 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list.py
--rw-r--r--   0        0        0      905 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_params.py
--rw-r--r--   0        0        0      990 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_response.py
--rw-r--r--   0        0        0      928 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_params.py
--rw-r--r--   0        0        0      977 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_response.py
--rw-r--r--   0        0        0      904 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_params.py
--rw-r--r--   0        0        0     1052 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_response.py
--rw-r--r--   0        0        0      999 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_put_params.py
--rw-r--r--   0        0        0     1137 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/list_subscription_recipient.py
--rw-r--r--   0        0        0     1103 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/put_subscriptions_recipient.py
--rw-r--r--   0        0        0      991 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/lists/types/recipient_subscriptions_response.py
--rw-r--r--   0        0        0      527 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/__init__.py
--rw-r--r--   0        0        0    20617 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/client.py
--rw-r--r--   0        0        0      747 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/__init__.py
--rw-r--r--   0        0        0     1156 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/list_messages_response.py
--rw-r--r--   0        0        0     2788 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/message_details.py
--rw-r--r--   0        0        0      952 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/message_history_response.py
--rw-r--r--   0        0        0     2661 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/message_status.py
--rw-r--r--   0        0        0     1689 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/reason.py
--rw-r--r--   0        0        0     1222 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/render_output.py
--rw-r--r--   0        0        0     1046 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/render_output_response.py
--rw-r--r--   0        0        0     1049 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_block.py
--rw-r--r--   0        0        0     1454 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_content.py
--rw-r--r--   0        0        0      985 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/__init__.py
--rw-r--r--   0        0        0    17458 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/client.py
--rw-r--r--   0        0        0     1463 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/__init__.py
--rw-r--r--   0        0        0     1000 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/base_check.py
--rw-r--r--   0        0        0     1420 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/block_type.py
--rw-r--r--   0        0        0      825 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/check.py
--rw-r--r--   0        0        0      639 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/check_status.py
--rw-r--r--   0        0        0     1147 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing.py
--rw-r--r--   0        0        0      183 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing_channel.py
--rw-r--r--   0        0        0      469 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing_method.py
--rw-r--r--   0        0        0      961 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification.py
--rw-r--r--   0        0        0     1201 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_block.py
--rw-r--r--   0        0        0     1143 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel.py
--rw-r--r--   0        0        0      937 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel_content.py
--rw-r--r--   0        0        0      224 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_content.py
--rw-r--r--   0        0        0      941 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_content_hierarchy.py
--rw-r--r--   0        0        0     1138 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_get_content_response.py
--rw-r--r--   0        0        0     1009 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_list_response.py
--rw-r--r--   0        0        0      928 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_get_response.py
--rw-r--r--   0        0        0      932 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_replace_response.py
--rw-r--r--   0        0        0     1877 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/__init__.py
--rw-r--r--   0        0        0    20924 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/client.py
--rw-r--r--   0        0        0     2897 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/__init__.py
--rw-r--r--   0        0        0      967 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/address.py
--rw-r--r--   0        0        0     1035 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile.py
--rw-r--r--   0        0        0      887 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile_audience.py
--rw-r--r--   0        0        0      950 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/delete_list_subscription_response.py
--rw-r--r--   0        0        0      104 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/device_type.py
--rw-r--r--   0        0        0      232 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/discord.py
--rw-r--r--   0        0        0      193 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/expo.py
--rw-r--r--   0        0        0     1356 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_list.py
--rw-r--r--   0        0        0     1102 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_response.py
--rw-r--r--   0        0        0     1021 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom.py
--rw-r--r--   0        0        0      874 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom_recipient.py
--rw-r--r--   0        0        0      940 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/merge_profile_response.py
--rw-r--r--   0        0        0      566 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/ms_teams.py
--rw-r--r--   0        0        0      906 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/ms_teams_base_properties.py
--rw-r--r--   0        0        0      915 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/multiple_tokens.py
--rw-r--r--   0        0        0      971 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_parameters.py
--rw-r--r--   0        0        0     1032 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_response.py
--rw-r--r--   0        0        0      942 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/replace_profile_response.py
--rw-r--r--   0        0        0      879 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_direct_message.py
--rw-r--r--   0        0        0      878 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_channel.py
--rw-r--r--   0        0        0      883 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_channel_id.py
--rw-r--r--   0        0        0      904 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_channel_name.py
--rw-r--r--   0        0        0      893 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_conversation_id.py
--rw-r--r--   0        0        0      874 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_email.py
--rw-r--r--   0        0        0      877 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_user_id.py
--rw-r--r--   0        0        0      869 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_channel.py
--rw-r--r--   0        0        0      865 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_email.py
--rw-r--r--   0        0        0      868 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_user_id.py
--rw-r--r--   0        0        0      316 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/slack.py
--rw-r--r--   0        0        0      886 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/slack_base_properties.py
--rw-r--r--   0        0        0      955 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/snooze_rule.py
--rw-r--r--   0        0        0      335 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/snooze_rule_type.py
--rw-r--r--   0        0        0     1012 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request.py
--rw-r--r--   0        0        0     1101 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request_list_object.py
--rw-r--r--   0        0        0      944 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_response.py
--rw-r--r--   0        0        0      865 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/token.py
--rw-r--r--   0        0        0     2011 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/profiles/types/user_profile.py
--rw-r--r--   0        0        0     3925 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/__init__.py
--rw-r--r--   0        0        0     5870 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/__init__.py
--rw-r--r--   0        0        0      122 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/attachment.py
--rw-r--r--   0        0        0     1102 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/audience_filter.py
--rw-r--r--   0        0        0     1210 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/audience_recipient.py
--rw-r--r--   0        0        0     2974 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/base_message.py
--rw-r--r--   0        0        0      876 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/base_social_presence.py
--rw-r--r--   0        0        0     1302 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_email.py
--rw-r--r--   0        0        0     1564 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_in_app.py
--rw-r--r--   0        0        0     1303 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_social_presence.py
--rw-r--r--   0        0        0     1234 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_template.py
--rw-r--r--   0        0        0     1158 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/brand_template_override.py
--rw-r--r--   0        0        0     2459 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/channel.py
--rw-r--r--   0        0        0      911 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/channel_metadata.py
--rw-r--r--   0        0        0      667 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/channel_source.py
--rw-r--r--   0        0        0      252 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/content.py
--rw-r--r--   0        0        0     1666 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/content_message.py
--rw-r--r--   0        0        0      800 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/criteria.py
--rw-r--r--   0        0        0      943 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/delay.py
--rw-r--r--   0        0        0     2040 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_action_node.py
--rw-r--r--   0        0        0     1076 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_base_node.py
--rw-r--r--   0        0        0     2603 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_channel_node.py
--rw-r--r--   0        0        0     1058 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content.py
--rw-r--r--   0        0        0     1193 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content_sugar.py
--rw-r--r--   0        0        0     1161 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_divider_node.py
--rw-r--r--   0        0        0     1430 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_group_node.py
--rw-r--r--   0        0        0     1592 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_image_node.py
--rw-r--r--   0        0        0     1367 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_meta_node.py
--rw-r--r--   0        0        0     2827 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_node.py
--rw-r--r--   0        0        0     1649 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_quote_node.py
--rw-r--r--   0        0        0     2391 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/elemental_text_node.py
--rw-r--r--   0        0        0     1027 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/email_footer.py
--rw-r--r--   0        0        0     1001 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/email_head.py
--rw-r--r--   0        0        0     1095 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/email_header.py
--rw-r--r--   0        0        0      119 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/expires_in_type.py
--rw-r--r--   0        0        0     1272 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/expiry.py
--rw-r--r--   0        0        0      468 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_action_button_style.py
--rw-r--r--   0        0        0      730 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_alignment.py
--rw-r--r--   0        0        0      160 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_preferences.py
--rw-r--r--   0        0        0     1103 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/i_profile_preferences.py
--rw-r--r--   0        0        0      915 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/icons.py
--rw-r--r--   0        0        0      745 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/in_app_placement.py
--rw-r--r--   0        0        0      906 2024-02-01 00:59:16.819857 trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_pattern_recipient.py
--rw-r--r--   0        0        0      904 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_recipient.py
--rw-r--r--   0        0        0      904 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/invalid_user_recipient.py
--rw-r--r--   0        0        0     1098 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_filter.py
--rw-r--r--   0        0        0      986 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient.py
--rw-r--r--   0        0        0      868 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient_type.py
--rw-r--r--   0        0        0     1042 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient.py
--rw-r--r--   0        0        0      861 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient_type.py
--rw-r--r--   0        0        0      868 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/locale.py
--rw-r--r--   0        0        0      160 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/locales.py
--rw-r--r--   0        0        0      912 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/logo.py
--rw-r--r--   0        0        0      227 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message.py
--rw-r--r--   0        0        0     1417 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_channel_email_override.py
--rw-r--r--   0        0        0      154 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_channels.py
--rw-r--r--   0        0        0     1173 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_context.py
--rw-r--r--   0        0        0      123 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_data.py
--rw-r--r--   0        0        0     1708 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_metadata.py
--rw-r--r--   0        0        0      196 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_providers.py
--rw-r--r--   0        0        0     1478 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_providers_type.py
--rw-r--r--   0        0        0      181 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/message_recipient.py
--rw-r--r--   0        0        0      904 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/metadata.py
--rw-r--r--   0        0        0      708 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/override.py
--rw-r--r--   0        0        0     1257 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/preference.py
--rw-r--r--   0        0        0      975 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/preferences.py
--rw-r--r--   0        0        0      473 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/recipient.py
--rw-r--r--   0        0        0     1536 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing.py
--rw-r--r--   0        0        0      289 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_channel.py
--rw-r--r--   0        0        0      448 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_method.py
--rw-r--r--   0        0        0     1229 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_strategy_channel.py
--rw-r--r--   0        0        0     1099 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/routing_strategy_provider.py
--rw-r--r--   0        0        0      677 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/rule_type.py
--rw-r--r--   0        0        0     1332 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/template_message.py
--rw-r--r--   0        0        0      601 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/text_align.py
--rw-r--r--   0        0        0      713 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/text_style.py
--rw-r--r--   0        0        0     1099 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/timeout.py
--rw-r--r--   0        0        0      922 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/timeouts.py
--rw-r--r--   0        0        0      876 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/tracking_override.py
--rw-r--r--   0        0        0     1966 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient.py
--rw-r--r--   0        0        0      861 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient_type.py
--rw-r--r--   0        0        0     1014 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/utm.py
--rw-r--r--   0        0        0     1055 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/send/types/widget_background.py
--rw-r--r--   0        0        0      411 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/__init__.py
--rw-r--r--   0        0        0     2821 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/client.py
--rw-r--r--   0        0        0      564 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/__init__.py
--rw-r--r--   0        0        0       89 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/channel_identifier.py
--rw-r--r--   0        0        0     1101 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/list_templates_response.py
--rw-r--r--   0        0        0     1764 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/notification_templates.py
--rw-r--r--   0        0        0     1378 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/routing_strategy.py
--rw-r--r--   0        0        0      472 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/routing_strategy_method.py
--rw-r--r--   0        0        0      909 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/tag.py
--rw-r--r--   0        0        0      991 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/templates/types/tag_data.py
--rw-r--r--   0        0        0      449 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/__init__.py
--rw-r--r--   0        0        0    13350 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/client.py
--rw-r--r--   0        0        0      624 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/__init__.py
--rw-r--r--   0        0        0      955 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/default_preferences.py
--rw-r--r--   0        0        0     1780 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/list_users_for_tenant_response.py
--rw-r--r--   0        0        0     1014 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/subscription_topic.py
--rw-r--r--   0        0        0      707 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/subscription_topic_status.py
--rw-r--r--   0        0        0      110 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/template_property.py
--rw-r--r--   0        0        0     1844 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/tenant.py
--rw-r--r--   0        0        0     1746 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/tenants/types/tenant_list_response.py
--rw-r--r--   0        0        0       65 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/translations/__init__.py
--rw-r--r--   0        0        0     5527 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/translations/client.py
--rw-r--r--   0        0        0     1259 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/__init__.py
--rw-r--r--   0        0        0     1098 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/client.py
--rw-r--r--   0        0        0     1298 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/__init__.py
--rw-r--r--   0        0        0      353 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/__init__.py
--rw-r--r--   0        0        0    10433 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/client.py
--rw-r--r--   0        0        0      473 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/__init__.py
--rw-r--r--   0        0        0     1351 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/topic_preference.py
--rw-r--r--   0        0        0      946 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_get_response.py
--rw-r--r--   0        0        0     1101 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_list_response.py
--rw-r--r--   0        0        0      893 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_update_response.py
--rw-r--r--   0        0        0      229 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/__init__.py
--rw-r--r--   0        0        0    10729 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/client.py
--rw-r--r--   0        0        0      308 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/__init__.py
--rw-r--r--   0        0        0     1279 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/add_user_to_single_tenants_params_profile.py
--rw-r--r--   0        0        0     1784 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/types/list_tenants_for_user_response.py
--rw-r--r--   0        0        0      765 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/__init__.py
--rw-r--r--   0        0        0    12257 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/client.py
--rw-r--r--   0        0        0     1135 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/__init__.py
--rw-r--r--   0        0        0      898 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/delete_user_token_opts.py
--rw-r--r--   0        0        0     1459 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/device.py
--rw-r--r--   0        0        0      117 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/expiry_date.py
--rw-r--r--   0        0        0      161 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_all_tokens_response.py
--rw-r--r--   0        0        0      895 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_opts.py
--rw-r--r--   0        0        0     1122 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_response.py
--rw-r--r--   0        0        0      881 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_tokens_opts.py
--rw-r--r--   0        0        0      964 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_op.py
--rw-r--r--   0        0        0     1134 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_operation.py
--rw-r--r--   0        0        0      948 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_user_token_opts.py
--rw-r--r--   0        0        0      780 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/provider_key.py
--rw-r--r--   0        0        0      935 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/put_user_token_opts.py
--rw-r--r--   0        0        0      950 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/put_user_tokens_opts.py
--rw-r--r--   0        0        0      770 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/token_status.py
--rw-r--r--   0        0        0     1223 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/tracking.py
--rw-r--r--   0        0        0     1752 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/user_token.py
--rw-r--r--   0        0        0      155 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/types/__init__.py
--rw-r--r--   0        0        0     1669 2024-02-01 00:59:16.823857 trycourier-6.0.0b1/src/courier/types/send_message_response.py
--rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 trycourier-6.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-19 13:18:38.103251 trycourier-6.0.1/LICENSE
+-rw-r--r--   0        0        0     5507 2024-04-19 13:18:38.103251 trycourier-6.0.1/README.md
+-rw-r--r--   0        0        0      596 2024-04-19 13:18:38.103251 trycourier-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0    14108 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/__init__.py
+-rw-r--r--   0        0        0      751 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/__init__.py
+-rw-r--r--   0        0        0    26958 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/client.py
+-rw-r--r--   0        0        0     1100 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/__init__.py
+-rw-r--r--   0        0        0     1199 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/audience.py
+-rw-r--r--   0        0        0      971 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/audience_list_response.py
+-rw-r--r--   0        0        0      939 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/audience_member.py
+-rw-r--r--   0        0        0     1052 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/audience_member_get_response.py
+-rw-r--r--   0        0        0      996 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/audience_member_list_response.py
+-rw-r--r--   0        0        0      901 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/audience_update_response.py
+-rw-r--r--   0        0        0      971 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/base_filter_config.py
+-rw-r--r--   0        0        0      386 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/comparison_operator.py
+-rw-r--r--   0        0        0      249 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/filter.py
+-rw-r--r--   0        0        0      255 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/filter_config.py
+-rw-r--r--   0        0        0      152 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/logical_operator.py
+-rw-r--r--   0        0        0     1191 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/nested_filter_config.py
+-rw-r--r--   0        0        0      240 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/operator.py
+-rw-r--r--   0        0        0     1252 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audiences/types/single_filter_config.py
+-rw-r--r--   0        0        0      299 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/__init__.py
+-rw-r--r--   0        0        0     9927 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/client.py
+-rw-r--r--   0        0        0      453 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/types/__init__.py
+-rw-r--r--   0        0        0      905 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/types/actor.py
+-rw-r--r--   0        0        0     1164 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/types/audit_event.py
+-rw-r--r--   0        0        0      988 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/types/get_audit_event_params.py
+-rw-r--r--   0        0        0      886 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/types/list_audit_events_params.py
+-rw-r--r--   0        0        0      983 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/types/list_audit_events_response.py
+-rw-r--r--   0        0        0      906 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/audit_events/types/target.py
+-rw-r--r--   0        0        0      137 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/auth_tokens/__init__.py
+-rw-r--r--   0        0        0     6701 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/auth_tokens/client.py
+-rw-r--r--   0        0        0      152 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/auth_tokens/types/__init__.py
+-rw-r--r--   0        0        0      882 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/auth_tokens/types/issue_token_response.py
+-rw-r--r--   0        0        0     1847 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/__init__.py
+-rw-r--r--   0        0        0    15769 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/client.py
+-rw-r--r--   0        0        0     2836 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/__init__.py
+-rw-r--r--   0        0        0      962 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/accessor_type.py
+-rw-r--r--   0        0        0      988 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/automation.py
+-rw-r--r--   0        0        0     1054 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/automation_ad_hoc_invoke_params.py
+-rw-r--r--   0        0        0      138 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/automation_add_to_batch_max_items_type.py
+-rw-r--r--   0        0        0     1935 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/automation_add_to_batch_retain.py
+-rw-r--r--   0        0        0      192 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/automation_add_to_batch_retain_type.py
+-rw-r--r--   0        0        0      178 2024-04-19 13:18:38.103251 trycourier-6.0.1/src/courier/automations/types/automation_add_to_batch_scope.py
+-rw-r--r--   0        0        0     3102 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_add_to_batch_step.py
+-rw-r--r--   0        0        0     1329 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_add_to_digest_step.py
+-rw-r--r--   0        0        0     1048 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_cancel_step.py
+-rw-r--r--   0        0        0     1331 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_delay_step.py
+-rw-r--r--   0        0        0     1758 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_fetch_data_step.py
+-rw-r--r--   0        0        0     1186 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_fetch_data_webhook.py
+-rw-r--r--   0        0        0      171 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_fetch_data_webhook_method.py
+-rw-r--r--   0        0        0     1108 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_invoke_params.py
+-rw-r--r--   0        0        0      978 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_invoke_response.py
+-rw-r--r--   0        0        0     1015 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_invoke_step.py
+-rw-r--r--   0        0        0     1056 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_invoke_template_params.py
+-rw-r--r--   0        0        0     1088 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_run_context.py
+-rw-r--r--   0        0        0     1262 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_send_list_step.py
+-rw-r--r--   0        0        0     1295 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_send_step.py
+-rw-r--r--   0        0        0     1030 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_step.py
+-rw-r--r--   0        0        0     1102 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_step_option.py
+-rw-r--r--   0        0        0     1052 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_throttle_on_throttle.py
+-rw-r--r--   0        0        0      176 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_throttle_scope.py
+-rw-r--r--   0        0        0     2275 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_throttle_step.py
+-rw-r--r--   0        0        0     1039 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_update_profile_step.py
+-rw-r--r--   0        0        0     1058 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/automation_v_2_send_step.py
+-rw-r--r--   0        0        0      184 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/merge_algorithm.py
+-rw-r--r--   0        0        0      101 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/automations/types/profile.py
+-rw-r--r--   0        0        0      419 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/__init__.py
+-rw-r--r--   0        0        0    28589 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/client.py
+-rw-r--r--   0        0        0      579 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/__init__.py
+-rw-r--r--   0        0        0     1716 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brand.py
+-rw-r--r--   0        0        0      962 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brand_colors.py
+-rw-r--r--   0        0        0      963 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brand_get_all_response.py
+-rw-r--r--   0        0        0     1120 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brand_parameters.py
+-rw-r--r--   0        0        0     1052 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brand_settings.py
+-rw-r--r--   0        0        0      907 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brand_snippet.py
+-rw-r--r--   0        0        0      915 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brand_snippets.py
+-rw-r--r--   0        0        0      958 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/brands/types/brands_response.py
+-rw-r--r--   0        0        0     1059 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/__init__.py
+-rw-r--r--   0        0        0    28740 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/client.py
+-rw-r--r--   0        0        0     1603 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_create_job_response.py
+-rw-r--r--   0        0        0      970 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_params.py
+-rw-r--r--   0        0        0      899 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_response.py
+-rw-r--r--   0        0        0     1015 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_users_params.py
+-rw-r--r--   0        0        0     1022 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_users_response.py
+-rw-r--r--   0        0        0      883 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_ingest_error.py
+-rw-r--r--   0        0        0      955 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_ingest_users_params.py
+-rw-r--r--   0        0        0      975 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_ingest_users_response.py
+-rw-r--r--   0        0        0      184 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_job_status.py
+-rw-r--r--   0        0        0      173 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_job_user_status.py
+-rw-r--r--   0        0        0     1161 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/bulk_message_user_response.py
+-rw-r--r--   0        0        0     1512 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_content_message.py
+-rw-r--r--   0        0        0     1096 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_message.py
+-rw-r--r--   0        0        0     1218 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_message_user.py
+-rw-r--r--   0        0        0     1672 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_message_v_1.py
+-rw-r--r--   0        0        0      310 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_message_v_2.py
+-rw-r--r--   0        0        0     1165 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_template_message.py
+-rw-r--r--   0        0        0     1046 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/bulk/types/job_details.py
+-rw-r--r--   0        0        0    16915 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/client.py
+-rw-r--r--   0        0        0     1127 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/__init__.py
+-rw-r--r--   0        0        0      527 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/errors/__init__.py
+-rw-r--r--   0        0        0      289 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/errors/already_exists_error.py
+-rw-r--r--   0        0        0      277 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      268 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/errors/conflict_error.py
+-rw-r--r--   0        0        0      298 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/errors/message_not_found_error.py
+-rw-r--r--   0        0        0      269 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      297 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/errors/payment_required_error.py
+-rw-r--r--   0        0        0     1207 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/__init__.py
+-rw-r--r--   0        0        0      988 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/already_exists.py
+-rw-r--r--   0        0        0      985 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/bad_request.py
+-rw-r--r--   0        0        0      939 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/base_error.py
+-rw-r--r--   0        0        0      213 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/channel_classification.py
+-rw-r--r--   0        0        0      935 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/channel_preference.py
+-rw-r--r--   0        0        0      983 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/conflict.py
+-rw-r--r--   0        0        0      876 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/email.py
+-rw-r--r--   0        0        0      990 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/message_not_found.py
+-rw-r--r--   0        0        0      983 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/not_found.py
+-rw-r--r--   0        0        0     1137 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/notification_preference_details.py
+-rw-r--r--   0        0        0      230 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/notification_preferences.py
+-rw-r--r--   0        0        0      886 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/paging.py
+-rw-r--r--   0        0        0      988 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/payment_required.py
+-rw-r--r--   0        0        0      177 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/preference_status.py
+-rw-r--r--   0        0        0     1038 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/recipient_preferences.py
+-rw-r--r--   0        0        0      883 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/rule.py
+-rw-r--r--   0        0        0     1147 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/commons/types/user_tenant_association.py
+-rw-r--r--   0        0        0      853 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/api_error.py
+-rw-r--r--   0        0        0     2088 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/core/request_options.py
+-rw-r--r--   0        0        0      159 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/environment.py
+-rw-r--r--   0        0        0      413 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/__init__.py
+-rw-r--r--   0        0        0    67268 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/client.py
+-rw-r--r--   0        0        0      569 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/types/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/types/list.py
+-rw-r--r--   0        0        0      957 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/types/list_get_all_response.py
+-rw-r--r--   0        0        0     1032 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/types/list_get_subscriptions_response.py
+-rw-r--r--   0        0        0      986 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/types/list_put_params.py
+-rw-r--r--   0        0        0     1166 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/types/list_subscription_recipient.py
+-rw-r--r--   0        0        0     1125 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/lists/types/put_subscriptions_recipient.py
+-rw-r--r--   0        0        0      527 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/__init__.py
+-rw-r--r--   0        0        0    39208 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/client.py
+-rw-r--r--   0        0        0      747 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/__init__.py
+-rw-r--r--   0        0        0     1157 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/list_messages_response.py
+-rw-r--r--   0        0        0     2811 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/message_details.py
+-rw-r--r--   0        0        0      932 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/message_history_response.py
+-rw-r--r--   0        0        0      357 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/message_status.py
+-rw-r--r--   0        0        0      233 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/reason.py
+-rw-r--r--   0        0        0     1234 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/render_output.py
+-rw-r--r--   0        0        0     1022 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/render_output_response.py
+-rw-r--r--   0        0        0     1050 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/rendered_message_block.py
+-rw-r--r--   0        0        0     1499 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/messages/types/rendered_message_content.py
+-rw-r--r--   0        0        0      985 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/__init__.py
+-rw-r--r--   0        0        0    43287 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/client.py
+-rw-r--r--   0        0        0     1463 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/__init__.py
+-rw-r--r--   0        0        0      943 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/base_check.py
+-rw-r--r--   0        0        0      229 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/block_type.py
+-rw-r--r--   0        0        0      947 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/check.py
+-rw-r--r--   0        0        0      168 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/check_status.py
+-rw-r--r--   0        0        0     1127 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/message_routing.py
+-rw-r--r--   0        0        0      183 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/message_routing_channel.py
+-rw-r--r--   0        0        0      161 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/message_routing_method.py
+-rw-r--r--   0        0        0      941 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification.py
+-rw-r--r--   0        0        0     1216 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification_block.py
+-rw-r--r--   0        0        0     1151 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification_channel.py
+-rw-r--r--   0        0        0      931 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification_channel_content.py
+-rw-r--r--   0        0        0      224 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification_content.py
+-rw-r--r--   0        0        0      935 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification_content_hierarchy.py
+-rw-r--r--   0        0        0     1139 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification_get_content_response.py
+-rw-r--r--   0        0        0      989 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/notification_list_response.py
+-rw-r--r--   0        0        0      908 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/submission_checks_get_response.py
+-rw-r--r--   0        0        0      912 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/notifications/types/submission_checks_replace_response.py
+-rw-r--r--   0        0        0     1877 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/profiles/__init__.py
+-rw-r--r--   0        0        0    40419 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/profiles/client.py
+-rw-r--r--   0        0        0     2897 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/profiles/types/__init__.py
+-rw-r--r--   0        0        0      947 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/profiles/types/address.py
+-rw-r--r--   0        0        0     1015 2024-04-19 13:18:38.107251 trycourier-6.0.1/src/courier/profiles/types/airship_profile.py
+-rw-r--r--   0        0        0      867 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/airship_profile_audience.py
+-rw-r--r--   0        0        0      893 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/delete_list_subscription_response.py
+-rw-r--r--   0        0        0      104 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/device_type.py
+-rw-r--r--   0        0        0      232 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/discord.py
+-rw-r--r--   0        0        0      193 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/expo.py
+-rw-r--r--   0        0        0     1348 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/get_list_subscriptions_list.py
+-rw-r--r--   0        0        0     1092 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/get_list_subscriptions_response.py
+-rw-r--r--   0        0        0     1036 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/intercom.py
+-rw-r--r--   0        0        0      854 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/intercom_recipient.py
+-rw-r--r--   0        0        0      883 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/merge_profile_response.py
+-rw-r--r--   0        0        0      566 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/ms_teams.py
+-rw-r--r--   0        0        0      886 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/ms_teams_base_properties.py
+-rw-r--r--   0        0        0      895 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/multiple_tokens.py
+-rw-r--r--   0        0        0      986 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/profile_get_parameters.py
+-rw-r--r--   0        0        0     1019 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/profile_get_response.py
+-rw-r--r--   0        0        0      885 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/replace_profile_response.py
+-rw-r--r--   0        0        0      859 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_direct_message.py
+-rw-r--r--   0        0        0      858 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_channel.py
+-rw-r--r--   0        0        0     1005 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_channel_id.py
+-rw-r--r--   0        0        0     1026 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_channel_name.py
+-rw-r--r--   0        0        0     1015 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_conversation_id.py
+-rw-r--r--   0        0        0      996 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_email.py
+-rw-r--r--   0        0        0      999 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_user_id.py
+-rw-r--r--   0        0        0      991 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_slack_channel.py
+-rw-r--r--   0        0        0      987 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_slack_email.py
+-rw-r--r--   0        0        0      990 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/send_to_slack_user_id.py
+-rw-r--r--   0        0        0      316 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/slack.py
+-rw-r--r--   0        0        0      866 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/slack_base_properties.py
+-rw-r--r--   0        0        0      935 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/snooze_rule.py
+-rw-r--r--   0        0        0      148 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/snooze_rule_type.py
+-rw-r--r--   0        0        0      992 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/subscribe_to_lists_request.py
+-rw-r--r--   0        0        0     1123 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/subscribe_to_lists_request_list_object.py
+-rw-r--r--   0        0        0      887 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/subscribe_to_lists_response.py
+-rw-r--r--   0        0        0      845 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/token.py
+-rw-r--r--   0        0        0     2026 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/profiles/types/user_profile.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/py.typed
+-rw-r--r--   0        0        0     4101 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/__init__.py
+-rw-r--r--   0        0        0     6149 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/attachment.py
+-rw-r--r--   0        0        0     1031 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/audience_filter.py
+-rw-r--r--   0        0        0     1201 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/audience_recipient.py
+-rw-r--r--   0        0        0     2961 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/base_message.py
+-rw-r--r--   0        0        0     1039 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/base_message_send_to.py
+-rw-r--r--   0        0        0      856 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/base_social_presence.py
+-rw-r--r--   0        0        0     1366 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/brand_settings_email.py
+-rw-r--r--   0        0        0     1637 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/brand_settings_in_app.py
+-rw-r--r--   0        0        0     1367 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/brand_settings_social_presence.py
+-rw-r--r--   0        0        0     1308 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/brand_template.py
+-rw-r--r--   0        0        0     1201 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/brand_template_override.py
+-rw-r--r--   0        0        0     2359 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/channel.py
+-rw-r--r--   0        0        0      898 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/channel_metadata.py
+-rw-r--r--   0        0        0      174 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/channel_source.py
+-rw-r--r--   0        0        0      252 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/content.py
+-rw-r--r--   0        0        0     1546 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/content_message.py
+-rw-r--r--   0        0        0      183 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/criteria.py
+-rw-r--r--   0        0        0      933 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/delay.py
+-rw-r--r--   0        0        0     2131 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_action_node.py
+-rw-r--r--   0        0        0     1126 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_base_node.py
+-rw-r--r--   0        0        0     2524 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_channel_node.py
+-rw-r--r--   0        0        0     1056 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_content.py
+-rw-r--r--   0        0        0     1180 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_content_sugar.py
+-rw-r--r--   0        0        0     1178 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_divider_node.py
+-rw-r--r--   0        0        0     1449 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_group_node.py
+-rw-r--r--   0        0        0     1689 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_image_node.py
+-rw-r--r--   0        0        0     1384 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_meta_node.py
+-rw-r--r--   0        0        0     8164 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_node.py
+-rw-r--r--   0        0        0     1697 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_quote_node.py
+-rw-r--r--   0        0        0     2459 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/elemental_text_node.py
+-rw-r--r--   0        0        0     1063 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/email_footer.py
+-rw-r--r--   0        0        0     1023 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/email_head.py
+-rw-r--r--   0        0        0     1141 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/email_header.py
+-rw-r--r--   0        0        0      119 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/expires_in_type.py
+-rw-r--r--   0        0        0     1257 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/expiry.py
+-rw-r--r--   0        0        0      160 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/i_action_button_style.py
+-rw-r--r--   0        0        0      169 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/i_alignment.py
+-rw-r--r--   0        0        0      160 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/i_preferences.py
+-rw-r--r--   0        0        0     1139 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/i_profile_preferences.py
+-rw-r--r--   0        0        0      909 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/icons.py
+-rw-r--r--   0        0        0      172 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/in_app_placement.py
+-rw-r--r--   0        0        0      886 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/invalid_list_pattern_recipient.py
+-rw-r--r--   0        0        0      884 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/invalid_list_recipient.py
+-rw-r--r--   0        0        0      884 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/invalid_user_recipient.py
+-rw-r--r--   0        0        0     1027 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/list_filter.py
+-rw-r--r--   0        0        0     1122 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/list_pattern_recipient.py
+-rw-r--r--   0        0        0      848 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/list_pattern_recipient_type.py
+-rw-r--r--   0        0        0     1185 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/list_recipient.py
+-rw-r--r--   0        0        0      841 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/list_recipient_type.py
+-rw-r--r--   0        0        0      848 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/locale.py
+-rw-r--r--   0        0        0      160 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/locales.py
+-rw-r--r--   0        0        0      906 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/logo.py
+-rw-r--r--   0        0        0      227 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message.py
+-rw-r--r--   0        0        0     1502 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_channel_email_override.py
+-rw-r--r--   0        0        0      154 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_channels.py
+-rw-r--r--   0        0        0     1123 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_context.py
+-rw-r--r--   0        0        0      123 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_data.py
+-rw-r--r--   0        0        0     1723 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_metadata.py
+-rw-r--r--   0        0        0      196 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_providers.py
+-rw-r--r--   0        0        0     1477 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_providers_type.py
+-rw-r--r--   0        0        0      181 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/message_recipient.py
+-rw-r--r--   0        0        0      891 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/metadata.py
+-rw-r--r--   0        0        0      910 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/ms_teams_recipient.py
+-rw-r--r--   0        0        0      193 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/override.py
+-rw-r--r--   0        0        0     1258 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/preference.py
+-rw-r--r--   0        0        0      990 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/preferences.py
+-rw-r--r--   0        0        0      583 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/recipient.py
+-rw-r--r--   0        0        0      125 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/recipient_data.py
+-rw-r--r--   0        0        0     1462 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/routing.py
+-rw-r--r--   0        0        0      289 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/routing_channel.py
+-rw-r--r--   0        0        0      154 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/routing_method.py
+-rw-r--r--   0        0        0     1279 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/routing_strategy_channel.py
+-rw-r--r--   0        0        0     1135 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/routing_strategy_provider.py
+-rw-r--r--   0        0        0      175 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/rule_type.py
+-rw-r--r--   0        0        0      898 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/slack_recipient.py
+-rw-r--r--   0        0        0     1212 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/template_message.py
+-rw-r--r--   0        0        0      160 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/text_align.py
+-rw-r--r--   0        0        0      164 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/text_style.py
+-rw-r--r--   0        0        0     1114 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/timeout.py
+-rw-r--r--   0        0        0      916 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/timeouts.py
+-rw-r--r--   0        0        0      856 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/tracking_override.py
+-rw-r--r--   0        0        0     2035 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/user_recipient.py
+-rw-r--r--   0        0        0      841 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/user_recipient_type.py
+-rw-r--r--   0        0        0     1029 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/utm.py
+-rw-r--r--   0        0        0     1101 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/send/types/widget_background.py
+-rw-r--r--   0        0        0      411 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/__init__.py
+-rw-r--r--   0        0        0     5598 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/client.py
+-rw-r--r--   0        0        0      564 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/__init__.py
+-rw-r--r--   0        0        0       89 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/channel_identifier.py
+-rw-r--r--   0        0        0     1091 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/list_templates_response.py
+-rw-r--r--   0        0        0     1781 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/notification_templates.py
+-rw-r--r--   0        0        0     1351 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/routing_strategy.py
+-rw-r--r--   0        0        0      162 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/routing_strategy_method.py
+-rw-r--r--   0        0        0      889 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/tag.py
+-rw-r--r--   0        0        0      992 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/templates/types/tag_data.py
+-rw-r--r--   0        0        0      449 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/__init__.py
+-rw-r--r--   0        0        0    29517 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/client.py
+-rw-r--r--   0        0        0      624 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/default_preferences.py
+-rw-r--r--   0        0        0     1737 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/list_users_for_tenant_response.py
+-rw-r--r--   0        0        0     1005 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/subscription_topic.py
+-rw-r--r--   0        0        0      184 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/subscription_topic_status.py
+-rw-r--r--   0        0        0      110 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/template_property.py
+-rw-r--r--   0        0        0     1904 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/tenant.py
+-rw-r--r--   0        0        0     1698 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/tenants/types/tenant_list_response.py
+-rw-r--r--   0        0        0       65 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/translations/__init__.py
+-rw-r--r--   0        0        0    10736 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/translations/client.py
+-rw-r--r--   0        0        0      155 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/types/__init__.py
+-rw-r--r--   0        0        0     1592 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/types/send_message_response.py
+-rw-r--r--   0        0        0     1354 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/__init__.py
+-rw-r--r--   0        0        0     1067 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/client.py
+-rw-r--r--   0        0        0      409 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/__init__.py
+-rw-r--r--   0        0        0    17633 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/client.py
+-rw-r--r--   0        0        0      561 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/types/__init__.py
+-rw-r--r--   0        0        0     1345 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/types/topic_preference.py
+-rw-r--r--   0        0        0     1276 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/types/topic_preference_update.py
+-rw-r--r--   0        0        0      926 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/types/user_preferences_get_response.py
+-rw-r--r--   0        0        0     1090 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/types/user_preferences_list_response.py
+-rw-r--r--   0        0        0      873 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/preferences/types/user_preferences_update_response.py
+-rw-r--r--   0        0        0      229 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tenants/__init__.py
+-rw-r--r--   0        0        0    28095 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tenants/client.py
+-rw-r--r--   0        0        0      308 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tenants/types/__init__.py
+-rw-r--r--   0        0        0     1288 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py
+-rw-r--r--   0        0        0     1740 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tenants/types/list_tenants_for_user_response.py
+-rw-r--r--   0        0        0      765 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tokens/__init__.py
+-rw-r--r--   0        0        0    28284 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tokens/client.py
+-rw-r--r--   0        0        0     1135 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tokens/types/__init__.py
+-rw-r--r--   0        0        0      878 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tokens/types/delete_user_token_opts.py
+-rw-r--r--   0        0        0     1576 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tokens/types/device.py
+-rw-r--r--   0        0        0      117 2024-04-19 13:18:38.111251 trycourier-6.0.1/src/courier/users/tokens/types/expiry_date.py
+-rw-r--r--   0        0        0      161 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/get_all_tokens_response.py
+-rw-r--r--   0        0        0      875 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/get_user_token_opts.py
+-rw-r--r--   0        0        0     1160 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/get_user_token_response.py
+-rw-r--r--   0        0        0      861 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/get_user_tokens_opts.py
+-rw-r--r--   0        0        0      183 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/patch_op.py
+-rw-r--r--   0        0        0     1158 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/patch_operation.py
+-rw-r--r--   0        0        0      928 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/patch_user_token_opts.py
+-rw-r--r--   0        0        0      179 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/provider_key.py
+-rw-r--r--   0        0        0      915 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/put_user_token_opts.py
+-rw-r--r--   0        0        0      930 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/put_user_tokens_opts.py
+-rw-r--r--   0        0        0      177 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/token_status.py
+-rw-r--r--   0        0        0     1387 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/tracking.py
+-rw-r--r--   0        0        0     1790 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/users/tokens/types/user_token.py
+-rw-r--r--   0        0        0       78 2024-04-19 13:18:38.115251 trycourier-6.0.1/src/courier/version.py
+-rw-r--r--   0        0        0     6000 1970-01-01 00:00:00.000000 trycourier-6.0.1/PKG-INFO
```

### Comparing `trycourier-6.0.0b1/LICENSE` & `trycourier-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/README.md` & `trycourier-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/__init__.py` & `trycourier-6.0.1/src/courier/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,230 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import SendMessageResponse
-from .resources import (
-    Actor,
-    Address,
-    AirshipProfile,
-    AirshipProfileAudience,
-    AlreadyExists,
-    AlreadyExistsError,
-    Attachment,
+from . import (
+    audiences,
+    audit_events,
+    auth_tokens,
+    automations,
+    brands,
+    bulk,
+    commons,
+    lists,
+    messages,
+    notifications,
+    profiles,
+    send,
+    templates,
+    tenants,
+    translations,
+    users,
+)
+from .audiences import (
     Audience,
-    AudienceFilter,
     AudienceListResponse,
     AudienceMember,
     AudienceMemberGetResponse,
     AudienceMemberListResponse,
-    AudienceRecipient,
     AudienceUpdateResponse,
-    AuditEvent,
+    BaseFilterConfig,
+    ComparisonOperator,
+    Filter,
+    FilterConfig,
+    LogicalOperator,
+    NestedFilterConfig,
+    Operator,
+    SingleFilterConfig,
+)
+from .audit_events import Actor, AuditEvent, GetAuditEventParams, ListAuditEventsParams, ListAuditEventsResponse, Target
+from .auth_tokens import IssueTokenResponse
+from .automations import (
+    AccessorType,
     Automation,
     AutomationAdHocInvokeParams,
+    AutomationAddToBatchMaxItemsType,
+    AutomationAddToBatchRetain,
+    AutomationAddToBatchRetainType,
+    AutomationAddToBatchScope,
+    AutomationAddToBatchStep,
+    AutomationAddToDigestStep,
     AutomationCancelStep,
     AutomationDelayStep,
+    AutomationFetchDataStep,
+    AutomationFetchDataWebhook,
+    AutomationFetchDataWebhookMethod,
     AutomationInvokeParams,
     AutomationInvokeResponse,
     AutomationInvokeStep,
     AutomationInvokeTemplateParams,
     AutomationRunContext,
     AutomationSendListStep,
     AutomationSendStep,
     AutomationStep,
-    AutomationStepAction,
     AutomationStepOption,
+    AutomationThrottleOnThrottle,
+    AutomationThrottleScope,
+    AutomationThrottleStep,
     AutomationUpdateProfileStep,
     AutomationV2SendStep,
-    BadRequest,
-    BadRequestError,
-    BaseCheck,
-    BaseError,
-    BaseFilterConfig,
-    BaseMessage,
-    BaseSocialPresence,
-    BlockType,
+    MergeAlgorithm,
+    Profile,
+)
+from .brands import (
     Brand,
     BrandColors,
     BrandGetAllResponse,
     BrandParameters,
     BrandSettings,
-    BrandSettingsEmail,
-    BrandSettingsInApp,
-    BrandSettingsSocialPresence,
     BrandSnippet,
     BrandSnippets,
-    BrandTemplate,
-    BrandTemplateOverride,
     BrandsResponse,
+)
+from .bulk import (
     BulkCreateJobResponse,
     BulkGetJobParams,
     BulkGetJobResponse,
     BulkGetJobUsersParams,
     BulkGetJobUsersResponse,
     BulkIngestError,
     BulkIngestUsersParams,
     BulkIngestUsersResponse,
     BulkJobStatus,
     BulkJobUserStatus,
     BulkMessageUserResponse,
-    Channel,
+    InboundBulkContentMessage,
+    InboundBulkMessage,
+    InboundBulkMessageUser,
+    InboundBulkMessageV1,
+    InboundBulkMessageV2,
+    InboundBulkTemplateMessage,
+    JobDetails,
+)
+from .commons import (
+    AlreadyExists,
+    AlreadyExistsError,
+    BadRequest,
+    BadRequestError,
+    BaseError,
     ChannelClassification,
-    ChannelIdentifier,
-    ChannelMetadata,
     ChannelPreference,
-    ChannelSource,
-    Check,
-    CheckStatus,
-    ComparisonOperator,
     Conflict,
     ConflictError,
+    Email,
+    MessageNotFound,
+    MessageNotFoundError,
+    NotFound,
+    NotFoundError,
+    NotificationPreferenceDetails,
+    NotificationPreferences,
+    Paging,
+    PaymentRequired,
+    PaymentRequiredError,
+    PreferenceStatus,
+    RecipientPreferences,
+    Rule,
+    UserTenantAssociation,
+)
+from .environment import CourierEnvironment
+from .lists import (
+    List,
+    ListGetAllResponse,
+    ListGetSubscriptionsResponse,
+    ListPutParams,
+    ListSubscriptionRecipient,
+    PutSubscriptionsRecipient,
+)
+from .messages import (
+    ListMessagesResponse,
+    MessageDetails,
+    MessageHistoryResponse,
+    MessageStatus,
+    Reason,
+    RenderOutput,
+    RenderOutputResponse,
+    RenderedMessageBlock,
+    RenderedMessageContent,
+)
+from .notifications import (
+    BaseCheck,
+    BlockType,
+    Check,
+    CheckStatus,
+    MessageRouting,
+    MessageRoutingChannel,
+    MessageRoutingMethod,
+    Notification,
+    NotificationBlock,
+    NotificationChannel,
+    NotificationChannelContent,
+    NotificationContent,
+    NotificationContentHierarchy,
+    NotificationGetContentResponse,
+    NotificationListResponse,
+    SubmissionChecksGetResponse,
+    SubmissionChecksReplaceResponse,
+)
+from .profiles import (
+    Address,
+    AirshipProfile,
+    AirshipProfileAudience,
+    DeleteListSubscriptionResponse,
+    DeviceType,
+    Discord,
+    Expo,
+    GetListSubscriptionsList,
+    GetListSubscriptionsResponse,
+    Intercom,
+    IntercomRecipient,
+    MergeProfileResponse,
+    MsTeams,
+    MsTeamsBaseProperties,
+    MultipleTokens,
+    ProfileGetParameters,
+    ProfileGetResponse,
+    ReplaceProfileResponse,
+    SendDirectMessage,
+    SendToChannel,
+    SendToMsTeamsChannelId,
+    SendToMsTeamsChannelName,
+    SendToMsTeamsConversationId,
+    SendToMsTeamsEmail,
+    SendToMsTeamsUserId,
+    SendToSlackChannel,
+    SendToSlackEmail,
+    SendToSlackUserId,
+    Slack,
+    SlackBaseProperties,
+    SnoozeRule,
+    SnoozeRuleType,
+    SubscribeToListsRequest,
+    SubscribeToListsRequestListObject,
+    SubscribeToListsResponse,
+    Token,
+    UserProfile,
+)
+from .send import (
+    Attachment,
+    AudienceFilter,
+    AudienceRecipient,
+    BaseMessage,
+    BaseMessageSendTo,
+    BaseSocialPresence,
+    BrandSettingsEmail,
+    BrandSettingsInApp,
+    BrandSettingsSocialPresence,
+    BrandTemplate,
+    BrandTemplateOverride,
+    Channel,
+    ChannelMetadata,
+    ChannelSource,
     Content,
     ContentMessage,
     Criteria,
-    DefaultPreferences,
     Delay,
-    DeleteListSubscriptionResponse,
-    DeviceType,
-    Discord,
     ElementalActionNode,
     ElementalBaseNode,
     ElementalChannelNode,
     ElementalContent,
     ElementalContentSugar,
     ElementalDividerNode,
     ElementalGroupNode,
@@ -101,196 +237,92 @@
     ElementalNode_Group,
     ElementalNode_Image,
     ElementalNode_Meta,
     ElementalNode_Quote,
     ElementalNode_Text,
     ElementalQuoteNode,
     ElementalTextNode,
-    Email,
     EmailFooter,
     EmailHead,
     EmailHeader,
     ExpiresInType,
     Expiry,
-    Expo,
-    Filter,
-    FilterConfig,
-    GetAuditEventParams,
-    GetListSubscriptionsList,
-    GetListSubscriptionsResponse,
     IActionButtonStyle,
     IAlignment,
     IPreferences,
     IProfilePreferences,
     Icons,
     InAppPlacement,
-    InboundBulkContentMessage,
-    InboundBulkMessage,
-    InboundBulkMessageUser,
-    InboundBulkMessageV1,
-    InboundBulkMessageV2,
-    InboundBulkTemplateMessage,
-    Intercom,
-    IntercomRecipient,
     InvalidListPatternRecipient,
     InvalidListRecipient,
     InvalidUserRecipient,
-    IssueTokenResponse,
-    JobDetails,
-    List,
-    ListAuditEventsParams,
-    ListAuditEventsResponse,
     ListFilter,
-    ListFindByRecipientIdParams,
-    ListFindByRecipientIdResponse,
-    ListGetAllParams,
-    ListGetAllResponse,
-    ListGetSubscriptionsParams,
-    ListGetSubscriptionsResponse,
-    ListMessagesResponse,
     ListPatternRecipient,
     ListPatternRecipientType,
-    ListPutParams,
     ListRecipient,
     ListRecipientType,
-    ListSubscriptionRecipient,
-    ListTemplatesResponse,
-    ListUsersForTenantResponse,
     Locale,
     Locales,
-    LogicalOperator,
     Logo,
-    MergeAlgorithm,
-    MergeProfileResponse,
     Message,
     MessageChannelEmailOverride,
     MessageChannels,
     MessageContext,
     MessageData,
-    MessageDetails,
-    MessageHistoryResponse,
     MessageMetadata,
-    MessageNotFound,
-    MessageNotFoundError,
     MessageProviders,
     MessageProvidersType,
     MessageRecipient,
-    MessageRouting,
-    MessageRoutingChannel,
-    MessageRoutingMethod,
-    MessageStatus,
     Metadata,
-    MsTeams,
-    MsTeamsBaseProperties,
-    MultipleTokens,
-    NestedFilterConfig,
-    NotFound,
-    NotFoundError,
-    Notification,
-    NotificationBlock,
-    NotificationChannel,
-    NotificationChannelContent,
-    NotificationContent,
-    NotificationContentHierarchy,
-    NotificationGetContentResponse,
-    NotificationListResponse,
-    NotificationPreferenceDetails,
-    NotificationPreferences,
-    NotificationTemplates,
-    Operator,
+    MsTeamsRecipient,
     Override,
-    Paging,
-    PaymentRequired,
-    PaymentRequiredError,
     Preference,
-    PreferenceStatus,
     Preferences,
-    Profile,
-    ProfileGetParameters,
-    ProfileGetResponse,
-    PutSubscriptionsRecipient,
-    Reason,
     Recipient,
-    RecipientPreferences,
-    RecipientSubscriptionsResponse,
-    RenderOutput,
-    RenderOutputResponse,
-    RenderedMessageBlock,
-    RenderedMessageContent,
-    ReplaceProfileResponse,
+    RecipientData,
     Routing,
     RoutingChannel,
     RoutingMethod,
-    RoutingStrategy,
     RoutingStrategyChannel,
-    RoutingStrategyMethod,
     RoutingStrategyProvider,
-    Rule,
     RuleType,
-    SendDirectMessage,
-    SendToChannel,
-    SendToMsTeamsChannelId,
-    SendToMsTeamsChannelName,
-    SendToMsTeamsConversationId,
-    SendToMsTeamsEmail,
-    SendToMsTeamsUserId,
-    SendToSlackChannel,
-    SendToSlackEmail,
-    SendToSlackUserId,
-    SingleFilterConfig,
-    Slack,
-    SlackBaseProperties,
-    SnoozeRule,
-    SnoozeRuleType,
-    SubmissionChecksGetResponse,
-    SubmissionChecksReplaceResponse,
-    SubscribeToListsRequest,
-    SubscribeToListsRequestListObject,
-    SubscribeToListsResponse,
-    SubscriptionTopic,
-    SubscriptionTopicStatus,
-    Tag,
-    TagData,
-    Target,
+    SlackRecipient,
     TemplateMessage,
-    TemplateProperty,
-    Tenant,
-    TenantListResponse,
     TextAlign,
     TextStyle,
     Timeout,
     Timeouts,
-    Token,
     TrackingOverride,
-    UserProfile,
     UserRecipient,
     UserRecipientType,
-    UserTenantAssociation,
     Utm,
     WidgetBackground,
-    audiences,
-    audit_events,
-    auth_tokens,
-    automations,
-    brands,
-    bulk,
-    commons,
-    lists,
-    messages,
-    notifications,
-    profiles,
-    send,
-    templates,
-    tenants,
-    translations,
-    users,
 )
-from .environment import CourierEnvironment
+from .templates import (
+    ChannelIdentifier,
+    ListTemplatesResponse,
+    NotificationTemplates,
+    RoutingStrategy,
+    RoutingStrategyMethod,
+    Tag,
+    TagData,
+)
+from .tenants import (
+    DefaultPreferences,
+    ListUsersForTenantResponse,
+    SubscriptionTopic,
+    SubscriptionTopicStatus,
+    TemplateProperty,
+    Tenant,
+    TenantListResponse,
+)
+from .version import __version__
 
 __all__ = [
+    "AccessorType",
     "Actor",
     "Address",
     "AirshipProfile",
     "AirshipProfileAudience",
     "AlreadyExists",
     "AlreadyExistsError",
     "Attachment",
@@ -301,34 +333,46 @@
     "AudienceMemberGetResponse",
     "AudienceMemberListResponse",
     "AudienceRecipient",
     "AudienceUpdateResponse",
     "AuditEvent",
     "Automation",
     "AutomationAdHocInvokeParams",
+    "AutomationAddToBatchMaxItemsType",
+    "AutomationAddToBatchRetain",
+    "AutomationAddToBatchRetainType",
+    "AutomationAddToBatchScope",
+    "AutomationAddToBatchStep",
+    "AutomationAddToDigestStep",
     "AutomationCancelStep",
     "AutomationDelayStep",
+    "AutomationFetchDataStep",
+    "AutomationFetchDataWebhook",
+    "AutomationFetchDataWebhookMethod",
     "AutomationInvokeParams",
     "AutomationInvokeResponse",
     "AutomationInvokeStep",
     "AutomationInvokeTemplateParams",
     "AutomationRunContext",
     "AutomationSendListStep",
     "AutomationSendStep",
     "AutomationStep",
-    "AutomationStepAction",
     "AutomationStepOption",
+    "AutomationThrottleOnThrottle",
+    "AutomationThrottleScope",
+    "AutomationThrottleStep",
     "AutomationUpdateProfileStep",
     "AutomationV2SendStep",
     "BadRequest",
     "BadRequestError",
     "BaseCheck",
     "BaseError",
     "BaseFilterConfig",
     "BaseMessage",
+    "BaseMessageSendTo",
     "BaseSocialPresence",
     "BlockType",
     "Brand",
     "BrandColors",
     "BrandGetAllResponse",
     "BrandParameters",
     "BrandSettings",
@@ -422,19 +466,15 @@
     "InvalidUserRecipient",
     "IssueTokenResponse",
     "JobDetails",
     "List",
     "ListAuditEventsParams",
     "ListAuditEventsResponse",
     "ListFilter",
-    "ListFindByRecipientIdParams",
-    "ListFindByRecipientIdResponse",
-    "ListGetAllParams",
     "ListGetAllResponse",
-    "ListGetSubscriptionsParams",
     "ListGetSubscriptionsResponse",
     "ListMessagesResponse",
     "ListPatternRecipient",
     "ListPatternRecipientType",
     "ListPutParams",
     "ListRecipient",
     "ListRecipientType",
@@ -463,14 +503,15 @@
     "MessageRouting",
     "MessageRoutingChannel",
     "MessageRoutingMethod",
     "MessageStatus",
     "Metadata",
     "MsTeams",
     "MsTeamsBaseProperties",
+    "MsTeamsRecipient",
     "MultipleTokens",
     "NestedFilterConfig",
     "NotFound",
     "NotFoundError",
     "Notification",
     "NotificationBlock",
     "NotificationChannel",
@@ -492,16 +533,16 @@
     "Preferences",
     "Profile",
     "ProfileGetParameters",
     "ProfileGetResponse",
     "PutSubscriptionsRecipient",
     "Reason",
     "Recipient",
+    "RecipientData",
     "RecipientPreferences",
-    "RecipientSubscriptionsResponse",
     "RenderOutput",
     "RenderOutputResponse",
     "RenderedMessageBlock",
     "RenderedMessageContent",
     "ReplaceProfileResponse",
     "Routing",
     "RoutingChannel",
@@ -522,14 +563,15 @@
     "SendToMsTeamsUserId",
     "SendToSlackChannel",
     "SendToSlackEmail",
     "SendToSlackUserId",
     "SingleFilterConfig",
     "Slack",
     "SlackBaseProperties",
+    "SlackRecipient",
     "SnoozeRule",
     "SnoozeRuleType",
     "SubmissionChecksGetResponse",
     "SubmissionChecksReplaceResponse",
     "SubscribeToListsRequest",
     "SubscribeToListsRequestListObject",
     "SubscribeToListsResponse",
@@ -550,14 +592,15 @@
     "TrackingOverride",
     "UserProfile",
     "UserRecipient",
     "UserRecipientType",
     "UserTenantAssociation",
     "Utm",
     "WidgetBackground",
+    "__version__",
     "audiences",
     "audit_events",
     "auth_tokens",
     "automations",
     "brands",
     "bulk",
     "commons",
```

### Comparing `trycourier-6.0.0b1/src/courier/core/client_wrapper.py` & `trycourier-6.0.1/src/courier/core/client_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
 import httpx
 
+from .http_client import AsyncHttpClient, HttpClient
+
 
 class BaseClientWrapper:
-    def __init__(self, *, authorization_token: typing.Union[str, typing.Callable[[], str]], base_url: str):
+    def __init__(
+        self,
+        *,
+        authorization_token: typing.Union[str, typing.Callable[[], str]],
+        base_url: str,
+        timeout: typing.Optional[float] = None,
+    ):
         self._authorization_token = authorization_token
         self._base_url = base_url
+        self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "trycourier",
-            "X-Fern-SDK-Version": "v6.0.0b1",
+            "X-Fern-SDK-Version": "v6.0.1",
         }
         headers["Authorization"] = f"Bearer {self._get_authorization_token()}"
         return headers
 
     def _get_authorization_token(self) -> str:
         if isinstance(self._authorization_token, str):
             return self._authorization_token
         else:
             return self._authorization_token()
 
     def get_base_url(self) -> str:
         return self._base_url
 
+    def get_timeout(self) -> typing.Optional[float]:
+        return self._timeout
+
 
 class SyncClientWrapper(BaseClientWrapper):
     def __init__(
         self,
         *,
         authorization_token: typing.Union[str, typing.Callable[[], str]],
         base_url: str,
+        timeout: typing.Optional[float] = None,
         httpx_client: httpx.Client,
     ):
-        super().__init__(authorization_token=authorization_token, base_url=base_url)
-        self.httpx_client = httpx_client
+        super().__init__(authorization_token=authorization_token, base_url=base_url, timeout=timeout)
+        self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
     def __init__(
         self,
         *,
         authorization_token: typing.Union[str, typing.Callable[[], str]],
         base_url: str,
+        timeout: typing.Optional[float] = None,
         httpx_client: httpx.AsyncClient,
     ):
-        super().__init__(authorization_token=authorization_token, base_url=base_url)
-        self.httpx_client = httpx_client
+        super().__init__(authorization_token=authorization_token, base_url=base_url, timeout=timeout)
+        self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `trycourier-6.0.0b1/src/courier/core/datetime_utils.py` & `trycourier-6.0.1/src/courier/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/core/jsonable_encoder.py` & `trycourier-6.0.1/src/courier/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic.json.ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, pydantic.BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -61,18 +57,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
@@ -80,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in pydantic.json.ENCODERS_BY_TYPE:
-        return pydantic.json.ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/__init__.py` & `trycourier-6.0.1/src/courier/audiences/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/__init__.py` & `trycourier-6.0.1/src/courier/audiences/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience.py` & `trycourier-6.0.1/src/courier/messages/types/render_output_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .filter import Filter
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .render_output import RenderOutput
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Audience(pydantic.BaseModel):
-    id: str = pydantic.Field(description="A unique identifier representing the audience_id")
-    name: str = pydantic.Field(description="The name of the audience")
-    description: str = pydantic.Field(description="A description of the audience")
-    filter: Filter
-    created_at: str
-    updated_at: str
+
+class RenderOutputResponse(pydantic_v1.BaseModel):
+    results: typing.List[RenderOutput] = pydantic_v1.Field()
+    """
+    An array of render output of a previously sent message.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_list_response.py` & `trycourier-6.0.1/src/courier/users/preferences/types/user_preferences_update_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .audience import Audience
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudienceListResponse(pydantic.BaseModel):
-    items: typing.List[Audience]
-    paging: Paging
+class UserPreferencesUpdateResponse(pydantic_v1.BaseModel):
+    message: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member.py` & `trycourier-6.0.1/src/courier/commons/types/conflict.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_error import BaseError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudienceMember(pydantic.BaseModel):
-    added_at: str
-    audience_id: str
-    audience_version: int
-    member_id: str
-    reason: str
+class Conflict(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_get_response.py` & `trycourier-6.0.1/src/courier/audiences/types/audience_member_get_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .audience_member import AudienceMember
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudienceMemberGetResponse(pydantic.BaseModel):
-    audience_member: AudienceMember = pydantic.Field(alias="audienceMember")
+class AudienceMemberGetResponse(pydantic_v1.BaseModel):
+    audience_member: AudienceMember = pydantic_v1.Field(alias="audienceMember")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_member_list_response.py` & `trycourier-6.0.1/src/courier/audiences/types/audience_list_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.paging import Paging
-from .audience_member import AudienceMember
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .audience import Audience
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudienceMemberListResponse(pydantic.BaseModel):
-    items: typing.List[AudienceMember]
+class AudienceListResponse(pydantic_v1.BaseModel):
+    items: typing.List[Audience]
     paging: Paging
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/audience_update_response.py` & `trycourier-6.0.1/src/courier/send/types/base_social_presence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .audience import Audience
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudienceUpdateResponse(pydantic.BaseModel):
-    audience: Audience
+class BaseSocialPresence(pydantic_v1.BaseModel):
+    url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/base_filter_config.py` & `trycourier-6.0.1/src/courier/audiences/types/base_filter_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .operator import Operator
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BaseFilterConfig(pydantic.BaseModel):
-    operator: Operator = pydantic.Field(description="The operator to use for filtering")
+class BaseFilterConfig(pydantic_v1.BaseModel):
+    operator: Operator = pydantic_v1.Field()
+    """
+    The operator to use for filtering
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/nested_filter_config.py` & `trycourier-6.0.1/src/courier/send/types/audience_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .base_filter_config import BaseFilterConfig
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class NestedFilterConfig(BaseFilterConfig):
+class AudienceFilter(pydantic_v1.BaseModel):
+    operator: typing.Literal["MEMBER_OF"] = pydantic_v1.Field()
     """
-    The operator to use for filtering
+    Send to users only if they are member of the account
     """
 
-    rules: typing.List[FilterConfig]
+    path: typing.Literal["account_id"]
+    value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .filter_config import FilterConfig  # noqa: E402
-
-NestedFilterConfig.update_forward_refs()
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audiences/types/single_filter_config.py` & `trycourier-6.0.1/src/courier/users/tenants/types/list_tenants_for_user_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ....commons.types.user_tenant_association import UserTenantAssociation
 from ....core.datetime_utils import serialize_datetime
-from .base_filter_config import BaseFilterConfig
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ListTenantsForUserResponse(pydantic_v1.BaseModel):
+    items: typing.Optional[typing.List[UserTenantAssociation]] = None
+    has_more: bool = pydantic_v1.Field()
+    """
+    Set to true when there are more pages that can be retrieved.
+    """
+
+    url: str = pydantic_v1.Field()
+    """
+    A url that may be used to generate these results.
+    """
 
-class SingleFilterConfig(BaseFilterConfig):
+    next_url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    A single filter to use for filtering
+    A url that may be used to generate fetch the next set of results.
+    Defined only when `has_more` is set to true
     """
 
-    value: str = pydantic.Field(description="The value to use for filtering")
-    path: str = pydantic.Field(
-        description="The attribe name from profile whose value will be operated against the filter value"
-    )
+    cursor: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A pointer to the next page of results. Defined
+    only when `has_more` is set to true
+    """
+
+    type: typing.Literal["list"] = pydantic_v1.Field()
+    """
+    Always set to `list`. Represents the type of this object.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audit_events/types/actor.py` & `trycourier-6.0.1/src/courier/send/types/timeouts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Actor(pydantic.BaseModel):
-    id: typing.Optional[str]
-    email: typing.Optional[str]
+class Timeouts(pydantic_v1.BaseModel):
+    provider: typing.Optional[int] = None
+    channel: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audit_events/types/audit_event.py` & `trycourier-6.0.1/src/courier/notifications/types/notification_list_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .actor import Actor
-from .target import Target
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class AuditEvent(pydantic.BaseModel):
-    actor: typing.Optional[Actor]
-    target: typing.Optional[Target]
-    audit_event_id: str = pydantic.Field(alias="auditEventId")
-    source: str
-    timestamp: str
-    type: str
+from ...commons.types.paging import Paging
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .notification import Notification
+
+
+class NotificationListResponse(pydantic_v1.BaseModel):
+    paging: Paging
+    results: typing.List[Notification]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audit_events/types/get_audit_event_params.py` & `trycourier-6.0.1/src/courier/auth_tokens/types/issue_token_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetAuditEventParams(pydantic.BaseModel):
-    audit_event_id: str = pydantic.Field(alias="auditEventId")
+class IssueTokenResponse(pydantic_v1.BaseModel):
+    token: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_params.py` & `trycourier-6.0.1/src/courier/notifications/types/check.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_check import BaseCheck
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListAuditEventsParams(pydantic.BaseModel):
-    cursor: typing.Optional[str]
+class Check(BaseCheck):
+    updated: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audit_events/types/list_audit_events_response.py` & `trycourier-6.0.1/src/courier/profiles/types/airship_profile_audience.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .audit_event import AuditEvent
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class ListAuditEventsResponse(pydantic.BaseModel):
-    paging: Paging
-    results: typing.List[AuditEvent]
+class AirshipProfileAudience(pydantic_v1.BaseModel):
+    named_user: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/audit_events/types/target.py` & `trycourier-6.0.1/src/courier/profiles/types/multiple_tokens.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .token import Token
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Target(pydantic.BaseModel):
-    id: typing.Optional[str]
-    email: typing.Optional[str]
+class MultipleTokens(pydantic_v1.BaseModel):
+    tokens: typing.List[Token]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/auth_tokens/types/issue_token_response.py` & `trycourier-6.0.1/src/courier/audit_events/types/list_audit_events_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class IssueTokenResponse(pydantic.BaseModel):
-    token: typing.Optional[str]
+class ListAuditEventsParams(pydantic_v1.BaseModel):
+    cursor: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/__init__.py` & `trycourier-6.0.1/src/courier/automations/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,67 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
+    AccessorType,
     Automation,
     AutomationAdHocInvokeParams,
+    AutomationAddToBatchMaxItemsType,
+    AutomationAddToBatchRetain,
+    AutomationAddToBatchRetainType,
+    AutomationAddToBatchScope,
+    AutomationAddToBatchStep,
+    AutomationAddToDigestStep,
     AutomationCancelStep,
     AutomationDelayStep,
+    AutomationFetchDataStep,
+    AutomationFetchDataWebhook,
+    AutomationFetchDataWebhookMethod,
     AutomationInvokeParams,
     AutomationInvokeResponse,
     AutomationInvokeStep,
     AutomationInvokeTemplateParams,
     AutomationRunContext,
     AutomationSendListStep,
     AutomationSendStep,
     AutomationStep,
-    AutomationStepAction,
     AutomationStepOption,
+    AutomationThrottleOnThrottle,
+    AutomationThrottleScope,
+    AutomationThrottleStep,
     AutomationUpdateProfileStep,
     AutomationV2SendStep,
     MergeAlgorithm,
     Profile,
 )
 
 __all__ = [
+    "AccessorType",
     "Automation",
     "AutomationAdHocInvokeParams",
+    "AutomationAddToBatchMaxItemsType",
+    "AutomationAddToBatchRetain",
+    "AutomationAddToBatchRetainType",
+    "AutomationAddToBatchScope",
+    "AutomationAddToBatchStep",
+    "AutomationAddToDigestStep",
     "AutomationCancelStep",
     "AutomationDelayStep",
+    "AutomationFetchDataStep",
+    "AutomationFetchDataWebhook",
+    "AutomationFetchDataWebhookMethod",
     "AutomationInvokeParams",
     "AutomationInvokeResponse",
     "AutomationInvokeStep",
     "AutomationInvokeTemplateParams",
     "AutomationRunContext",
     "AutomationSendListStep",
     "AutomationSendStep",
     "AutomationStep",
-    "AutomationStepAction",
     "AutomationStepOption",
+    "AutomationThrottleOnThrottle",
+    "AutomationThrottleScope",
+    "AutomationThrottleStep",
     "AutomationUpdateProfileStep",
     "AutomationV2SendStep",
     "MergeAlgorithm",
     "Profile",
 ]
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation.py` & `trycourier-6.0.1/src/courier/automations/types/automation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .automation_step_option import AutomationStepOption
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Automation(pydantic.BaseModel):
-    cancelation_token: typing.Optional[str]
+class Automation(pydantic_v1.BaseModel):
+    cancelation_token: typing.Optional[str] = None
     steps: typing.List[AutomationStepOption]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_ad_hoc_invoke_params.py` & `trycourier-6.0.1/src/courier/automations/types/automation_ad_hoc_invoke_params.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .automation import Automation
 from .automation_invoke_params import AutomationInvokeParams
 
 
 class AutomationAdHocInvokeParams(AutomationInvokeParams):
     automation: Automation
 
@@ -19,8 +20,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_cancel_step.py` & `trycourier-6.0.1/src/courier/commons/types/payment_required.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_error import BaseError
 
-from ....core.datetime_utils import serialize_datetime
-from .automation_step import AutomationStep
 
-
-class AutomationCancelStep(AutomationStep):
-    action: typing_extensions.Literal["cancel"]
-    cancelation_token: typing.Optional[str]
+class PaymentRequired(BaseError):
+    type: typing.Literal["authorization_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_delay_step.py` & `trycourier-6.0.1/src/courier/templates/types/tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .tag_data import TagData
 
-from ....core.datetime_utils import serialize_datetime
-from .automation_step import AutomationStep
 
-
-class AutomationDelayStep(AutomationStep):
-    action: typing_extensions.Literal["delay"]
-    until: typing.Optional[str]
+class Tag(pydantic_v1.BaseModel):
+    data: typing.List[TagData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_params.py` & `trycourier-6.0.1/src/courier/send/types/logo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .profile import Profile
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AutomationInvokeParams(pydantic.BaseModel):
-    brand: typing.Optional[str]
-    data: typing.Optional[typing.Dict[str, typing.Any]]
-    profile: typing.Optional[Profile]
-    recipient: typing.Optional[str]
-    template: typing.Optional[str]
+class Logo(pydantic_v1.BaseModel):
+    href: typing.Optional[str] = None
+    image: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_response.py` & `trycourier-6.0.1/src/courier/send/types/email_footer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AutomationInvokeResponse(pydantic.BaseModel):
-    run_id: str = pydantic.Field(alias="runId")
+class EmailFooter(pydantic_v1.BaseModel):
+    content: typing.Optional[typing.Any] = None
+    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_step.py` & `trycourier-6.0.1/src/courier/send/types/slack_recipient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...profiles.types.slack import Slack
 
-from ....core.datetime_utils import serialize_datetime
-from .automation_step import AutomationStep
 
-
-class AutomationInvokeStep(AutomationStep):
-    action: typing_extensions.Literal["invoke"]
-    template: str
+class SlackRecipient(pydantic_v1.BaseModel):
+    slack: Slack
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_invoke_template_params.py` & `trycourier-6.0.1/src/courier/automations/types/automation_send_list_step.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .automation_invoke_params import AutomationInvokeParams
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_step import AutomationStep
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AutomationInvokeTemplateParams(AutomationInvokeParams):
-    template_id: str = pydantic.Field(alias="templateId")
+class AutomationSendListStep(AutomationStep):
+    action: typing.Literal["send-list"]
+    brand: typing.Optional[str] = None
+    data: typing.Optional[typing.Dict[str, typing.Any]] = None
+    list_: str = pydantic_v1.Field(alias="list")
+    override: typing.Optional[typing.Dict[str, typing.Any]] = None
+    template: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_run_context.py` & `trycourier-6.0.1/src/courier/automations/types/automation_invoke_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .profile import Profile
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AutomationRunContext(pydantic.BaseModel):
-    brand: typing.Optional[str]
-    data: typing.Optional[typing.Any]
-    profile: typing.Optional[Profile]
-    template: typing.Optional[str]
-    recipient: typing.Optional[str]
+class AutomationInvokeParams(pydantic_v1.BaseModel):
+    brand: typing.Optional[str] = None
+    data: typing.Optional[typing.Dict[str, typing.Any]] = None
+    profile: typing.Optional[Profile] = None
+    recipient: typing.Optional[str] = None
+    template: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_list_step.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_conversation_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
-from ....core.datetime_utils import serialize_datetime
-from .automation_step import AutomationStep
 
-
-class AutomationSendListStep(AutomationStep):
-    action: typing_extensions.Literal["send-list"]
-    brand: typing.Optional[str]
-    data: typing.Optional[typing.Dict[str, typing.Any]]
-    list: str
-    override: typing.Optional[typing.Dict[str, typing.Any]]
-    template: typing.Optional[str]
+class SendToMsTeamsConversationId(MsTeamsBaseProperties):
+    conversation_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_send_step.py` & `trycourier-6.0.1/src/courier/commons/types/email.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
-from .automation_step import AutomationStep
 
-
-class AutomationSendStep(AutomationStep):
-    action: typing_extensions.Literal["send"]
-    brand: typing.Optional[str]
-    data: typing.Optional[typing.Dict[str, typing.Any]]
-    override: typing.Optional[typing.Dict[str, typing.Any]]
-    profile: typing.Optional[typing.Any]
-    recipient: typing.Optional[str]
-    template: typing.Optional[str]
+class Email(pydantic_v1.BaseModel):
+    footer: typing.Any
+    header: typing.Any
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step.py` & `trycourier-6.0.1/src/courier/profiles/types/airship_profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .airship_profile_audience import AirshipProfileAudience
+from .device_type import DeviceType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AutomationStep(pydantic.BaseModel):
-    if_: typing.Optional[str] = pydantic.Field(alias="if")
-    ref: typing.Optional[str]
+class AirshipProfile(pydantic_v1.BaseModel):
+    audience: AirshipProfileAudience
+    device_types: typing.List[DeviceType]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_step_option.py` & `trycourier-6.0.1/src/courier/automations/types/automation_step_option.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
+from .automation_add_to_batch_step import AutomationAddToBatchStep
+from .automation_add_to_digest_step import AutomationAddToDigestStep
 from .automation_cancel_step import AutomationCancelStep
 from .automation_delay_step import AutomationDelayStep
+from .automation_fetch_data_step import AutomationFetchDataStep
 from .automation_invoke_step import AutomationInvokeStep
 from .automation_send_list_step import AutomationSendListStep
 from .automation_send_step import AutomationSendStep
+from .automation_throttle_step import AutomationThrottleStep
 from .automation_update_profile_step import AutomationUpdateProfileStep
 from .automation_v_2_send_step import AutomationV2SendStep
 
 AutomationStepOption = typing.Union[
+    AutomationAddToDigestStep,
+    AutomationAddToBatchStep,
+    AutomationThrottleStep,
     AutomationCancelStep,
     AutomationDelayStep,
+    AutomationFetchDataStep,
     AutomationInvokeStep,
     AutomationSendStep,
     AutomationV2SendStep,
     AutomationSendListStep,
     AutomationUpdateProfileStep,
 ]
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_update_profile_step.py` & `trycourier-6.0.1/src/courier/automations/types/automation_cancel_step.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_step import AutomationStep
 
-from ....core.datetime_utils import serialize_datetime
-from .merge_algorithm import MergeAlgorithm
-from .profile import Profile
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class AutomationUpdateProfileStep(pydantic.BaseModel):
-    action: typing_extensions.Literal["update-profile"]
-    recipient_id: str
-    profile: Profile
-    merge: MergeAlgorithm
+
+class AutomationCancelStep(AutomationStep):
+    action: typing.Literal["cancel"]
+    cancelation_token: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/automations/types/automation_v_2_send_step.py` & `trycourier-6.0.1/src/courier/automations/types/automation_v_2_send_step.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
-
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from ...send.types.message import Message
 from .automation_step import AutomationStep
 
 
 class AutomationV2SendStep(AutomationStep):
-    action: typing_extensions.Literal["send"]
+    action: typing.Literal["send"]
     message: Message
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/__init__.py` & `trycourier-6.0.1/src/courier/brands/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brand.py` & `trycourier-6.0.1/src/courier/brands/types/brand.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .brand_settings import BrandSettings
 from .brand_snippets import BrandSnippets
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class Brand(pydantic_v1.BaseModel):
+    created: int = pydantic_v1.Field()
+    """
+    The date/time of when the brand was created. Represented in milliseconds since Unix epoch.
+    """
+
+    id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Brand Identifier
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    Brand name
+    """
+
+    published: int = pydantic_v1.Field()
+    """
+    The date/time of when the brand was published. Represented in milliseconds since Unix epoch.
+    """
 
-class Brand(pydantic.BaseModel):
-    created: int = pydantic.Field(
-        description="The date/time of when the brand was created. Represented in milliseconds since Unix epoch."
-    )
-    id: typing.Optional[str] = pydantic.Field(description="Brand Identifier")
-    name: str = pydantic.Field(description="Brand name")
-    published: int = pydantic.Field(
-        description="The date/time of when the brand was published. Represented in milliseconds since Unix epoch."
-    )
     settings: BrandSettings
-    updated: int = pydantic.Field(
-        description="The date/time of when the brand was updated. Represented in milliseconds since Unix epoch."
-    )
-    snippets: typing.Optional[BrandSnippets]
-    version: str = pydantic.Field(description="The version identifier for the brand")
+    updated: int = pydantic_v1.Field()
+    """
+    The date/time of when the brand was updated. Represented in milliseconds since Unix epoch.
+    """
+
+    snippets: typing.Optional[BrandSnippets] = None
+    version: str = pydantic_v1.Field()
+    """
+    The version identifier for the brand
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_colors.py` & `trycourier-6.0.1/src/courier/profiles/types/token.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BrandColors(pydantic.BaseModel):
-    primary: typing.Optional[str]
-    secondary: typing.Optional[str]
-    tertiary: typing.Optional[str]
+class Token(pydantic_v1.BaseModel):
+    token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_get_all_response.py` & `trycourier-6.0.1/src/courier/profiles/types/ms_teams_base_properties.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .brand import Brand
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class BrandGetAllResponse(pydantic.BaseModel):
-    paging: Paging
-    results: typing.List[Brand]
+class MsTeamsBaseProperties(pydantic_v1.BaseModel):
+    tenant_id: str
+    service_url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_parameters.py` & `trycourier-6.0.1/src/courier/brands/types/brand_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .brand_settings import BrandSettings
 from .brand_snippets import BrandSnippets
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class BrandParameters(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
+    """
+    The name of the brand.
+    """
 
-class BrandParameters(pydantic.BaseModel):
-    id: typing.Optional[str]
-    name: str = pydantic.Field(description="The name of the brand.")
     settings: BrandSettings
-    snippets: typing.Optional[BrandSnippets]
+    snippets: typing.Optional[BrandSnippets] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_settings.py` & `trycourier-6.0.1/src/courier/notifications/types/notification_channel_content.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.email import Email
-from .brand_colors import BrandColors
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class BrandSettings(pydantic.BaseModel):
-    colors: typing.Optional[BrandColors]
-    inapp: typing.Optional[typing.Any]
-    email: typing.Optional[Email]
+class NotificationChannelContent(pydantic_v1.BaseModel):
+    subject: typing.Optional[str] = None
+    title: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippet.py` & `trycourier-6.0.1/src/courier/profiles/types/slack_base_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BrandSnippet(pydantic.BaseModel):
-    format: typing_extensions.Literal["handlebars"]
-    name: str
-    value: str
+class SlackBaseProperties(pydantic_v1.BaseModel):
+    access_token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brand_snippets.py` & `trycourier-6.0.1/src/courier/send/types/list_recipient_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .brand_snippet import BrandSnippet
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BrandSnippets(pydantic.BaseModel):
-    items: typing.List[BrandSnippet]
 
+class ListRecipientType(pydantic_v1.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/brands/types/brands_response.py` & `trycourier-6.0.1/src/courier/users/tokens/types/get_user_token_opts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .brand import Brand
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BrandsResponse(pydantic.BaseModel):
-    paging: Paging
-    results: typing.List[Brand]
+class GetUserTokenOpts(pydantic_v1.BaseModel):
+    user_id: str
+    token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/__init__.py` & `trycourier-6.0.1/src/courier/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/__init__.py` & `trycourier-6.0.1/src/courier/bulk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_create_job_response.py` & `trycourier-6.0.1/src/courier/automations/types/automation_delay_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BulkCreateJobResponse(pydantic.BaseModel):
-    job_id: str = pydantic.Field(alias="jobId")
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_step import AutomationStep
+
+
+class AutomationDelayStep(AutomationStep):
+    action: typing.Literal["delay"]
+    duration: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The [ISO 8601 duration](https://en.wikipedia.org/wiki/ISO_8601#Durations) string for how long to delay for
+    """
+
+    until: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The ISO 8601 timestamp for when the delay should end
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_params.py` & `trycourier-6.0.1/src/courier/send/types/elemental_group_node.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .elemental_base_node import ElementalBaseNode
 
 
-class BulkGetJobParams(pydantic.BaseModel):
-    job_id: str = pydantic.Field(alias="jobId")
+class ElementalGroupNode(ElementalBaseNode):
+    """
+    Allows you to group elements together. This can be useful when used in combination with "if" or "loop". See [control flow docs](https://www.courier.com/docs/platform/content/elemental/control-flow/) for more details.
+    """
+
+    elements: typing.List[ElementalNode] = pydantic_v1.Field()
+    """
+    Sub elements to render.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+from .elemental_node import ElementalNode  # noqa: E402
+
+ElementalGroupNode.update_forward_refs()
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_response.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .job_details import JobDetails
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BulkGetJobResponse(pydantic.BaseModel):
+class BulkGetJobResponse(pydantic_v1.BaseModel):
     job: JobDetails
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_params.py` & `trycourier-6.0.1/src/courier/brands/types/brand_snippet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BulkGetJobUsersParams(pydantic.BaseModel):
-    job_id: str = pydantic.Field(alias="jobId")
-    cursor: typing.Optional[str]
+class BrandSnippet(pydantic_v1.BaseModel):
+    format: typing.Literal["handlebars"]
+    name: str
+    value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_get_job_users_response.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_users_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.paging import Paging
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .bulk_message_user_response import BulkMessageUserResponse
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BulkGetJobUsersResponse(pydantic.BaseModel):
+class BulkGetJobUsersResponse(pydantic_v1.BaseModel):
     items: typing.List[BulkMessageUserResponse]
     paging: Paging
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_error.py` & `trycourier-6.0.1/src/courier/commons/types/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BulkIngestError(pydantic.BaseModel):
-    user: typing.Any
-    error: typing.Any
+class Rule(pydantic_v1.BaseModel):
+    start: typing.Optional[str] = None
+    until: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_params.py` & `trycourier-6.0.1/src/courier/users/tokens/types/get_user_tokens_opts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .inbound_bulk_message_user import InboundBulkMessageUser
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BulkIngestUsersParams(pydantic.BaseModel):
-    users: typing.List[InboundBulkMessageUser]
+class GetUserTokensOpts(pydantic_v1.BaseModel):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_ingest_users_response.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_ingest_users_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .bulk_ingest_error import BulkIngestError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BulkIngestUsersResponse(pydantic.BaseModel):
+class BulkIngestUsersResponse(pydantic_v1.BaseModel):
     total: int
-    errors: typing.Optional[typing.List[BulkIngestError]]
+    errors: typing.Optional[typing.List[BulkIngestError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/bulk_message_user_response.py` & `trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_template_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .bulk_job_user_status import BulkJobUserStatus
-from .inbound_bulk_message_user import InboundBulkMessageUser
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...send.types.base_message import BaseMessage
 
 
-class BulkMessageUserResponse(InboundBulkMessageUser):
-    status: BulkJobUserStatus
-    message_id: typing.Optional[str] = pydantic.Field(alias="messageId")
+class InboundBulkTemplateMessage(BaseMessage):
+    template: str = pydantic_v1.Field()
+    """
+    The id of the notification template to be rendered and sent to the recipient(s).
+    This field or the content field must be supplied.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_content_message.py` & `trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_content_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from ...send.types.base_message import BaseMessage
 from ...send.types.content import Content
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class InboundBulkContentMessage(BaseMessage):
     """
     The message property has the following primary top-level properties. They define the destination and content of the message.
     Additional advanced configuration fields [are defined below](https://www.courier.com/docs/reference/send/message/#other-message-properties).
     """
 
-    content: Content = pydantic.Field(
-        description=(
-            "Describes the content of the message in a way that will work for email, push,\n"
-            "chat, or any channel. Either this or template must be specified.\n"
-        )
-    )
+    content: Content = pydantic_v1.Field()
+    """
+    Describes the content of the message in a way that will work for email, push,
+    chat, or any channel. Either this or template must be specified.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message.py` & `trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .inbound_bulk_message_v_1 import InboundBulkMessageV1
 from .inbound_bulk_message_v_2 import InboundBulkMessageV2
 
 
 class InboundBulkMessage(InboundBulkMessageV1):
-    message: typing.Optional[InboundBulkMessageV2]
+    message: typing.Optional[InboundBulkMessageV2] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_user.py` & `trycourier-6.0.1/src/courier/lists/types/put_subscriptions_recipient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.recipient_preferences import RecipientPreferences
-from ...send.types.user_recipient import UserRecipient
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InboundBulkMessageUser(pydantic.BaseModel):
-    preferences: typing.Optional[RecipientPreferences]
-    profile: typing.Optional[typing.Any]
-    recipient: typing.Optional[str]
-    data: typing.Optional[typing.Any]
-    to: typing.Optional[UserRecipient]
+class PutSubscriptionsRecipient(pydantic_v1.BaseModel):
+    recipient_id: str = pydantic_v1.Field(alias="recipientId")
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_message_v_1.py` & `trycourier-6.0.1/src/courier/tenants/types/list_users_for_tenant_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class InboundBulkMessageV1(pydantic.BaseModel):
-    brand: typing.Optional[str] = pydantic.Field(
-        description=(
-            "A unique identifier that represents the brand that should be used\n" "for rendering the notification.\n"
-        )
-    )
-    data: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description=(
-            "JSON that includes any data you want to pass to a message template.\n"
-            "The data will populate the corresponding template variables.\n"
-        )
-    )
-    event: typing.Optional[str]
-    locale: typing.Optional[typing.Dict[str, typing.Any]]
-    override: typing.Optional[typing.Any] = pydantic.Field(
-        description=(
-            "JSON that is merged into the request sent by Courier to the provider\n"
-            "to override properties or to gain access to features in the provider\n"
-            "API that are not natively supported by Courier.\n"
-        )
-    )
+from ...commons.types.user_tenant_association import UserTenantAssociation
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+
+
+class ListUsersForTenantResponse(pydantic_v1.BaseModel):
+    items: typing.Optional[typing.List[UserTenantAssociation]] = None
+    has_more: bool = pydantic_v1.Field()
+    """
+    Set to true when there are more pages that can be retrieved.
+    """
+
+    url: str = pydantic_v1.Field()
+    """
+    A url that may be used to generate these results.
+    """
+
+    next_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A url that may be used to generate fetch the next set of results.
+    Defined only when `has_more` is set to true
+    """
+
+    cursor: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A pointer to the next page of results. Defined
+    only when `has_more` is set to true
+    """
+
+    type: typing.Literal["list"] = pydantic_v1.Field()
+    """
+    Always set to `list`. Represents the type of this object.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/inbound_bulk_template_message.py` & `trycourier-6.0.1/src/courier/send/types/content_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...send.types.base_message import BaseMessage
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class InboundBulkTemplateMessage(BaseMessage):
-    template: str = pydantic.Field(
-        description=(
-            "The id of the notification template to be rendered and sent to the recipient(s).\n"
-            "This field or the content field must be supplied.\n"
-        )
-    )
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_message import BaseMessage
+from .base_message_send_to import BaseMessageSendTo
+from .content import Content
+
+
+class ContentMessage(BaseMessage, BaseMessageSendTo):
+    """
+    The message property has the following primary top-level properties. They define the destination and content of the message.
+    Additional advanced configuration fields [are defined below](https://www.courier.com/docs/reference/send/message/#other-message-properties).
+    """
+
+    content: Content = pydantic_v1.Field()
+    """
+    Describes the content of the message in a way that will work for email, push,
+    chat, or any channel. Either this or template must be specified.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/bulk/types/job_details.py` & `trycourier-6.0.1/src/courier/send/types/email_header.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .bulk_job_status import BulkJobStatus
-from .inbound_bulk_message import InboundBulkMessage
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class JobDetails(pydantic.BaseModel):
-    definition: InboundBulkMessage
-    enqueued: int
-    failures: int
-    received: int
-    status: BulkJobStatus
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .logo import Logo
+
+
+class EmailHeader(pydantic_v1.BaseModel):
+    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
+    bar_color: typing.Optional[str] = pydantic_v1.Field(alias="barColor", default=None)
+    logo: Logo
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/__init__.py` & `trycourier-6.0.1/src/courier/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/errors/__init__.py` & `trycourier-6.0.1/src/courier/commons/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/__init__.py` & `trycourier-6.0.1/src/courier/commons/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/already_exists.py` & `trycourier-6.0.1/src/courier/profiles/types/subscribe_to_lists_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .subscribe_to_lists_request_list_object import SubscribeToListsRequestListObject
 
-from ....core.datetime_utils import serialize_datetime
-from .base_error import BaseError
 
-
-class AlreadyExists(BaseError):
-    type: typing_extensions.Literal["invalid_request_error"]
+class SubscribeToListsRequest(pydantic_v1.BaseModel):
+    lists: typing.List[SubscribeToListsRequestListObject]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/bad_request.py` & `trycourier-6.0.1/src/courier/commons/types/not_found.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
-
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .base_error import BaseError
 
 
-class BadRequest(BaseError):
-    type: typing_extensions.Literal["invalid_request_error"]
+class NotFound(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/base_error.py` & `trycourier-6.0.1/src/courier/send/types/widget_background.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BaseError(pydantic.BaseModel):
-    message: str = pydantic.Field(description="A message describing the error that occurred.")
+class WidgetBackground(pydantic_v1.BaseModel):
+    top_color: typing.Optional[str] = pydantic_v1.Field(alias="topColor", default=None)
+    bottom_color: typing.Optional[str] = pydantic_v1.Field(alias="bottomColor", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/channel_preference.py` & `trycourier-6.0.1/src/courier/notifications/types/submission_checks_replace_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .channel_classification import ChannelClassification
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .check import Check
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ChannelPreference(pydantic.BaseModel):
-    channel: ChannelClassification
+class SubmissionChecksReplaceResponse(pydantic_v1.BaseModel):
+    checks: typing.List[Check]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/conflict.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_ingest_users_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .inbound_bulk_message_user import InboundBulkMessageUser
 
-from ....core.datetime_utils import serialize_datetime
-from .base_error import BaseError
 
-
-class Conflict(BaseError):
-    type: typing_extensions.Literal["invalid_request_error"]
+class BulkIngestUsersParams(pydantic_v1.BaseModel):
+    users: typing.List[InboundBulkMessageUser]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/email.py` & `trycourier-6.0.1/src/courier/send/types/invalid_user_recipient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Email(pydantic.BaseModel):
-    footer: typing.Any
-    header: typing.Any
+class InvalidUserRecipient(pydantic_v1.BaseModel):
+    list_id: str
+    list_pattern: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/message_not_found.py` & `trycourier-6.0.1/src/courier/send/types/elemental_content_sugar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
-from .base_error import BaseError
 
-
-class MessageNotFound(BaseError):
-    type: typing_extensions.Literal["invalid_request_error"]
+class ElementalContentSugar(pydantic_v1.BaseModel):
+    """
+    Syntatic Sugar to provide a fast shorthand for Courier Elemental Blocks.
+    """
+
+    title: str = pydantic_v1.Field()
+    """
+    The title to be displayed by supported channels i.e. push, email (as subject)
+    """
+
+    body: str = pydantic_v1.Field()
+    """
+    The text content displayed in the notification.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/not_found.py` & `trycourier-6.0.1/src/courier/brands/types/brands_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...commons.types.paging import Paging
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .brand import Brand
 
-from ....core.datetime_utils import serialize_datetime
-from .base_error import BaseError
 
-
-class NotFound(BaseError):
-    type: typing_extensions.Literal["invalid_request_error"]
+class BrandsResponse(pydantic_v1.BaseModel):
+    paging: Paging
+    results: typing.List[Brand]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/notification_preference_details.py` & `trycourier-6.0.1/src/courier/commons/types/notification_preference_details.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .channel_preference import ChannelPreference
 from .preference_status import PreferenceStatus
 from .rule import Rule
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NotificationPreferenceDetails(pydantic.BaseModel):
+class NotificationPreferenceDetails(pydantic_v1.BaseModel):
     status: PreferenceStatus
-    rules: typing.Optional[typing.List[Rule]]
-    channel_preferences: typing.Optional[typing.List[ChannelPreference]]
+    rules: typing.Optional[typing.List[Rule]] = None
+    channel_preferences: typing.Optional[typing.List[ChannelPreference]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/paging.py` & `trycourier-6.0.1/src/courier/commons/types/paging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Paging(pydantic.BaseModel):
-    cursor: typing.Optional[str]
+class Paging(pydantic_v1.BaseModel):
+    cursor: typing.Optional[str] = None
     more: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/payment_required.py` & `trycourier-6.0.1/src/courier/users/preferences/types/user_preferences_get_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
-
 from ....core.datetime_utils import serialize_datetime
-from .base_error import BaseError
+from ....core.pydantic_utilities import pydantic_v1
+from .topic_preference import TopicPreference
 
 
-class PaymentRequired(BaseError):
-    type: typing_extensions.Literal["authorization_error"]
+class UserPreferencesGetResponse(pydantic_v1.BaseModel):
+    topic: TopicPreference
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/recipient_preferences.py` & `trycourier-6.0.1/src/courier/send/types/utm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .notification_preferences import NotificationPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RecipientPreferences(pydantic.BaseModel):
-    categories: typing.Optional[NotificationPreferences]
-    notifications: typing.Optional[NotificationPreferences]
+class Utm(pydantic_v1.BaseModel):
+    source: typing.Optional[str] = None
+    medium: typing.Optional[str] = None
+    campaign: typing.Optional[str] = None
+    term: typing.Optional[str] = None
+    content: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/rule.py` & `trycourier-6.0.1/src/courier/send/types/locale.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Rule(pydantic.BaseModel):
-    start: typing.Optional[str]
-    until: str
+class Locale(pydantic_v1.BaseModel):
+    content: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/commons/types/user_tenant_association.py` & `trycourier-6.0.1/src/courier/send/types/elemental_base_node.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class UserTenantAssociation(pydantic.BaseModel):
-    user_id: str = pydantic.Field(description="User ID for the assocation between tenant and user")
-    type: typing_extensions.Literal["user"]
-    tenant_id: str = pydantic.Field(description="Tenant ID for the assocation between tenant and user")
-    profile: typing.Dict[str, typing.Any]
+class ElementalBaseNode(pydantic_v1.BaseModel):
+    channels: typing.Optional[typing.List[str]] = None
+    ref: typing.Optional[str] = None
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    loop: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/client.py` & `trycourier-6.0.1/src/courier/audiences/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,586 +1,644 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
-from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ...core.jsonable_encoder import jsonable_encoder
-from ...core.remove_none_from_dict import remove_none_from_dict
 from ..commons.errors.bad_request_error import BadRequestError
-from ..commons.errors.not_found_error import NotFoundError
 from ..commons.types.bad_request import BadRequest
-from ..commons.types.not_found import NotFound
-from ..commons.types.recipient_preferences import RecipientPreferences
-from .types.list import List
-from .types.list_get_all_response import ListGetAllResponse
-from .types.list_get_subscriptions_response import ListGetSubscriptionsResponse
-from .types.list_put_params import ListPutParams
-from .types.put_subscriptions_recipient import PutSubscriptionsRecipient
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ..core.api_error import ApiError
+from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.remove_none_from_dict import remove_none_from_dict
+from ..core.request_options import RequestOptions
+from .types.audience import Audience
+from .types.audience_list_response import AudienceListResponse
+from .types.audience_member_list_response import AudienceMemberListResponse
+from .types.audience_update_response import AudienceUpdateResponse
+from .types.filter import Filter
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class ListsClient:
+class AudiencesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def list(self, *, cursor: typing.Optional[str] = None, pattern: typing.Optional[str] = None) -> ListGetAllResponse:
+    def get(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Audience:
         """
-        Returns all of the lists, with the ability to filter based on a pattern.
+        Returns the specified audience by id.
 
         Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next page of lists.
+            - audience_id: str. A unique identifier representing the audience_id
 
-            - pattern: typing.Optional[str]. "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
+
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.audiences.get(
+            audience_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
-            params=remove_none_from_dict({"cursor": cursor, "pattern": pattern}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListGetAllResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(Audience, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, list_id: str, *, cursor: typing.Optional[str] = None, pattern: typing.Optional[str] = None) -> List:
+    def update(
+        self,
+        audience_id: str,
+        *,
+        name: typing.Optional[str] = OMIT,
+        description: typing.Optional[str] = OMIT,
+        filter: typing.Optional[Filter] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> AudienceUpdateResponse:
         """
-        Returns a list based on the list ID provided.
+        Creates or updates audience.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - audience_id: str. A unique identifier representing the audience id
 
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next page of lists.
+            - name: typing.Optional[str]. The name of the audience
 
-            - pattern: typing.Optional[str]. "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}"),
-            params=remove_none_from_dict({"cursor": cursor, "pattern": pattern}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(List, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            - description: typing.Optional[str]. A description of the audience
 
-    def update(self, list_id: str, *, request: ListPutParams) -> List:
-        """
-        Create or replace an existing list with the supplied values.
+            - filter: typing.Optional[Filter].
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier import SingleFilterConfig
+        from courier.client import Courier
 
-            - request: ListPutParams.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}"),
-            json=jsonable_encoder(request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(List, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def delete(self, list_id: str) -> None:
-        """
-        Delete a list by list ID.
-
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client.audiences.update(
+            audience_id="string",
+            name="string",
+            description="string",
+            filter=SingleFilterConfig(
+                value="string",
+                path="string",
+                operator="ENDS_WITH",
+            ),
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def restore(self, list_id: str) -> None:
-        """
-        Restore a previously deleted list.
-
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if name is not OMIT:
+            _request["name"] = name
+        if description is not OMIT:
+            _request["description"] = description
+        if filter is not OMIT:
+            _request["filter"] = filter
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/restore"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(AudienceUpdateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_subscribers(self, list_id: str, *, cursor: typing.Optional[str] = None) -> ListGetSubscriptionsResponse:
+    def delete(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Get the list's subscriptions.
+        Deletes the specified audience.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of list subscriptions
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions"),
-            params=remove_none_from_dict({"cursor": cursor}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListGetSubscriptionsResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def update_subscribers(self, list_id: str, *, request: typing.List[PutSubscriptionsRecipient]) -> None:
-        """
-        Subscribes the users to the list, overwriting existing subscriptions. If the list does not exist, it will be automatically created.
+            - audience_id: str. A unique identifier representing the audience id
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
 
-            - request: typing.List[PutSubscriptionsRecipient].
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.audiences.delete(
+            audience_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions"),
-            json=jsonable_encoder(request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def add_subscribers(
+    def list_members(
         self,
-        list_id: str,
+        audience_id: str,
         *,
-        request: typing.List[PutSubscriptionsRecipient],
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[int] = None,
-    ) -> None:
+        cursor: typing.Optional[str] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> AudienceMemberListResponse:
         """
-        Subscribes additional users to the list, without modifying existing subscriptions. If the list does not exist, it will be automatically created.
+        Get list of members of an audience.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - audience_id: str. A unique identifier representing the audience id
 
-            - request: typing.List[PutSubscriptionsRecipient].
+            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of members
 
-            - idempotency_key: typing.Optional[str].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
 
-            - idempotency_expiry: typing.Optional[int].
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.audiences.list_members(
+            audience_id="string",
+            cursor="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_dict(
-                {
-                    **self._client_wrapper.get_headers(),
-                    "Idempotency-Key": idempotency_key,
-                    "X-Idempotency-Expiration": idempotency_expiry,
-                }
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}/members"
             ),
-            timeout=60,
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(AudienceMemberListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def subscribe(
-        self, list_id: str, user_id: str, *, preferences: typing.Optional[RecipientPreferences] = OMIT
-    ) -> None:
+    def list_audiences(
+        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> AudienceListResponse:
         """
-        Subscribe a user to an existing list (note: if the List does not exist, it will be automatically created).
+        Get the audiences associated with the authorization token.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audiences
 
-            - user_id: str. A unique identifier representing the recipient associated with the list
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
 
-            - preferences: typing.Optional[RecipientPreferences].
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if preferences is not OMIT:
-            _request["preferences"] = preferences
-        _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions/{user_id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.audiences.list_audiences(
+            cursor="string",
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def unsubscribe(self, list_id: str, user_id: str) -> None:
-        """
-        Delete a subscription to a list by list ID and user ID.
-
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - user_id: str. A unique identifier representing the recipient associated with the list
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions/{user_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(AudienceListResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncListsClient:
+class AsyncAudiencesClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def list(
-        self, *, cursor: typing.Optional[str] = None, pattern: typing.Optional[str] = None
-    ) -> ListGetAllResponse:
+    async def get(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Audience:
         """
-        Returns all of the lists, with the ability to filter based on a pattern.
+        Returns the specified audience by id.
 
         Parameters:
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next page of lists.
+            - audience_id: str. A unique identifier representing the audience_id
 
-            - pattern: typing.Optional[str]. "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
+
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.audiences.get(
+            audience_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "lists"),
-            params=remove_none_from_dict({"cursor": cursor, "pattern": pattern}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListGetAllResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(Audience, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(
-        self, list_id: str, *, cursor: typing.Optional[str] = None, pattern: typing.Optional[str] = None
-    ) -> List:
+    async def update(
+        self,
+        audience_id: str,
+        *,
+        name: typing.Optional[str] = OMIT,
+        description: typing.Optional[str] = OMIT,
+        filter: typing.Optional[Filter] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> AudienceUpdateResponse:
         """
-        Returns a list based on the list ID provided.
+        Creates or updates audience.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - audience_id: str. A unique identifier representing the audience id
 
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next page of lists.
+            - name: typing.Optional[str]. The name of the audience
 
-            - pattern: typing.Optional[str]. "A pattern used to filter the list items returned. Pattern types supported: exact match on `list_id` or a pattern of one or more pattern parts. you may replace a part with either: `*` to match all parts in that position, or `**` to signify a wildcard `endsWith` pattern match."
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}"),
-            params=remove_none_from_dict({"cursor": cursor, "pattern": pattern}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(List, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            - description: typing.Optional[str]. A description of the audience
 
-    async def update(self, list_id: str, *, request: ListPutParams) -> List:
-        """
-        Create or replace an existing list with the supplied values.
+            - filter: typing.Optional[Filter].
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier import SingleFilterConfig
+        from courier.client import AsyncCourier
 
-            - request: ListPutParams.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}"),
-            json=jsonable_encoder(request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(List, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def delete(self, list_id: str) -> None:
-        """
-        Delete a list by list ID.
-
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        await client.audiences.update(
+            audience_id="string",
+            name="string",
+            description="string",
+            filter=SingleFilterConfig(
+                value="string",
+                path="string",
+                operator="ENDS_WITH",
+            ),
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def restore(self, list_id: str) -> None:
-        """
-        Restore a previously deleted list.
-
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if name is not OMIT:
+            _request["name"] = name
+        if description is not OMIT:
+            _request["description"] = description
+        if filter is not OMIT:
+            _request["filter"] = filter
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/restore"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(AudienceUpdateResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_subscribers(
-        self, list_id: str, *, cursor: typing.Optional[str] = None
-    ) -> ListGetSubscriptionsResponse:
+    async def delete(self, audience_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
-        Get the list's subscriptions.
+        Deletes the specified audience.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of list subscriptions
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions"),
-            params=remove_none_from_dict({"cursor": cursor}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListGetSubscriptionsResponse, _response.json())  # type: ignore
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def update_subscribers(self, list_id: str, *, request: typing.List[PutSubscriptionsRecipient]) -> None:
-        """
-        Subscribes the users to the list, overwriting existing subscriptions. If the list does not exist, it will be automatically created.
+            - audience_id: str. A unique identifier representing the audience id
 
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
 
-            - request: typing.List[PutSubscriptionsRecipient].
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.audiences.delete(
+            audience_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions"),
-            json=jsonable_encoder(request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
             return
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def add_subscribers(
+    async def list_members(
         self,
-        list_id: str,
+        audience_id: str,
         *,
-        request: typing.List[PutSubscriptionsRecipient],
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[int] = None,
-    ) -> None:
+        cursor: typing.Optional[str] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> AudienceMemberListResponse:
         """
-        Subscribes additional users to the list, without modifying existing subscriptions. If the list does not exist, it will be automatically created.
+        Get list of members of an audience.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - audience_id: str. A unique identifier representing the audience id
 
-            - request: typing.List[PutSubscriptionsRecipient].
+            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of members
 
-            - idempotency_key: typing.Optional[str].
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
 
-            - idempotency_expiry: typing.Optional[int].
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.audiences.list_members(
+            audience_id="string",
+            cursor="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions"),
-            json=jsonable_encoder(request),
-            headers=remove_none_from_dict(
-                {
-                    **self._client_wrapper.get_headers(),
-                    "Idempotency-Key": idempotency_key,
-                    "X-Idempotency-Expiration": idempotency_expiry,
-                }
+            "GET",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audiences/{jsonable_encoder(audience_id)}/members"
             ),
-            timeout=60,
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(AudienceMemberListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def subscribe(
-        self, list_id: str, user_id: str, *, preferences: typing.Optional[RecipientPreferences] = OMIT
-    ) -> None:
+    async def list_audiences(
+        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> AudienceListResponse:
         """
-        Subscribe a user to an existing list (note: if the List does not exist, it will be automatically created).
+        Get the audiences associated with the authorization token.
 
         Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
+            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audiences
 
-            - user_id: str. A unique identifier representing the recipient associated with the list
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
 
-            - preferences: typing.Optional[RecipientPreferences].
-        """
-        _request: typing.Dict[str, typing.Any] = {}
-        if preferences is not OMIT:
-            _request["preferences"] = preferences
-        _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions/{user_id}"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.audiences.list_audiences(
+            cursor="string",
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def unsubscribe(self, list_id: str, user_id: str) -> None:
-        """
-        Delete a subscription to a list by list ID and user ID.
-
-        Parameters:
-            - list_id: str. A unique identifier representing the list you wish to retrieve.
-
-            - user_id: str. A unique identifier representing the recipient associated with the list
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"lists/{list_id}/subscriptions/{user_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audiences"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
-        if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFound, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(AudienceListResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/__init__.py` & `trycourier-6.0.1/src/courier/lists/types/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .list import List
-from .list_find_by_recipient_id_params import ListFindByRecipientIdParams
-from .list_find_by_recipient_id_response import ListFindByRecipientIdResponse
-from .list_get_all_params import ListGetAllParams
 from .list_get_all_response import ListGetAllResponse
-from .list_get_subscriptions_params import ListGetSubscriptionsParams
 from .list_get_subscriptions_response import ListGetSubscriptionsResponse
 from .list_put_params import ListPutParams
 from .list_subscription_recipient import ListSubscriptionRecipient
 from .put_subscriptions_recipient import PutSubscriptionsRecipient
-from .recipient_subscriptions_response import RecipientSubscriptionsResponse
 
 __all__ = [
     "List",
-    "ListFindByRecipientIdParams",
-    "ListFindByRecipientIdResponse",
-    "ListGetAllParams",
     "ListGetAllResponse",
-    "ListGetSubscriptionsParams",
     "ListGetSubscriptionsResponse",
     "ListPutParams",
     "ListSubscriptionRecipient",
     "PutSubscriptionsRecipient",
-    "RecipientSubscriptionsResponse",
 ]
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list.py` & `trycourier-6.0.1/src/courier/messages/types/list_messages_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class List(pydantic.BaseModel):
-    id: str
-    name: str
-    created: typing.Optional[int]
-    updated: typing.Optional[int]
+from ...commons.types.paging import Paging
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .message_details import MessageDetails
+
+
+class ListMessagesResponse(pydantic_v1.BaseModel):
+    paging: Paging = pydantic_v1.Field()
+    """
+    Paging information for the result set.
+    """
+
+    results: typing.List[MessageDetails] = pydantic_v1.Field()
+    """
+    An array of messages with their details.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_params.py` & `trycourier-6.0.1/src/courier/audiences/types/audience_member_list_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...commons.types.paging import Paging
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .audience_member import AudienceMember
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListFindByRecipientIdParams(pydantic.BaseModel):
-    cursor: typing.Optional[str]
+class AudienceMemberListResponse(pydantic_v1.BaseModel):
+    items: typing.List[AudienceMember]
+    paging: Paging
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_find_by_recipient_id_response.py` & `trycourier-6.0.1/src/courier/lists/types/list_get_all_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.paging import Paging
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .list import List
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListFindByRecipientIdResponse(pydantic.BaseModel):
+class ListGetAllResponse(pydantic_v1.BaseModel):
     paging: Paging
-    results: typing.List[List]
+    items: typing.List[List]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_params.py` & `trycourier-6.0.1/src/courier/automations/types/automation_run_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .profile import Profile
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListGetAllParams(pydantic.BaseModel):
-    cursor: typing.Optional[str]
-    pattern: typing.Optional[str]
+class AutomationRunContext(pydantic_v1.BaseModel):
+    brand: typing.Optional[str] = None
+    data: typing.Optional[typing.Any] = None
+    profile: typing.Optional[Profile] = None
+    template: typing.Optional[str] = None
+    recipient: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_all_response.py` & `trycourier-6.0.1/src/courier/notifications/types/submission_checks_get_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .list import List
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .check import Check
 
 
-class ListGetAllResponse(pydantic.BaseModel):
-    paging: Paging
-    items: typing.List[List]
+class SubmissionChecksGetResponse(pydantic_v1.BaseModel):
+    checks: typing.List[Check]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_params.py` & `trycourier-6.0.1/src/courier/send/types/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .utm import Utm
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListGetSubscriptionsParams(pydantic.BaseModel):
-    cursor: typing.Optional[str]
+class Metadata(pydantic_v1.BaseModel):
+    utm: typing.Optional[Utm] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_get_subscriptions_response.py` & `trycourier-6.0.1/src/courier/audit_events/types/list_audit_events_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.paging import Paging
-from .list_subscription_recipient import ListSubscriptionRecipient
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .audit_event import AuditEvent
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListGetSubscriptionsResponse(pydantic.BaseModel):
+class ListAuditEventsResponse(pydantic_v1.BaseModel):
     paging: Paging
-    items: typing.List[ListSubscriptionRecipient]
+    results: typing.List[AuditEvent]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_put_params.py` & `trycourier-6.0.1/src/courier/lists/types/list_subscription_recipient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListPutParams(pydantic.BaseModel):
-    name: str
-    preferences: typing.Optional[RecipientPreferences]
+class ListSubscriptionRecipient(pydantic_v1.BaseModel):
+    recipient_id: str = pydantic_v1.Field(alias="recipientId")
+    created: typing.Optional[str] = None
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/list_subscription_recipient.py` & `trycourier-6.0.1/src/courier/automations/types/automation_update_profile_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .merge_algorithm import MergeAlgorithm
+from .profile import Profile
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListSubscriptionRecipient(pydantic.BaseModel):
-    recipient_id: str = pydantic.Field(alias="recipientId")
-    created: typing.Optional[str]
-    preferences: typing.Optional[RecipientPreferences]
+class AutomationUpdateProfileStep(pydantic_v1.BaseModel):
+    action: typing.Literal["update-profile"]
+    recipient_id: str
+    profile: Profile
+    merge: MergeAlgorithm
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/put_subscriptions_recipient.py` & `trycourier-6.0.1/src/courier/lists/types/list_put_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PutSubscriptionsRecipient(pydantic.BaseModel):
-    recipient_id: str = pydantic.Field(alias="recipientId")
-    preferences: typing.Optional[RecipientPreferences]
+class ListPutParams(pydantic_v1.BaseModel):
+    name: str
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/lists/types/recipient_subscriptions_response.py` & `trycourier-6.0.1/src/courier/brands/types/brand_get_all_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.paging import Paging
-from .list import List
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .brand import Brand
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RecipientSubscriptionsResponse(pydantic.BaseModel):
+class BrandGetAllResponse(pydantic_v1.BaseModel):
     paging: Paging
-    results: typing.List[List]
+    results: typing.List[Brand]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/__init__.py` & `trycourier-6.0.1/src/courier/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/client.py` & `trycourier-6.0.1/src/courier/users/preferences/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,436 +1,399 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
+from ...commons.errors.bad_request_error import BadRequestError
+from ...commons.errors.not_found_error import NotFoundError
+from ...commons.types.bad_request import BadRequest
+from ...commons.types.not_found import NotFound
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ...core.jsonable_encoder import jsonable_encoder
+from ...core.pydantic_utilities import pydantic_v1
 from ...core.remove_none_from_dict import remove_none_from_dict
-from ..commons.errors.bad_request_error import BadRequestError
-from ..commons.errors.message_not_found_error import MessageNotFoundError
-from ..commons.types.bad_request import BadRequest
-from ..commons.types.message_not_found import MessageNotFound
-from .types.list_messages_response import ListMessagesResponse
-from .types.message_details import MessageDetails
-from .types.message_history_response import MessageHistoryResponse
-from .types.render_output_response import RenderOutputResponse
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.request_options import RequestOptions
+from .types.topic_preference_update import TopicPreferenceUpdate
+from .types.user_preferences_get_response import UserPreferencesGetResponse
+from .types.user_preferences_list_response import UserPreferencesListResponse
+from .types.user_preferences_update_response import UserPreferencesUpdateResponse
 
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
-class MessagesClient:
+
+class PreferencesClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(
-        self,
-        *,
-        archived: typing.Optional[bool] = None,
-        cursor: typing.Optional[str] = None,
-        event: typing.Optional[str] = None,
-        list: typing.Optional[str] = None,
-        message_id: typing.Optional[str] = None,
-        notification: typing.Optional[str] = None,
-        recipient: typing.Optional[str] = None,
-        status: typing.Optional[str] = None,
-        tags: typing.Optional[str] = None,
-        enqueued_after: typing.Optional[str] = None,
-        trace_id: typing.Optional[str] = None,
-    ) -> ListMessagesResponse:
+        self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserPreferencesListResponse:
         """
-        Fetch the statuses of messages you've previously sent.
+        Fetch all user preferences.
 
         Parameters:
-            - archived: typing.Optional[bool]. A boolean value that indicates whether archived messages should be included in the response.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of message statuses.
-
-            - event: typing.Optional[str]. A unique identifier representing the event that was used to send the event.
-
-            - list: typing.Optional[str]. A unique identifier representing the list the message was sent to.
-
-            - message_id: typing.Optional[str]. A unique identifier representing the message_id returned from either /send or /send/list.
-
-            - notification: typing.Optional[str]. A unique identifier representing the notification that was used to send the event.
-
-            - recipient: typing.Optional[str]. A unique identifier representing the recipient associated with the requested profile.
+            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
 
-            - status: typing.Optional[str]. An indicator of the current status of the message. Multiple status values can be passed in.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
 
-            - tags: typing.Optional[str]. A comma delimited list of 'tags'. Messages will be returned if they match any of the tags passed in.
-
-            - enqueued_after: typing.Optional[str]. The enqueued datetime of a message to filter out messages received before.
-
-            - trace_id: typing.Optional[str]. The unique identifier used to trace the requests
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.users.preferences.list(
+            user_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
-            params=remove_none_from_dict(
-                {
-                    "archived": archived,
-                    "cursor": cursor,
-                    "event": event,
-                    "list": list,
-                    "messageId": message_id,
-                    "notification": notification,
-                    "recipient": recipient,
-                    "status": status,
-                    "tags": tags,
-                    "enqueued_after": enqueued_after,
-                    "traceId": trace_id,
-                }
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/preferences"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListMessagesResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(UserPreferencesListResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, message_id: str) -> MessageDetails:
+    def get(
+        self, user_id: str, topic_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserPreferencesGetResponse:
         """
-        Fetch the status of a message you've previously sent.
+        Fetch user preferences for a specific subscription topic.
 
         Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
+            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+
+            - topic_id: str. A unique identifier associated with a subscription topic.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
+
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.users.preferences.get(
+            user_id="string",
+            topic_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageDetails, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(UserPreferencesGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def cancel(
+    def update(
         self,
-        message_id: str,
+        user_id: str,
+        topic_id: str,
         *,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[int] = None,
-    ) -> MessageDetails:
+        topic: TopicPreferenceUpdate,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserPreferencesUpdateResponse:
         """
-        Cancel a message that is currently in the process of being delivered. A well-formatted API call to the cancel message API will return either `200` status code for a successful cancellation or `409` status code for an unsuccessful cancellation. Both cases will include the actual message record in the response body (see details below).
+        Update or Create user preferences for a specific subscription topic.
 
         Parameters:
-            - message_id: str. A unique identifier representing the message ID
+            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
 
-            - idempotency_key: typing.Optional[str].
+            - topic_id: str. A unique identifier associated with a subscription topic.
 
-            - idempotency_expiry: typing.Optional[int].
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}/cancel"),
-            headers=remove_none_from_dict(
-                {
-                    **self._client_wrapper.get_headers(),
-                    "Idempotency-Key": idempotency_key,
-                    "X-Idempotency-Expiration": idempotency_expiry,
-                }
-            ),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageDetails, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            - topic: TopicPreferenceUpdate.
 
-    def get_history(self, message_id: str, *, type: typing.Optional[str] = None) -> MessageHistoryResponse:
-        """
-        Fetch the array of events of a message you've previously sent.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
+        from courier.users import TopicPreferenceUpdate
 
-        Parameters:
-            - message_id: str. A unique identifier representing the message ID
-
-            - type: typing.Optional[str]. A supported Message History type that will filter the events returned.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}/history"),
-            params=remove_none_from_dict({"type": type}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageHistoryResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def get_content(self, message_id: str) -> RenderOutputResponse:
-        """
-        Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}/output"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client.users.preferences.update(
+            user_id="abc-123",
+            topic_id="74Q4QGFBEX481DP6JRPMV751H4XT",
+            topic=TopicPreferenceUpdate(
+                status="OPTED_IN",
+                has_custom_routing=True,
+                custom_routing=["inbox", "email"],
+            ),
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RenderOutputResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def archive(self, request_id: str) -> None:
-        """
-        Parameters:
-            - request_id: str. A unique identifier representing the request ID
         """
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"requests/{request_id}/archive"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder({"topic": topic})
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder({"topic": topic}),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(UserPreferencesUpdateResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncMessagesClient:
+class AsyncPreferencesClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(
-        self,
-        *,
-        archived: typing.Optional[bool] = None,
-        cursor: typing.Optional[str] = None,
-        event: typing.Optional[str] = None,
-        list: typing.Optional[str] = None,
-        message_id: typing.Optional[str] = None,
-        notification: typing.Optional[str] = None,
-        recipient: typing.Optional[str] = None,
-        status: typing.Optional[str] = None,
-        tags: typing.Optional[str] = None,
-        enqueued_after: typing.Optional[str] = None,
-        trace_id: typing.Optional[str] = None,
-    ) -> ListMessagesResponse:
+        self, user_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserPreferencesListResponse:
         """
-        Fetch the statuses of messages you've previously sent.
+        Fetch all user preferences.
 
         Parameters:
-            - archived: typing.Optional[bool]. A boolean value that indicates whether archived messages should be included in the response.
-
-            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of message statuses.
-
-            - event: typing.Optional[str]. A unique identifier representing the event that was used to send the event.
-
-            - list: typing.Optional[str]. A unique identifier representing the list the message was sent to.
-
-            - message_id: typing.Optional[str]. A unique identifier representing the message_id returned from either /send or /send/list.
-
-            - notification: typing.Optional[str]. A unique identifier representing the notification that was used to send the event.
-
-            - recipient: typing.Optional[str]. A unique identifier representing the recipient associated with the requested profile.
-
-            - status: typing.Optional[str]. An indicator of the current status of the message. Multiple status values can be passed in.
+            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
 
-            - tags: typing.Optional[str]. A comma delimited list of 'tags'. Messages will be returned if they match any of the tags passed in.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
 
-            - enqueued_after: typing.Optional[str]. The enqueued datetime of a message to filter out messages received before.
-
-            - trace_id: typing.Optional[str]. The unique identifier used to trace the requests
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.users.preferences.list(
+            user_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "messages"),
-            params=remove_none_from_dict(
-                {
-                    "archived": archived,
-                    "cursor": cursor,
-                    "event": event,
-                    "list": list,
-                    "messageId": message_id,
-                    "notification": notification,
-                    "recipient": recipient,
-                    "status": status,
-                    "tags": tags,
-                    "enqueued_after": enqueued_after,
-                    "traceId": trace_id,
-                }
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{jsonable_encoder(user_id)}/preferences"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListMessagesResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(UserPreferencesListResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, message_id: str) -> MessageDetails:
+    async def get(
+        self, user_id: str, topic_id: str, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> UserPreferencesGetResponse:
         """
-        Fetch the status of a message you've previously sent.
+        Fetch user preferences for a specific subscription topic.
 
         Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
+            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
+
+            - topic_id: str. A unique identifier associated with a subscription topic.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
+
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.users.preferences.get(
+            user_id="string",
+            topic_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageDetails, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
+            return pydantic_v1.parse_obj_as(UserPreferencesGetResponse, _response.json())  # type: ignore
         if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
+            raise NotFoundError(pydantic_v1.parse_obj_as(NotFound, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def cancel(
+    async def update(
         self,
-        message_id: str,
+        user_id: str,
+        topic_id: str,
         *,
-        idempotency_key: typing.Optional[str] = None,
-        idempotency_expiry: typing.Optional[int] = None,
-    ) -> MessageDetails:
+        topic: TopicPreferenceUpdate,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> UserPreferencesUpdateResponse:
         """
-        Cancel a message that is currently in the process of being delivered. A well-formatted API call to the cancel message API will return either `200` status code for a successful cancellation or `409` status code for an unsuccessful cancellation. Both cases will include the actual message record in the response body (see details below).
+        Update or Create user preferences for a specific subscription topic.
 
         Parameters:
-            - message_id: str. A unique identifier representing the message ID
-
-            - idempotency_key: typing.Optional[str].
+            - user_id: str. A unique identifier associated with the user whose preferences you wish to retrieve.
 
-            - idempotency_expiry: typing.Optional[int].
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}/cancel"),
-            headers=remove_none_from_dict(
-                {
-                    **self._client_wrapper.get_headers(),
-                    "Idempotency-Key": idempotency_key,
-                    "X-Idempotency-Expiration": idempotency_expiry,
-                }
-            ),
-            timeout=60,
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageDetails, _response.json())  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            - topic_id: str. A unique identifier associated with a subscription topic.
 
-    async def get_history(self, message_id: str, *, type: typing.Optional[str] = None) -> MessageHistoryResponse:
-        """
-        Fetch the array of events of a message you've previously sent.
+            - topic: TopicPreferenceUpdate.
 
-        Parameters:
-            - message_id: str. A unique identifier representing the message ID
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
+        from courier.users import TopicPreferenceUpdate
 
-            - type: typing.Optional[str]. A supported Message History type that will filter the events returned.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}/history"),
-            params=remove_none_from_dict({"type": type}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(MessageHistoryResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def get_content(self, message_id: str) -> RenderOutputResponse:
-        """
-        Parameters:
-            - message_id: str. A unique identifier associated with the message you wish to retrieve (results from a send).
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"messages/{message_id}/output"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        await client.users.preferences.update(
+            user_id="abc-123",
+            topic_id="74Q4QGFBEX481DP6JRPMV751H4XT",
+            topic=TopicPreferenceUpdate(
+                status="OPTED_IN",
+                has_custom_routing=True,
+                custom_routing=["inbox", "email"],
+            ),
         )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RenderOutputResponse, _response.json())  # type: ignore
-        if _response.status_code == 400:
-            raise BadRequestError(pydantic.parse_obj_as(BadRequest, _response.json()))  # type: ignore
-        if _response.status_code == 404:
-            raise MessageNotFoundError(pydantic.parse_obj_as(MessageNotFound, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def archive(self, request_id: str) -> None:
-        """
-        Parameters:
-            - request_id: str. A unique identifier representing the request ID
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"requests/{request_id}/archive"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"users/{jsonable_encoder(user_id)}/preferences/{jsonable_encoder(topic_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder({"topic": topic})
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder({"topic": topic}),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(UserPreferencesUpdateResponse, _response.json())  # type: ignore
+        if _response.status_code == 400:
+            raise BadRequestError(pydantic_v1.parse_obj_as(BadRequest, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/__init__.py` & `trycourier-6.0.1/src/courier/messages/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/list_messages_response.py` & `trycourier-6.0.1/src/courier/profiles/types/get_list_subscriptions_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.paging import Paging
-from .message_details import MessageDetails
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .get_list_subscriptions_list import GetListSubscriptionsList
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListMessagesResponse(pydantic.BaseModel):
-    paging: Paging = pydantic.Field(description="Paging information for the result set.")
-    results: typing.List[MessageDetails] = pydantic.Field(description="An array of messages with their details.")
+class GetListSubscriptionsResponse(pydantic_v1.BaseModel):
+    paging: Paging
+    results: typing.List[GetListSubscriptionsList] = pydantic_v1.Field()
+    """
+    An array of lists
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/message_details.py` & `trycourier-6.0.1/src/courier/messages/types/message_details.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,85 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .message_status import MessageStatus
 from .reason import Reason
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class MessageDetails(pydantic.BaseModel):
-    id: str = pydantic.Field(
-        description="A unique identifier associated with the message you wish to retrieve (results from a send)."
-    )
-    status: MessageStatus = pydantic.Field(description="The current status of the message.")
-    enqueued: int = pydantic.Field(
-        description="A UTC timestamp at which Courier received the message request. Stored as a millisecond representation of the Unix epoch."
-    )
-    sent: int = pydantic.Field(
-        description="A UTC timestamp at which Courier passed the message to the Integration provider. Stored as a millisecond representation of the Unix epoch."
-    )
-    delivered: int = pydantic.Field(
-        description="A UTC timestamp at which the Integration provider delivered the message. Stored as a millisecond representation of the Unix epoch."
-    )
-    opened: int = pydantic.Field(
-        description="A UTC timestamp at which the recipient opened a message for the first time. Stored as a millisecond representation of the Unix epoch."
-    )
-    clicked: int = pydantic.Field(
-        description="A UTC timestamp at which the recipient clicked on a tracked link for the first time. Stored as a millisecond representation of the Unix epoch."
-    )
-    recipient: str = pydantic.Field(
-        description="A unique identifier associated with the recipient of the delivered message."
-    )
-    event: str = pydantic.Field(description="A unique identifier associated with the event of the delivered message.")
-    notification: str = pydantic.Field(
-        description="A unique identifier associated with the notification of the delivered message."
-    )
-    error: typing.Optional[str] = pydantic.Field(description="A message describing the error that occurred.")
-    reason: typing.Optional[Reason] = pydantic.Field(description="The reason for the current status of the message.")
+
+class MessageDetails(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    A unique identifier associated with the message you wish to retrieve (results from a send).
+    """
+
+    status: MessageStatus = pydantic_v1.Field()
+    """
+    The current status of the message.
+    """
+
+    enqueued: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which Courier received the message request. Stored as a millisecond representation of the Unix epoch.
+    """
+
+    sent: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which Courier passed the message to the Integration provider. Stored as a millisecond representation of the Unix epoch.
+    """
+
+    delivered: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which the Integration provider delivered the message. Stored as a millisecond representation of the Unix epoch.
+    """
+
+    opened: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which the recipient opened a message for the first time. Stored as a millisecond representation of the Unix epoch.
+    """
+
+    clicked: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which the recipient clicked on a tracked link for the first time. Stored as a millisecond representation of the Unix epoch.
+    """
+
+    recipient: str = pydantic_v1.Field()
+    """
+    A unique identifier associated with the recipient of the delivered message.
+    """
+
+    event: str = pydantic_v1.Field()
+    """
+    A unique identifier associated with the event of the delivered message.
+    """
+
+    notification: str = pydantic_v1.Field()
+    """
+    A unique identifier associated with the notification of the delivered message.
+    """
+
+    error: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A message describing the error that occurred.
+    """
+
+    reason: typing.Optional[Reason] = pydantic_v1.Field(default=None)
+    """
+    The reason for the current status of the message.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/message_history_response.py` & `trycourier-6.0.1/src/courier/send/types/channel_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .message_details import MessageDetails
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .utm import Utm
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class MessageHistoryResponse(pydantic.BaseModel):
-    results: typing.List[MessageDetails]
+class ChannelMetadata(pydantic_v1.BaseModel):
+    utm: typing.Optional[Utm] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/render_output.py` & `trycourier-6.0.1/src/courier/messages/types/rendered_message_block.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .rendered_message_content import RenderedMessageContent
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RenderOutput(pydantic.BaseModel):
-    channel: str = pydantic.Field(description="The channel used for rendering the message.")
-    channel_id: str = pydantic.Field(description="The ID of channel used for rendering the message.")
-    content: RenderedMessageContent = pydantic.Field(description="Content details of the rendered message.")
+class RenderedMessageBlock(pydantic_v1.BaseModel):
+    type: str = pydantic_v1.Field()
+    """
+    The block type of the rendered message block.
+    """
+
+    text: str = pydantic_v1.Field()
+    """
+    The block text of the rendered message block.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/render_output_response.py` & `trycourier-6.0.1/src/courier/commons/types/already_exists.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .render_output import RenderOutput
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_error import BaseError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RenderOutputResponse(pydantic.BaseModel):
-    results: typing.List[RenderOutput] = pydantic.Field(
-        description="An array of render output of a previously sent message."
-    )
+class AlreadyExists(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_block.py` & `trycourier-6.0.1/src/courier/send/types/audience_recipient.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .audience_filter import AudienceFilter
+from .message_data import MessageData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class AudienceRecipient(pydantic_v1.BaseModel):
+    audience_id: str = pydantic_v1.Field()
+    """
+    A unique identifier associated with an Audience. A message will be sent to each user in the audience.
+    """
 
-class RenderedMessageBlock(pydantic.BaseModel):
-    type: str = pydantic.Field(description="The block type of the rendered message block.")
-    text: str = pydantic.Field(description="The block text of the rendered message block.")
+    data: typing.Optional[MessageData] = None
+    filters: typing.Optional[typing.List[AudienceFilter]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/messages/types/rendered_message_content.py` & `trycourier-6.0.1/src/courier/send/types/routing_strategy_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .rendered_message_block import RenderedMessageBlock
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .metadata import Metadata
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class RenderedMessageContent(pydantic.BaseModel):
-    html: str = pydantic.Field(description="The html content of the rendered message.")
-    title: str = pydantic.Field(description="The title of the rendered message.")
-    body: str = pydantic.Field(description="The body of the rendered message.")
-    subject: str = pydantic.Field(description="The subject of the rendered message.")
-    text: str = pydantic.Field(description="The text of the rendered message.")
-    blocks: typing.List[RenderedMessageBlock] = pydantic.Field(description="The blocks of the rendered message.")
+
+class RoutingStrategyProvider(pydantic_v1.BaseModel):
+    name: str
+    config: typing.Optional[typing.Dict[str, typing.Any]] = None
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    metadata: Metadata
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/__init__.py` & `trycourier-6.0.1/src/courier/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/__init__.py` & `trycourier-6.0.1/src/courier/notifications/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/base_check.py` & `trycourier-6.0.1/src/courier/send/types/routing_strategy_channel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .message_providers import MessageProviders
+from .routing_method import RoutingMethod
 
-from ....core.datetime_utils import serialize_datetime
-from .check_status import CheckStatus
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BaseCheck(pydantic.BaseModel):
-    id: str
-    status: CheckStatus
-    type: typing_extensions.Literal["custom"]
+class RoutingStrategyChannel(pydantic_v1.BaseModel):
+    channel: str
+    config: typing.Optional[typing.Dict[str, typing.Any]] = None
+    method: typing.Optional[RoutingMethod] = None
+    providers: typing.Optional[MessageProviders] = None
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/check.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .base_check import BaseCheck
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class Check(BaseCheck):
-    updated: int
+class SendToMsTeamsEmail(MsTeamsBaseProperties):
+    email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/message_routing.py` & `trycourier-6.0.1/src/courier/notifications/types/message_routing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .message_routing_method import MessageRoutingMethod
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class MessageRouting(pydantic.BaseModel):
+class MessageRouting(pydantic_v1.BaseModel):
     method: MessageRoutingMethod
     channels: typing.List[MessageRoutingChannel]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .message_routing_channel import MessageRoutingChannel  # noqa: E402
 
 MessageRouting.update_forward_refs()
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification.py` & `trycourier-6.0.1/src/courier/notifications/types/notification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .message_routing import MessageRouting
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Notification(pydantic.BaseModel):
+class Notification(pydantic_v1.BaseModel):
     created_at: int
     id: str
     routing: MessageRouting
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -24,8 +20,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_block.py` & `trycourier-6.0.1/src/courier/notifications/types/notification_channel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .block_type import BlockType
-from .notification_content import NotificationContent
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .notification_channel_content import NotificationChannelContent
 
 
-class NotificationBlock(pydantic.BaseModel):
-    alias: typing.Optional[str]
-    context: typing.Optional[str]
+class NotificationChannel(pydantic_v1.BaseModel):
     id: str
-    type: BlockType
-    content: typing.Optional[NotificationContent]
-    locales: typing.Optional[typing.Dict[str, NotificationContent]]
-    checksum: typing.Optional[str]
+    type: typing.Optional[str] = None
+    content: typing.Optional[NotificationChannelContent] = None
+    locales: typing.Optional[typing.Dict[str, NotificationChannelContent]] = None
+    checksum: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel.py` & `trycourier-6.0.1/src/courier/send/types/timeout.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .notification_channel_content import NotificationChannelContent
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .criteria import Criteria
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NotificationChannel(pydantic.BaseModel):
-    id: str
-    type: typing.Optional[str]
-    content: typing.Optional[NotificationChannelContent]
-    locales: typing.Optional[typing.Dict[str, NotificationChannelContent]]
-    checksum: typing.Optional[str]
+class Timeout(pydantic_v1.BaseModel):
+    provider: typing.Optional[typing.Dict[str, int]] = None
+    channel: typing.Optional[typing.Dict[str, int]] = None
+    message: typing.Optional[int] = None
+    escalation: typing.Optional[int] = None
+    criteria: typing.Optional[Criteria] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_channel_content.py` & `trycourier-6.0.1/src/courier/users/tokens/types/tracking.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NotificationChannelContent(pydantic.BaseModel):
-    subject: typing.Optional[str]
-    title: typing.Optional[str]
+class Tracking(pydantic_v1.BaseModel):
+    os_version: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The operating system version
+    """
+
+    ip: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The IP address of the device
+    """
+
+    lat: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The latitude of the device
+    """
+
+    long_: typing.Optional[str] = pydantic_v1.Field(alias="long", default=None)
+    """
+    The longitude of the device
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_content_hierarchy.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_ingest_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NotificationContentHierarchy(pydantic.BaseModel):
-    parent: typing.Optional[str]
-    children: typing.Optional[str]
+class BulkIngestError(pydantic_v1.BaseModel):
+    user: typing.Any
+    error: typing.Any
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_get_content_response.py` & `trycourier-6.0.1/src/courier/notifications/types/notification_block.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .notification_block import NotificationBlock
-from .notification_channel import NotificationChannel
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .block_type import BlockType
+from .notification_content import NotificationContent
 
 
-class NotificationGetContentResponse(pydantic.BaseModel):
-    blocks: typing.Optional[typing.List[NotificationBlock]]
-    channels: typing.Optional[typing.List[NotificationChannel]]
-    checksum: typing.Optional[str]
+class NotificationBlock(pydantic_v1.BaseModel):
+    alias: typing.Optional[str] = None
+    context: typing.Optional[str] = None
+    id: str
+    type: BlockType
+    content: typing.Optional[NotificationContent] = None
+    locales: typing.Optional[typing.Dict[str, NotificationContent]] = None
+    checksum: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/notification_list_response.py` & `trycourier-6.0.1/src/courier/send/types/email_head.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .notification import Notification
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class NotificationListResponse(pydantic.BaseModel):
-    paging: Paging
-    results: typing.List[Notification]
+class EmailHead(pydantic_v1.BaseModel):
+    inherit_default: bool = pydantic_v1.Field(alias="inheritDefault")
+    content: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_get_response.py` & `trycourier-6.0.1/src/courier/users/tokens/types/delete_user_token_opts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .check import Check
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubmissionChecksGetResponse(pydantic.BaseModel):
-    checks: typing.List[Check]
+class DeleteUserTokenOpts(pydantic_v1.BaseModel):
+    user_id: str
+    token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/notifications/types/submission_checks_replace_response.py` & `trycourier-6.0.1/src/courier/profiles/types/intercom_recipient.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .check import Check
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubmissionChecksReplaceResponse(pydantic.BaseModel):
-    checks: typing.List[Check]
+class IntercomRecipient(pydantic_v1.BaseModel):
+    id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/__init__.py` & `trycourier-6.0.1/src/courier/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/__init__.py` & `trycourier-6.0.1/src/courier/profiles/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/address.py` & `trycourier-6.0.1/src/courier/audiences/types/nested_filter_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_filter_config import BaseFilterConfig
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class NestedFilterConfig(BaseFilterConfig):
+    """
+    The operator to use for filtering
+    """
 
-class Address(pydantic.BaseModel):
-    formatted: str
-    street_address: str
-    locality: str
-    region: str
-    postal_code: str
-    country: str
+    rules: typing.List[FilterConfig]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+from .filter_config import FilterConfig  # noqa: E402
+
+NestedFilterConfig.update_forward_refs()
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile.py` & `trycourier-6.0.1/src/courier/automations/types/automation_fetch_data_webhook.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .airship_profile_audience import AirshipProfileAudience
-from .device_type import DeviceType
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_fetch_data_webhook_method import AutomationFetchDataWebhookMethod
 
 
-class AirshipProfile(pydantic.BaseModel):
-    audience: AirshipProfileAudience
-    device_types: typing.List[DeviceType]
+class AutomationFetchDataWebhook(pydantic_v1.BaseModel):
+    body: typing.Optional[typing.Dict[str, typing.Any]] = None
+    headers: typing.Optional[typing.Dict[str, typing.Any]] = None
+    params: typing.Optional[typing.Dict[str, typing.Any]] = None
+    method: AutomationFetchDataWebhookMethod
+    url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/airship_profile_audience.py` & `trycourier-6.0.1/src/courier/send/types/message_context.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AirshipProfileAudience(pydantic.BaseModel):
-    named_user: str
+class MessageContext(pydantic_v1.BaseModel):
+    tenant_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    An id of a tenant, see [tenants api docs](https://www.courier.com/docs/reference/tenants/).
+    Will load brand, default preferences and any other base context data associated with this tenant.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/delete_list_subscription_response.py` & `trycourier-6.0.1/src/courier/profiles/types/delete_list_subscription_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class DeleteListSubscriptionResponse(pydantic.BaseModel):
-    status: typing_extensions.Literal["SUCCESS"]
+class DeleteListSubscriptionResponse(pydantic_v1.BaseModel):
+    status: typing.Literal["SUCCESS"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_list.py` & `trycourier-6.0.1/src/courier/users/preferences/types/topic_preference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ....commons.types.channel_classification import ChannelClassification
+from ....commons.types.preference_status import PreferenceStatus
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.recipient_preferences import RecipientPreferences
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class GetListSubscriptionsList(pydantic.BaseModel):
-    id: str
-    name: str = pydantic.Field(description="List name")
-    created: str = pydantic.Field(
-        description="The date/time of when the list was created. Represented as a string in ISO format."
-    )
-    updated: str = pydantic.Field(
-        description="The date/time of when the list was updated. Represented as a string in ISO format."
-    )
-    preferences: typing.Optional[RecipientPreferences]
+
+class TopicPreference(pydantic_v1.BaseModel):
+    custom_routing: typing.Optional[typing.List[ChannelClassification]] = pydantic_v1.Field(default=None)
+    """
+    The Channels a user has chosen to receive notifications through for this topic
+    """
+
+    default_status: PreferenceStatus
+    has_custom_routing: typing.Optional[bool] = None
+    status: PreferenceStatus
+    topic_id: str
+    topic_name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/get_list_subscriptions_response.py` & `trycourier-6.0.1/src/courier/users/preferences/types/user_preferences_list_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ....commons.types.paging import Paging
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .get_list_subscriptions_list import GetListSubscriptionsList
+from ....core.pydantic_utilities import pydantic_v1
+from .topic_preference import TopicPreference
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetListSubscriptionsResponse(pydantic.BaseModel):
+class UserPreferencesListResponse(pydantic_v1.BaseModel):
     paging: Paging
-    results: typing.List[GetListSubscriptionsList] = pydantic.Field(description="An array of lists")
+    items: typing.List[TopicPreference] = pydantic_v1.Field()
+    """
+    The Preferences associated with the user_id.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom.py` & `trycourier-6.0.1/src/courier/automations/types/automation_invoke_template_params.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .intercom_recipient import IntercomRecipient
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_invoke_params import AutomationInvokeParams
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Intercom(pydantic.BaseModel):
-    from_: str = pydantic.Field(alias="from")
-    to: IntercomRecipient
+class AutomationInvokeTemplateParams(AutomationInvokeParams):
+    template_id: str = pydantic_v1.Field(alias="templateId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/intercom_recipient.py` & `trycourier-6.0.1/src/courier/automations/types/automation_throttle_on_throttle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class IntercomRecipient(pydantic.BaseModel):
-    id: str
+class AutomationThrottleOnThrottle(pydantic_v1.BaseModel):
+    node_id: str = pydantic_v1.Field(alias="$node_id")
+    """
+    The node to go to if the request is throttled
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/merge_profile_response.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_users_params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class MergeProfileResponse(pydantic.BaseModel):
-    status: typing_extensions.Literal["SUCCESS"]
+class BulkGetJobUsersParams(pydantic_v1.BaseModel):
+    job_id: str = pydantic_v1.Field(alias="jobId")
+    cursor: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/ms_teams.py` & `trycourier-6.0.1/src/courier/profiles/types/ms_teams.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/ms_teams_base_properties.py` & `trycourier-6.0.1/src/courier/users/tokens/types/put_user_token_opts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
+from .user_token import UserToken
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class MsTeamsBaseProperties(pydantic.BaseModel):
-    tenant_id: str
-    service_url: str
+class PutUserTokenOpts(pydantic_v1.BaseModel):
+    user_id: str
+    token: UserToken
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/multiple_tokens.py` & `trycourier-6.0.1/src/courier/audiences/types/audience_update_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .token import Token
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .audience import Audience
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class MultipleTokens(pydantic.BaseModel):
-    tokens: typing.List[Token]
+class AudienceUpdateResponse(pydantic_v1.BaseModel):
+    audience: Audience
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_parameters.py` & `trycourier-6.0.1/src/courier/templates/types/list_templates_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...commons.types.paging import Paging
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .notification_templates import NotificationTemplates
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ProfileGetParameters(pydantic.BaseModel):
-    recipient_id: str = pydantic.Field(alias="recipientId")
+class ListTemplatesResponse(pydantic_v1.BaseModel):
+    paging: Paging
+    results: typing.List[NotificationTemplates] = pydantic_v1.Field()
+    """
+    An array of Notification Templates
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/profile_get_response.py` & `trycourier-6.0.1/src/courier/commons/types/bad_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_error import BaseError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ProfileGetResponse(pydantic.BaseModel):
-    profile: typing.Dict[str, typing.Any]
-    preferences: typing.Optional[RecipientPreferences]
+class BadRequest(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/replace_profile_response.py` & `trycourier-6.0.1/src/courier/audiences/types/audience_member.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ReplaceProfileResponse(pydantic.BaseModel):
-    status: typing_extensions.Literal["SUCCESS"]
+class AudienceMember(pydantic_v1.BaseModel):
+    added_at: str
+    audience_id: str
+    audience_version: int
+    member_id: str
+    reason: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_direct_message.py` & `trycourier-6.0.1/src/courier/send/types/user_recipient_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class SendDirectMessage(pydantic.BaseModel):
-    user_id: str
 
+class UserRecipientType(pydantic_v1.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_channel.py` & `trycourier-6.0.1/src/courier/commons/types/message_not_found.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_error import BaseError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SendToChannel(pydantic.BaseModel):
-    channel_id: str
+class MessageNotFound(BaseError):
+    type: typing.Literal["invalid_request_error"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_channel_id.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_user_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class SendToMsTeamsChannelId(MsTeamsBaseProperties):
-    channel_id: str
+class SendToMsTeamsUserId(MsTeamsBaseProperties):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_channel_name.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_create_job_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .ms_teams_base_properties import MsTeamsBaseProperties
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class SendToMsTeamsChannelName(MsTeamsBaseProperties):
-    channel_name: str
-    team_id: str
+class BulkCreateJobResponse(pydantic_v1.BaseModel):
+    job_id: str = pydantic_v1.Field(alias="jobId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_conversation_id.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_channel_name.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .ms_teams_base_properties import MsTeamsBaseProperties
 
 
-class SendToMsTeamsConversationId(MsTeamsBaseProperties):
-    conversation_id: str
+class SendToMsTeamsChannelName(MsTeamsBaseProperties):
+    channel_name: str
+    team_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_email.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_slack_email.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .ms_teams_base_properties import MsTeamsBaseProperties
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .slack_base_properties import SlackBaseProperties
 
 
-class SendToMsTeamsEmail(MsTeamsBaseProperties):
+class SendToSlackEmail(SlackBaseProperties):
     email: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_ms_teams_user_id.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_slack_user_id.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .ms_teams_base_properties import MsTeamsBaseProperties
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .slack_base_properties import SlackBaseProperties
 
 
-class SendToMsTeamsUserId(MsTeamsBaseProperties):
+class SendToSlackUserId(SlackBaseProperties):
     user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_channel.py` & `trycourier-6.0.1/src/courier/profiles/types/profile_get_parameters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .slack_base_properties import SlackBaseProperties
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class SendToSlackChannel(SlackBaseProperties):
-    channel: str
+class ProfileGetParameters(pydantic_v1.BaseModel):
+    recipient_id: str = pydantic_v1.Field(alias="recipientId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_email.py` & `trycourier-6.0.1/src/courier/users/tokens/types/get_user_token_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .slack_base_properties import SlackBaseProperties
+from ....core.pydantic_utilities import pydantic_v1
+from .token_status import TokenStatus
+from .user_token import UserToken
 
 
-class SendToSlackEmail(SlackBaseProperties):
-    email: str
+class GetUserTokenResponse(UserToken):
+    status: typing.Optional[TokenStatus] = None
+    status_reason: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The reason for the token status.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/send_to_slack_user_id.py` & `trycourier-6.0.1/src/courier/commons/types/user_tenant_association.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .slack_base_properties import SlackBaseProperties
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class SendToSlackUserId(SlackBaseProperties):
-    user_id: str
+class UserTenantAssociation(pydantic_v1.BaseModel):
+    user_id: str = pydantic_v1.Field()
+    """
+    User ID for the assocation between tenant and user
+    """
+
+    type: typing.Literal["user"]
+    tenant_id: str = pydantic_v1.Field()
+    """
+    Tenant ID for the assocation between tenant and user
+    """
+
+    profile: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/slack_base_properties.py` & `trycourier-6.0.1/src/courier/templates/types/tag_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SlackBaseProperties(pydantic.BaseModel):
-    access_token: str
+class TagData(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    A unique identifier of the tag.
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    Name of the tag.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/snooze_rule.py` & `trycourier-6.0.1/src/courier/send/types/invalid_list_recipient.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .snooze_rule_type import SnoozeRuleType
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SnoozeRule(pydantic.BaseModel):
-    type: SnoozeRuleType
-    start: str
-    until: str
+class InvalidListRecipient(pydantic_v1.BaseModel):
+    user_id: str
+    list_pattern: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request.py` & `trycourier-6.0.1/src/courier/send/types/brand_settings_email.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .subscribe_to_lists_request_list_object import SubscribeToListsRequestListObject
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .brand_template_override import BrandTemplateOverride
+from .email_footer import EmailFooter
+from .email_head import EmailHead
+from .email_header import EmailHeader
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubscribeToListsRequest(pydantic.BaseModel):
-    lists: typing.List[SubscribeToListsRequestListObject]
+class BrandSettingsEmail(pydantic_v1.BaseModel):
+    template_override: typing.Optional[BrandTemplateOverride] = pydantic_v1.Field(
+        alias="templateOverride", default=None
+    )
+    head: typing.Optional[EmailHead] = None
+    footer: typing.Optional[EmailFooter] = None
+    header: typing.Optional[EmailHeader] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_request_list_object.py` & `trycourier-6.0.1/src/courier/send/types/brand_template_override.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .brand_template import BrandTemplate
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubscribeToListsRequestListObject(pydantic.BaseModel):
-    list_id: str = pydantic.Field(alias="listId")
-    preferences: typing.Optional[RecipientPreferences]
+class BrandTemplateOverride(BrandTemplate):
+    mjml: BrandTemplate
+    footer_background_color: typing.Optional[str] = pydantic_v1.Field(alias="footerBackgroundColor", default=None)
+    footer_full_width: typing.Optional[bool] = pydantic_v1.Field(alias="footerFullWidth", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/subscribe_to_lists_response.py` & `trycourier-6.0.1/src/courier/profiles/types/subscribe_to_lists_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class SubscribeToListsResponse(pydantic.BaseModel):
-    status: typing_extensions.Literal["SUCCESS"]
+class SubscribeToListsResponse(pydantic_v1.BaseModel):
+    status: typing.Literal["SUCCESS"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/token.py` & `trycourier-6.0.1/src/courier/tenants/types/default_preferences.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .subscription_topic import SubscriptionTopic
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Token(pydantic.BaseModel):
-    token: str
+class DefaultPreferences(pydantic_v1.BaseModel):
+    items: typing.List[SubscriptionTopic]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/profiles/types/user_profile.py` & `trycourier-6.0.1/src/courier/profiles/types/user_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .address import Address
 from .airship_profile import AirshipProfile
 from .discord import Discord
 from .expo import Expo
 from .intercom import Intercom
 from .ms_teams import MsTeams
 from .slack import Slack
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UserProfile(pydantic.BaseModel):
+class UserProfile(pydantic_v1.BaseModel):
     address: Address
     birthdate: str
     email: str
     email_verified: bool
     family_name: str
     gender: str
     given_name: str
@@ -35,24 +31,26 @@
     picture: str
     preferred_name: str
     profile: str
     sub: str
     updated_at: str
     website: str
     zoneinfo: str
-    custom: typing.Any = pydantic.Field(
-        description="A free form object. Due to a limitation of the API Explorer, you can only enter string key/values below, but this API accepts more complex object structures."
-    )
+    custom: typing.Any = pydantic_v1.Field()
+    """
+    A free form object. Due to a limitation of the API Explorer, you can only enter string key/values below, but this API accepts more complex object structures.
+    """
+
     airship: AirshipProfile
     apn: str
     target_arn: str
     discord: Discord
     expo: Expo
-    facebook_psid: str = pydantic.Field(alias="facebookPSID")
-    firebase_token: str = pydantic.Field(alias="firebaseToken")
+    facebook_psid: str = pydantic_v1.Field(alias="facebookPSID")
+    firebase_token: str = pydantic_v1.Field(alias="firebaseToken")
     intercom: Intercom
     slack: Slack
     ms_teams: MsTeams
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -61,8 +59,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/__init__.py` & `trycourier-6.0.1/src/courier/send/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Attachment,
     AudienceFilter,
     AudienceRecipient,
     BaseMessage,
+    BaseMessageSendTo,
     BaseSocialPresence,
     BrandSettingsEmail,
     BrandSettingsInApp,
     BrandSettingsSocialPresence,
     BrandTemplate,
     BrandTemplateOverride,
     Channel,
@@ -66,24 +67,27 @@
     MessageContext,
     MessageData,
     MessageMetadata,
     MessageProviders,
     MessageProvidersType,
     MessageRecipient,
     Metadata,
+    MsTeamsRecipient,
     Override,
     Preference,
     Preferences,
     Recipient,
+    RecipientData,
     Routing,
     RoutingChannel,
     RoutingMethod,
     RoutingStrategyChannel,
     RoutingStrategyProvider,
     RuleType,
+    SlackRecipient,
     TemplateMessage,
     TextAlign,
     TextStyle,
     Timeout,
     Timeouts,
     TrackingOverride,
     UserRecipient,
@@ -93,14 +97,15 @@
 )
 
 __all__ = [
     "Attachment",
     "AudienceFilter",
     "AudienceRecipient",
     "BaseMessage",
+    "BaseMessageSendTo",
     "BaseSocialPresence",
     "BrandSettingsEmail",
     "BrandSettingsInApp",
     "BrandSettingsSocialPresence",
     "BrandTemplate",
     "BrandTemplateOverride",
     "Channel",
@@ -158,24 +163,27 @@
     "MessageContext",
     "MessageData",
     "MessageMetadata",
     "MessageProviders",
     "MessageProvidersType",
     "MessageRecipient",
     "Metadata",
+    "MsTeamsRecipient",
     "Override",
     "Preference",
     "Preferences",
     "Recipient",
+    "RecipientData",
     "Routing",
     "RoutingChannel",
     "RoutingMethod",
     "RoutingStrategyChannel",
     "RoutingStrategyProvider",
     "RuleType",
+    "SlackRecipient",
     "TemplateMessage",
     "TextAlign",
     "TextStyle",
     "Timeout",
     "Timeouts",
     "TrackingOverride",
     "UserRecipient",
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/__init__.py` & `trycourier-6.0.1/src/courier/send/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .attachment import Attachment
 from .audience_filter import AudienceFilter
 from .audience_recipient import AudienceRecipient
 from .base_message import BaseMessage
+from .base_message_send_to import BaseMessageSendTo
 from .base_social_presence import BaseSocialPresence
 from .brand_settings_email import BrandSettingsEmail
 from .brand_settings_in_app import BrandSettingsInApp
 from .brand_settings_social_presence import BrandSettingsSocialPresence
 from .brand_template import BrandTemplate
 from .brand_template_override import BrandTemplateOverride
 from .channel import Channel
@@ -67,24 +68,27 @@
 from .message_context import MessageContext
 from .message_data import MessageData
 from .message_metadata import MessageMetadata
 from .message_providers import MessageProviders
 from .message_providers_type import MessageProvidersType
 from .message_recipient import MessageRecipient
 from .metadata import Metadata
+from .ms_teams_recipient import MsTeamsRecipient
 from .override import Override
 from .preference import Preference
 from .preferences import Preferences
 from .recipient import Recipient
+from .recipient_data import RecipientData
 from .routing import Routing
 from .routing_channel import RoutingChannel
 from .routing_method import RoutingMethod
 from .routing_strategy_channel import RoutingStrategyChannel
 from .routing_strategy_provider import RoutingStrategyProvider
 from .rule_type import RuleType
+from .slack_recipient import SlackRecipient
 from .template_message import TemplateMessage
 from .text_align import TextAlign
 from .text_style import TextStyle
 from .timeout import Timeout
 from .timeouts import Timeouts
 from .tracking_override import TrackingOverride
 from .user_recipient import UserRecipient
@@ -93,14 +97,15 @@
 from .widget_background import WidgetBackground
 
 __all__ = [
     "Attachment",
     "AudienceFilter",
     "AudienceRecipient",
     "BaseMessage",
+    "BaseMessageSendTo",
     "BaseSocialPresence",
     "BrandSettingsEmail",
     "BrandSettingsInApp",
     "BrandSettingsSocialPresence",
     "BrandTemplate",
     "BrandTemplateOverride",
     "Channel",
@@ -158,24 +163,27 @@
     "MessageContext",
     "MessageData",
     "MessageMetadata",
     "MessageProviders",
     "MessageProvidersType",
     "MessageRecipient",
     "Metadata",
+    "MsTeamsRecipient",
     "Override",
     "Preference",
     "Preferences",
     "Recipient",
+    "RecipientData",
     "Routing",
     "RoutingChannel",
     "RoutingMethod",
     "RoutingStrategyChannel",
     "RoutingStrategyProvider",
     "RuleType",
+    "SlackRecipient",
     "TemplateMessage",
     "TextAlign",
     "TextStyle",
     "Timeout",
     "Timeouts",
     "TrackingOverride",
     "UserRecipient",
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/audience_filter.py` & `trycourier-6.0.1/src/courier/send/types/ms_teams_recipient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...profiles.types.ms_teams import MsTeams
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class AudienceFilter(pydantic.BaseModel):
-    operator: typing_extensions.Literal["MEMBER_OF"] = pydantic.Field(
-        description="Send to users only if they are member of the account"
-    )
-    path: typing_extensions.Literal["account_id"]
-    value: str
+class MsTeamsRecipient(pydantic_v1.BaseModel):
+    ms_teams: MsTeams
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/audience_recipient.py` & `trycourier-6.0.1/src/courier/notifications/types/base_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .audience_filter import AudienceFilter
-from .message_data import MessageData
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class AudienceRecipient(pydantic.BaseModel):
-    audience_id: str = pydantic.Field(
-        description="A unique identifier associated with an Audience. A message will be sent to each user in the audience."
-    )
-    data: typing.Optional[MessageData]
-    filters: typing.Optional[typing.List[AudienceFilter]]
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .check_status import CheckStatus
+
+
+class BaseCheck(pydantic_v1.BaseModel):
+    id: str
+    status: CheckStatus
+    type: typing.Literal["custom"]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/base_message.py` & `trycourier-6.0.1/src/courier/send/types/base_message.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,76 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .delay import Delay
 from .expiry import Expiry
 from .message_channels import MessageChannels
 from .message_context import MessageContext
 from .message_data import MessageData
 from .message_metadata import MessageMetadata
 from .message_providers import MessageProviders
 from .routing import Routing
 from .timeout import Timeout
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BaseMessage(pydantic.BaseModel):
-    data: typing.Optional[MessageData] = pydantic.Field(
-        description=(
-            "An arbitrary object that includes any data you want to pass to the message.\n"
-            "The data will populate the corresponding template or elements variables.\n"
-        )
-    )
-    brand_id: typing.Optional[str]
-    channels: typing.Optional[MessageChannels] = pydantic.Field(
-        description="\"Define run-time configuration for one or more channels. If you don't specify channels, the default configuration for each channel will be used. Valid ChannelId's are: email, sms, push, inbox, direct_message, banner, and webhook.\""
-    )
-    context: typing.Optional[MessageContext] = pydantic.Field(
-        description="Context to load with this recipient. Will override any context set on message.context."
-    )
-    metadata: typing.Optional[MessageMetadata] = pydantic.Field(
-        description="Metadata such as utm tracking attached with the notification through this channel."
-    )
-    providers: typing.Optional[MessageProviders] = pydantic.Field(
-        description="An object whose keys are valid provider identifiers which map to an object."
-    )
-    routing: typing.Optional[Routing]
-    timeout: typing.Optional[Timeout] = pydantic.Field(
-        description="Time in ms to attempt the channel before failing over to the next available channel."
-    )
-    delay: typing.Optional[Delay] = pydantic.Field(
-        description="Defines the time to wait before delivering the message."
-    )
-    expiry: typing.Optional[Expiry] = pydantic.Field(
-        description=(
-            '"Expiry allows you to set an absolute or relative time in which a message expires.\n'
-            'Note: This is only valid for the Courier Inbox channel as of 12-08-2022."\n'
-        )
-    )
+
+class BaseMessage(pydantic_v1.BaseModel):
+    data: typing.Optional[MessageData] = pydantic_v1.Field(default=None)
+    """
+    An arbitrary object that includes any data you want to pass to the message.
+    The data will populate the corresponding template or elements variables.
+    """
+
+    brand_id: typing.Optional[str] = None
+    channels: typing.Optional[MessageChannels] = pydantic_v1.Field(default=None)
+    """
+    "Define run-time configuration for one or more channels. If you don't specify channels, the default configuration for each channel will be used. Valid ChannelId's are: email, sms, push, inbox, direct_message, banner, and webhook."
+    """
+
+    context: typing.Optional[MessageContext] = pydantic_v1.Field(default=None)
+    """
+    Context to load with this recipient. Will override any context set on message.context.
+    """
+
+    metadata: typing.Optional[MessageMetadata] = pydantic_v1.Field(default=None)
+    """
+    Metadata such as utm tracking attached with the notification through this channel.
+    """
+
+    providers: typing.Optional[MessageProviders] = pydantic_v1.Field(default=None)
+    """
+    An object whose keys are valid provider identifiers which map to an object.
+    """
+
+    routing: typing.Optional[Routing] = None
+    timeout: typing.Optional[Timeout] = pydantic_v1.Field(default=None)
+    """
+    Time in ms to attempt the channel before failing over to the next available channel.
+    """
+
+    delay: typing.Optional[Delay] = pydantic_v1.Field(default=None)
+    """
+    Defines the time to wait before delivering the message.
+    """
+
+    expiry: typing.Optional[Expiry] = pydantic_v1.Field(default=None)
+    """
+    "Expiry allows you to set an absolute or relative time in which a message expires.
+    Note: This is only valid for the Courier Inbox channel as of 12-08-2022."
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/base_social_presence.py` & `trycourier-6.0.1/src/courier/automations/types/automation_step.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BaseSocialPresence(pydantic.BaseModel):
-    url: str
+class AutomationStep(pydantic_v1.BaseModel):
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    ref: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_email.py` & `trycourier-6.0.1/src/courier/send/types/brand_settings_in_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .brand_template_override import BrandTemplateOverride
-from .email_footer import EmailFooter
-from .email_head import EmailHead
-from .email_header import EmailHeader
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BrandSettingsEmail(pydantic.BaseModel):
-    template_override: typing.Optional[BrandTemplateOverride] = pydantic.Field(alias="templateOverride")
-    head: typing.Optional[EmailHead]
-    footer: typing.Optional[EmailFooter]
-    header: typing.Optional[EmailHeader]
+from ...brands.types.brand_colors import BrandColors
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .icons import Icons
+from .in_app_placement import InAppPlacement
+from .preferences import Preferences
+from .widget_background import WidgetBackground
+
+
+class BrandSettingsInApp(pydantic_v1.BaseModel):
+    border_radius: typing.Optional[str] = pydantic_v1.Field(alias="borderRadius", default=None)
+    disable_message_icon: typing.Optional[bool] = pydantic_v1.Field(alias="disableMessageIcon", default=None)
+    font_family: typing.Optional[str] = pydantic_v1.Field(alias="fontFamily", default=None)
+    placement: typing.Optional[InAppPlacement] = None
+    widget_background: WidgetBackground = pydantic_v1.Field(alias="widgetBackground")
+    colors: BrandColors
+    icons: Icons
+    preferences: Preferences
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_in_app.py` & `trycourier-6.0.1/src/courier/send/types/brand_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...brands.types.brand_colors import BrandColors
-from .icons import Icons
-from .in_app_placement import InAppPlacement
-from .preferences import Preferences
-from .widget_background import WidgetBackground
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BrandSettingsInApp(pydantic.BaseModel):
-    border_radius: typing.Optional[str] = pydantic.Field(alias="borderRadius")
-    disable_message_icon: typing.Optional[bool] = pydantic.Field(alias="disableMessageIcon")
-    font_family: typing.Optional[str] = pydantic.Field(alias="fontFamily")
-    placement: typing.Optional[InAppPlacement]
-    widget_background: WidgetBackground = pydantic.Field(alias="widgetBackground")
-    colors: BrandColors
-    icons: Icons
-    preferences: Preferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+
+
+class BrandTemplate(pydantic_v1.BaseModel):
+    background_color: typing.Optional[str] = pydantic_v1.Field(alias="backgroundColor", default=None)
+    blocks_background_color: typing.Optional[str] = pydantic_v1.Field(alias="blocksBackgroundColor", default=None)
+    enabled: bool
+    footer: typing.Optional[str] = None
+    head: typing.Optional[str] = None
+    header: typing.Optional[str] = None
+    width: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/brand_settings_social_presence.py` & `trycourier-6.0.1/src/courier/send/types/brand_settings_social_presence.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .base_social_presence import BaseSocialPresence
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BrandSettingsSocialPresence(pydantic.BaseModel):
-    inherit_default: typing.Optional[bool] = pydantic.Field(alias="inheritDefault")
-    facebook: typing.Optional[BaseSocialPresence]
-    instagram: typing.Optional[BaseSocialPresence]
-    linkedin: typing.Optional[BaseSocialPresence]
-    medium: typing.Optional[BaseSocialPresence]
-    twitter: typing.Optional[BaseSocialPresence]
+class BrandSettingsSocialPresence(pydantic_v1.BaseModel):
+    inherit_default: typing.Optional[bool] = pydantic_v1.Field(alias="inheritDefault", default=None)
+    facebook: typing.Optional[BaseSocialPresence] = None
+    instagram: typing.Optional[BaseSocialPresence] = None
+    linkedin: typing.Optional[BaseSocialPresence] = None
+    medium: typing.Optional[BaseSocialPresence] = None
+    twitter: typing.Optional[BaseSocialPresence] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/brand_template.py` & `trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_message_v_1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class BrandTemplate(pydantic.BaseModel):
-    background_color: typing.Optional[str] = pydantic.Field(alias="backgroundColor")
-    blocks_background_color: typing.Optional[str] = pydantic.Field(alias="blocksBackgroundColor")
-    enabled: bool
-    footer: typing.Optional[str]
-    head: typing.Optional[str]
-    header: typing.Optional[str]
-    width: typing.Optional[str]
+
+class InboundBulkMessageV1(pydantic_v1.BaseModel):
+    brand: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A unique identifier that represents the brand that should be used
+    for rendering the notification.
+    """
+
+    data: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    JSON that includes any data you want to pass to a message template.
+    The data will populate the corresponding template variables.
+    """
+
+    event: typing.Optional[str] = None
+    locale: typing.Optional[typing.Dict[str, typing.Any]] = None
+    override: typing.Optional[typing.Any] = pydantic_v1.Field(default=None)
+    """
+    JSON that is merged into the request sent by Courier to the provider
+    to override properties or to gain access to features in the provider
+    API that are not natively supported by Courier.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/brand_template_override.py` & `trycourier-6.0.1/src/courier/audit_events/types/audit_event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .brand_template import BrandTemplate
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .actor import Actor
+from .target import Target
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BrandTemplateOverride(BrandTemplate):
-    mjml: BrandTemplate
-    footer_background_color: typing.Optional[str] = pydantic.Field(alias="footerBackgroundColor")
-    footer_full_width: typing.Optional[bool] = pydantic.Field(alias="footerFullWidth")
+class AuditEvent(pydantic_v1.BaseModel):
+    actor: typing.Optional[Actor] = None
+    target: typing.Optional[Target] = None
+    audit_event_id: str = pydantic_v1.Field(alias="auditEventId")
+    source: str
+    timestamp: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/channel.py` & `trycourier-6.0.1/src/courier/send/types/channel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .channel_metadata import ChannelMetadata
 from .override import Override
 from .routing_method import RoutingMethod
 from .timeouts import Timeouts
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Channel(pydantic.BaseModel):
-    brand_id: typing.Optional[str] = pydantic.Field(
-        description=(
-            "Id of the brand that should be used for rendering the message.\n"
-            "If not specified, the brand configured as default brand will be used.\n"
-        )
-    )
-    providers: typing.Optional[typing.List[str]] = pydantic.Field(
-        description=(
-            "A list of providers enabled for this channel. Courier will select\n"
-            "one provider to send through unless routing_method is set to all.\n"
-        )
-    )
-    routing_method: typing.Optional[RoutingMethod] = pydantic.Field(
-        description=(
-            "The method for selecting the providers to send the message with.\n"
-            "Single will send to one of the available providers for this channel,\n"
-            "all will send the message through all channels. Defaults to `single`.\n"
-        )
-    )
-    if_: typing.Optional[str] = pydantic.Field(
-        alias="if",
-        description=(
-            "A JavaScript conditional expression to determine if the message should\n"
-            "be sent through the channel. Has access to the data and profile object.\n"
-            "For example, `data.name === profile.name`\n"
-        ),
-    )
-    timeouts: typing.Optional[Timeouts]
-    override: typing.Optional[Override] = pydantic.Field(description="Channel specific overrides.")
-    metadata: typing.Optional[ChannelMetadata]
+
+class Channel(pydantic_v1.BaseModel):
+    brand_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Id of the brand that should be used for rendering the message.
+    If not specified, the brand configured as default brand will be used.
+    """
+
+    providers: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    A list of providers enabled for this channel. Courier will select
+    one provider to send through unless routing_method is set to all.
+    """
+
+    routing_method: typing.Optional[RoutingMethod] = pydantic_v1.Field(default=None)
+    """
+    The method for selecting the providers to send the message with.
+    Single will send to one of the available providers for this channel,
+    all will send the message through all channels. Defaults to `single`.
+    """
+
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    """
+    A JavaScript conditional expression to determine if the message should
+    be sent through the channel. Has access to the data and profile object.
+    For example, `data.name === profile.name`
+    """
+
+    timeouts: typing.Optional[Timeouts] = None
+    override: typing.Optional[Override] = pydantic_v1.Field(default=None)
+    """
+    Channel specific overrides.
+    """
+
+    metadata: typing.Optional[ChannelMetadata] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/channel_metadata.py` & `trycourier-6.0.1/src/courier/send/types/template_message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .utm import Utm
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_message import BaseMessage
+from .base_message_send_to import BaseMessageSendTo
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ChannelMetadata(pydantic.BaseModel):
-    utm: typing.Optional[Utm]
+class TemplateMessage(BaseMessage, BaseMessageSendTo):
+    template: str = pydantic_v1.Field()
+    """
+    The id of the notification template to be rendered and sent to the recipient(s).
+    This field or the content field must be supplied.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/content_message.py` & `trycourier-6.0.1/src/courier/automations/types/automation_add_to_batch_retain.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .base_message import BaseMessage
-from .content import Content
-from .message_recipient import MessageRecipient
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_add_to_batch_retain_type import AutomationAddToBatchRetainType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class AutomationAddToBatchRetain(pydantic_v1.BaseModel):
+    """
+    Defines what items should be retained and passed along to the next steps when the batch is released
+    ---
+    from courier import AutomationAddToBatchRetain
+
+    AutomationAddToBatchRetain(
+        type="highest",
+        count=10,
+        sort_key="refs.data.my_custom_scoring",
+    )
+    """
 
-class ContentMessage(BaseMessage):
+    type: AutomationAddToBatchRetainType = pydantic_v1.Field()
     """
-    The message property has the following primary top-level properties. They define the destination and content of the message.
-    Additional advanced configuration fields [are defined below](https://www.courier.com/docs/reference/send/message/#other-message-properties).
+    Keep N number of notifications based on the type. First/Last N based on notification received.
+    highest/lowest based on a scoring key providing in the data accessed by sort_key
     """
 
-    content: Content = pydantic.Field(
-        description=(
-            "Describes the content of the message in a way that will work for email, push,\n"
-            "chat, or any channel. Either this or template must be specified.\n"
-        )
-    )
-    to: MessageRecipient = pydantic.Field(description="The recipient or a list of recipients of the message")
+    count: int = pydantic_v1.Field()
+    """
+    The number of records to keep in batch. Default is 10 and only configurable by requesting from support.
+    When configurable minimum is 2 and maximum is 100.
+    """
+
+    sort_key: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Defines the data value data[sort_key] that is used to sort the stored items. Required when type is set to highest or lowest.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/delay.py` & `trycourier-6.0.1/src/courier/users/tokens/types/patch_user_token_opts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
+from .patch_operation import PatchOperation
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Delay(pydantic.BaseModel):
-    duration: int = pydantic.Field(description="The duration of the delay in milliseconds.")
+class PatchUserTokenOpts(pydantic_v1.BaseModel):
+    patch: typing.List[PatchOperation]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_action_node.py` & `trycourier-6.0.1/src/courier/send/types/elemental_action_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 from .i_action_button_style import IActionButtonStyle
 from .i_alignment import IAlignment
 from .locales import Locales
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class ElementalActionNode(ElementalBaseNode):
     """
     Allows the user to execute an action. Can be a button or a link.
     """
 
-    content: str = pydantic.Field(description="The text content of the action shown to the user.")
-    href: str = pydantic.Field(description="The target URL of the action.")
-    action_id: typing.Optional[str] = pydantic.Field(
-        description="A unique id used to identify the action when it is executed."
-    )
-    align: typing.Optional[IAlignment] = pydantic.Field(
-        description='The alignment of the action button. Defaults to "center".'
-    )
-    background_color: typing.Optional[str] = pydantic.Field(description="The background color of the action button.")
-    style: typing.Optional[IActionButtonStyle] = pydantic.Field(description="Defaults to `button`.")
-    locales: Locales = pydantic.Field(
-        description="Region specific content. See [locales docs](https://www.courier.com/docs/platform/content/elemental/locales/) for more details."
-    )
+    content: str = pydantic_v1.Field()
+    """
+    The text content of the action shown to the user.
+    """
+
+    href: str = pydantic_v1.Field()
+    """
+    The target URL of the action.
+    """
+
+    action_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A unique id used to identify the action when it is executed.
+    """
+
+    align: typing.Optional[IAlignment] = pydantic_v1.Field(default=None)
+    """
+    The alignment of the action button. Defaults to "center".
+    """
+
+    background_color: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The background color of the action button.
+    """
+
+    style: typing.Optional[IActionButtonStyle] = pydantic_v1.Field(default=None)
+    """
+    Defaults to `button`.
+    """
+
+    locales: Locales = pydantic_v1.Field()
+    """
+    Region specific content. See [locales docs](https://www.courier.com/docs/platform/content/elemental/locales/) for more details.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_base_node.py` & `trycourier-6.0.1/src/courier/automations/types/automation_invoke_step.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_step import AutomationStep
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ElementalBaseNode(pydantic.BaseModel):
-    channels: typing.Optional[typing.List[str]]
-    ref: typing.Optional[str]
-    if_: typing.Optional[str] = pydantic.Field(alias="if")
-    loop: typing.Optional[str]
+class AutomationInvokeStep(AutomationStep):
+    action: typing.Literal["invoke"]
+    template: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_channel_node.py` & `trycourier-6.0.1/src/courier/send/types/elemental_channel_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class ElementalChannelNode(ElementalBaseNode):
     """
     The channel element allows a notification to be customized based on which channel it is sent through.
     For example, you may want to display a detailed message when the notification is sent through email,
     and a more concise message in a push notification. Channel elements are only valid as top-level
     elements; you cannot nest channel elements. If there is a channel element specified at the top-level
     of the document, all sibling elements must be channel elements.
     Note: As an alternative, most elements support a `channel` property. Which allows you to selectively
     display an individual element on a per channel basis. See the
     [control flow docs](https://www.courier.com/docs/platform/content/elemental/control-flow/) for more details.
     """
 
-    channel: str = pydantic.Field(
-        description=(
-            "The channel the contents of this element should be applied to. Can be `email`,\n"
-            "`push`, `direct_message`, `sms` or a provider such as slack\n"
-        )
-    )
-    elements: typing.Optional[typing.List[ElementalNode]] = pydantic.Field(
-        description=(
-            "An array of elements to apply to the channel. If `raw` has not been\n"
-            "specified, `elements` is `required`.\n"
-        )
-    )
-    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description=(
-            "Raw data to apply to the channel. If `elements` has not been\n" "specified, `raw` is `required`.\n"
-        )
-    )
+    channel: str = pydantic_v1.Field()
+    """
+    The channel the contents of this element should be applied to. Can be `email`,
+    `push`, `direct_message`, `sms` or a provider such as slack
+    """
+
+    elements: typing.Optional[typing.List[ElementalNode]] = pydantic_v1.Field(default=None)
+    """
+    An array of elements to apply to the channel. If `raw` has not been
+    specified, `elements` is `required`.
+    """
+
+    raw: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    Raw data to apply to the channel. If `elements` has not been
+    specified, `raw` is `required`.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
 
 
 from .elemental_node import ElementalNode  # noqa: E402
 
 ElementalChannelNode.update_forward_refs()
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content.py` & `trycourier-6.0.1/src/courier/commons/types/base_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .elemental_node import ElementalNode
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ElementalContent(pydantic.BaseModel):
-    version: str = pydantic.Field(description='For example, "2022-01-01"')
-    brand: typing.Optional[typing.Any]
-    elements: typing.List[ElementalNode]
+class BaseError(pydantic_v1.BaseModel):
+    message: str = pydantic_v1.Field()
+    """
+    A message describing the error that occurred.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_content_sugar.py` & `trycourier-6.0.1/src/courier/templates/types/routing_strategy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .channel_identifier import ChannelIdentifier
+from .routing_strategy_method import RoutingStrategyMethod
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ElementalContentSugar(pydantic.BaseModel):
+class RoutingStrategy(pydantic_v1.BaseModel):
+    method: RoutingStrategyMethod = pydantic_v1.Field()
     """
-    Syntatic Sugar to provide a fast shorthand for Courier Elemental Blocks.
+    The method for selecting channels to send the message with. Value can be either 'single' or 'all'. If not provided will default to 'single'
     """
 
-    title: str = pydantic.Field(
-        description="The title to be displayed by supported channels i.e. push, email (as subject)"
-    )
-    body: str = pydantic.Field(description="The text content displayed in the notification.")
+    channels: typing.List[ChannelIdentifier] = pydantic_v1.Field()
+    """
+    An array of valid channel identifiers (like email, push, sms, etc.) and additional routing nodes.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_divider_node.py` & `trycourier-6.0.1/src/courier/send/types/elemental_divider_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class ElementalDividerNode(ElementalBaseNode):
     """
     Renders a dividing line between elements.
     """
 
-    color: typing.Optional[str] = pydantic.Field(
-        description="The CSS color to render the line with. For example, `#fff`"
-    )
+    color: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The CSS color to render the line with. For example, `#fff`
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_group_node.py` & `trycourier-6.0.1/src/courier/send/types/elemental_image_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .elemental_base_node import ElementalBaseNode
+from .i_alignment import IAlignment
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ElementalImageNode(ElementalBaseNode):
+    """
+    Used to embed an image into the notification.
+    """
 
-class ElementalGroupNode(ElementalBaseNode):
+    src: str = pydantic_v1.Field()
     """
-    Allows you to group elements together. This can be useful when used in combination with "if" or "loop". See [control flow docs](https://www.courier.com/docs/platform/content/elemental/control-flow/) for more details.
+    The source of the image.
     """
 
-    elements: typing.List[ElementalNode] = pydantic.Field(description="Sub elements to render.")
+    href: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A URL to link to when the image is clicked.
+    """
+
+    align: typing.Optional[IAlignment] = pydantic_v1.Field(default=None)
+    """
+    The alignment of the image.
+    """
+
+    alt_text: typing.Optional[str] = pydantic_v1.Field(alias="altText", default=None)
+    """
+    Alternate text for the image.
+    """
+
+    width: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    CSS width properties to apply to the image. For example, 50px
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .elemental_node import ElementalNode  # noqa: E402
-
-ElementalGroupNode.update_forward_refs()
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_image_node.py` & `trycourier-6.0.1/src/courier/send/types/elemental_quote_node.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 from .i_alignment import IAlignment
+from .locales import Locales
+from .text_style import TextStyle
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ElementalQuoteNode(ElementalBaseNode):
+    """
+    Renders a quote block.
+    """
+
+    content: str = pydantic_v1.Field()
+    """
+    The text value of the quote.
+    """
 
-class ElementalImageNode(ElementalBaseNode):
+    align: typing.Optional[IAlignment] = pydantic_v1.Field(default=None)
     """
-    Used to embed an image into the notification.
+    Alignment of the quote.
     """
 
-    src: str = pydantic.Field(description="The source of the image.")
-    href: typing.Optional[str] = pydantic.Field(description="A URL to link to when the image is clicked.")
-    align: typing.Optional[IAlignment] = pydantic.Field(description="The alignment of the image.")
-    alt_text: typing.Optional[str] = pydantic.Field(alias="altText", description="Alternate text for the image.")
-    width: typing.Optional[str] = pydantic.Field(
-        description="CSS width properties to apply to the image. For example, 50px"
-    )
+    border_color: typing.Optional[str] = pydantic_v1.Field(alias="borderColor", default=None)
+    """
+    CSS border color property. For example, `#fff`
+    """
+
+    text_style: TextStyle
+    locales: Locales = pydantic_v1.Field()
+    """
+    Region specific content. See [locales docs](https://www.courier.com/docs/platform/content/elemental/locales/) for more details.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_meta_node.py` & `trycourier-6.0.1/src/courier/send/types/elemental_meta_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class ElementalMetaNode(ElementalBaseNode):
     """
     The meta element contains information describing the notification that may
     be used by a particular channel or provider. One important field is the title
     field which will be used as the title for channels that support it.
     """
 
-    title: typing.Optional[str] = pydantic.Field(
-        description="The title to be displayed by supported channels. For example, the email subject."
-    )
+    title: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The title to be displayed by supported channels. For example, the email subject.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/elemental_text_node.py` & `trycourier-6.0.1/src/courier/send/types/elemental_text_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,81 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
-
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .elemental_base_node import ElementalBaseNode
 from .locales import Locales
 from .text_align import TextAlign
 from .text_style import TextStyle
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class ElementalTextNode(ElementalBaseNode):
     """
     Represents a body of text to be rendered inside of the notification.
     """
 
-    content: str = pydantic.Field(
-        description=(
-            "The text content displayed in the notification. Either this\n"
-            "field must be specified, or the elements field\n"
-        )
-    )
-    align: TextAlign = pydantic.Field(description="Text alignment.")
-    text_style: typing.Optional[TextStyle] = pydantic.Field(
-        description="Allows the text to be rendered as a heading level."
-    )
-    color: typing.Optional[str] = pydantic.Field(
-        description="Specifies the color of text. Can be any valid css color value"
-    )
-    bold: typing.Optional[str] = pydantic.Field(description="Apply bold to the text")
-    italic: typing.Optional[str] = pydantic.Field(description="Apply italics to the text")
-    strikethrough: typing.Optional[str] = pydantic.Field(description="Apply a strike through the text")
-    underline: typing.Optional[str] = pydantic.Field(description="Apply an underline to the text")
-    locales: typing.Optional[Locales] = pydantic.Field(
-        description="Region specific content. See [locales docs](https://www.courier.com/docs/platform/content/elemental/locales/) for more details."
-    )
-    format: typing.Optional[typing_extensions.Literal["markdown"]]
+    content: str = pydantic_v1.Field()
+    """
+    The text content displayed in the notification. Either this
+    field must be specified, or the elements field
+    """
+
+    align: TextAlign = pydantic_v1.Field()
+    """
+    Text alignment.
+    """
+
+    text_style: typing.Optional[TextStyle] = pydantic_v1.Field(default=None)
+    """
+    Allows the text to be rendered as a heading level.
+    """
+
+    color: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Specifies the color of text. Can be any valid css color value
+    """
+
+    bold: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Apply bold to the text
+    """
+
+    italic: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Apply italics to the text
+    """
+
+    strikethrough: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Apply a strike through the text
+    """
+
+    underline: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Apply an underline to the text
+    """
+
+    locales: typing.Optional[Locales] = pydantic_v1.Field(default=None)
+    """
+    Region specific content. See [locales docs](https://www.courier.com/docs/platform/content/elemental/locales/) for more details.
+    """
+
+    format: typing.Optional[typing.Literal["markdown"]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/email_footer.py` & `trycourier-6.0.1/src/courier/users/preferences/types/topic_preference_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ....commons.types.channel_classification import ChannelClassification
+from ....commons.types.preference_status import PreferenceStatus
 from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class TopicPreferenceUpdate(pydantic_v1.BaseModel):
+    status: PreferenceStatus
+    custom_routing: typing.Optional[typing.List[ChannelClassification]] = pydantic_v1.Field(default=None)
+    """
+    The Channels a user has chosen to receive notifications through for this topic
+    """
 
-class EmailFooter(pydantic.BaseModel):
-    content: typing.Optional[typing.Any]
-    inherit_default: typing.Optional[bool] = pydantic.Field(alias="inheritDefault")
+    has_custom_routing: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/email_head.py` & `trycourier-6.0.1/src/courier/users/tenants/types/add_user_to_single_tenants_params_profile.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class EmailHead(pydantic.BaseModel):
-    inherit_default: bool = pydantic.Field(alias="inheritDefault")
-    content: typing.Optional[str]
+class AddUserToSingleTenantsParamsProfile(pydantic_v1.BaseModel):
+    title: str
+    email: str = pydantic_v1.Field()
+    """
+    Email Address
+    """
+
+    phone_number: str = pydantic_v1.Field()
+    """
+    A valid phone number
+    """
+
+    locale: str = pydantic_v1.Field()
+    """
+    The user's preferred ISO 639-1 language code.
+    """
+
+    additional_fields: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    """
+    Additional provider specific fields may be specified.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/email_header.py` & `trycourier-6.0.1/src/courier/send/types/message_providers_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .logo import Logo
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .metadata import Metadata
+
+
+class MessageProvidersType(pydantic_v1.BaseModel):
+    override: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    Provider specific overrides.
+    """
+
+    if_: typing.Optional[str] = pydantic_v1.Field(alias="if", default=None)
+    """
+    A JavaScript conditional expression to determine if the message should be sent
+    through the channel. Has access to the data and profile object. For example,
+    `data.name === profile.name`
+    """
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class EmailHeader(pydantic.BaseModel):
-    inherit_default: typing.Optional[bool] = pydantic.Field(alias="inheritDefault")
-    bar_color: typing.Optional[str] = pydantic.Field(alias="barColor")
-    logo: Logo
+    timeouts: typing.Optional[int] = None
+    metadata: typing.Optional[Metadata] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/expiry.py` & `trycourier-6.0.1/src/courier/send/types/expiry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .expires_in_type import ExpiresInType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Expiry(pydantic.BaseModel):
-    expires_at: typing.Optional[str] = pydantic.Field(
-        description="An epoch timestamp or ISO8601 timestamp with timezone `(YYYY-MM-DDThh:mm:ss.sTZD)` that describes the time in which a message expires."
-    )
-    expires_in: ExpiresInType = pydantic.Field(
-        description="A duration in the form of milliseconds or an ISO8601 Duration format (i.e. P1DT4H)."
-    )
+class Expiry(pydantic_v1.BaseModel):
+    expires_at: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    An epoch timestamp or ISO8601 timestamp with timezone `(YYYY-MM-DDThh:mm:ss.sTZD)` that describes the time in which a message expires.
+    """
+
+    expires_in: ExpiresInType = pydantic_v1.Field()
+    """
+    A duration in the form of milliseconds or an ISO8601 Duration format (i.e. P1DT4H).
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/i_profile_preferences.py` & `trycourier-6.0.1/src/courier/audit_events/types/actor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .i_preferences import IPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class IProfilePreferences(pydantic.BaseModel):
-    categories: typing.Optional[IPreferences]
-    notifications: IPreferences
-    template_id: typing.Optional[str] = pydantic.Field(alias="templateId")
+class Actor(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    email: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/icons.py` & `trycourier-6.0.1/src/courier/bulk/types/inbound_bulk_message_user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from ...send.types.user_recipient import UserRecipient
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Icons(pydantic.BaseModel):
-    bell: typing.Optional[str]
-    message: typing.Optional[str]
+class InboundBulkMessageUser(pydantic_v1.BaseModel):
+    preferences: typing.Optional[RecipientPreferences] = None
+    profile: typing.Optional[typing.Any] = None
+    recipient: typing.Optional[str] = None
+    data: typing.Optional[typing.Any] = None
+    to: typing.Optional[UserRecipient] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_pattern_recipient.py` & `trycourier-6.0.1/src/courier/send/types/elemental_content.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .elemental_node import ElementalNode
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ElementalContent(pydantic_v1.BaseModel):
+    version: str = pydantic_v1.Field()
+    """
+    For example, "2022-01-01"
+    """
 
-class InvalidListPatternRecipient(pydantic.BaseModel):
-    user_id: str
-    list_id: str
+    brand: typing.Optional[typing.Any] = None
+    elements: typing.List[ElementalNode]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/invalid_list_recipient.py` & `trycourier-6.0.1/src/courier/bulk/types/job_details.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .bulk_job_status import BulkJobStatus
+from .inbound_bulk_message import InboundBulkMessage
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InvalidListRecipient(pydantic.BaseModel):
-    user_id: str
-    list_pattern: str
+class JobDetails(pydantic_v1.BaseModel):
+    definition: InboundBulkMessage
+    enqueued: int
+    failures: int
+    received: int
+    status: BulkJobStatus
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/invalid_user_recipient.py` & `trycourier-6.0.1/src/courier/commons/types/channel_preference.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .channel_classification import ChannelClassification
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InvalidUserRecipient(pydantic.BaseModel):
-    list_id: str
-    list_pattern: str
+class ChannelPreference(pydantic_v1.BaseModel):
+    channel: ChannelClassification
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/list_filter.py` & `trycourier-6.0.1/src/courier/profiles/types/address.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-from ....core.datetime_utils import serialize_datetime
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ListFilter(pydantic.BaseModel):
-    operator: typing_extensions.Literal["MEMBER_OF"] = pydantic.Field(
-        description="Send to users only if they are member of the account"
-    )
-    path: typing_extensions.Literal["account_id"]
-    value: str
+class Address(pydantic_v1.BaseModel):
+    formatted: str
+    street_address: str
+    locality: str
+    region: str
+    postal_code: str
+    country: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient.py` & `trycourier-6.0.1/src/courier/send/types/list_pattern_recipient.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .list_pattern_recipient_type import ListPatternRecipientType
 from .message_data import MessageData
 
 
 class ListPatternRecipient(ListPatternRecipientType):
-    list_pattern: typing.Optional[str]
-    data: typing.Optional[MessageData]
+    list_pattern: typing.Optional[str] = None
+    data: typing.Optional[MessageData] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/list_pattern_recipient_type.py` & `trycourier-6.0.1/src/courier/send/types/delay.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class Delay(pydantic_v1.BaseModel):
+    duration: int = pydantic_v1.Field()
+    """
+    The duration of the delay in milliseconds.
+    """
 
-class ListPatternRecipientType(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_message_user_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .list_filter import ListFilter
-from .list_recipient_type import ListRecipientType
-from .message_data import MessageData
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .bulk_job_user_status import BulkJobUserStatus
+from .inbound_bulk_message_user import InboundBulkMessageUser
 
 
-class ListRecipient(ListRecipientType):
-    list_id: typing.Optional[str]
-    data: typing.Optional[MessageData]
-    filters: typing.Optional[typing.List[ListFilter]]
+class BulkMessageUserResponse(InboundBulkMessageUser):
+    status: BulkJobUserStatus
+    message_id: typing.Optional[str] = pydantic_v1.Field(alias="messageId", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/list_recipient_type.py` & `trycourier-6.0.1/src/courier/tenants/types/subscription_topic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .subscription_topic_status import SubscriptionTopicStatus
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class SubscriptionTopic(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
+    """
+    Topic ID
+    """
+
+    status: SubscriptionTopicStatus
 
-class ListRecipientType(pydantic.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/locale.py` & `trycourier-6.0.1/src/courier/send/types/list_recipient.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .list_filter import ListFilter
+from .list_recipient_type import ListRecipientType
+from .message_data import MessageData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Locale(pydantic.BaseModel):
-    content: str
+class ListRecipient(ListRecipientType):
+    list_id: typing.Optional[str] = None
+    data: typing.Optional[MessageData] = None
+    filters: typing.Optional[typing.List[ListFilter]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/logo.py` & `trycourier-6.0.1/src/courier/users/tokens/types/patch_operation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Logo(pydantic.BaseModel):
-    href: typing.Optional[str]
-    image: typing.Optional[str]
+class PatchOperation(pydantic_v1.BaseModel):
+    op: str = pydantic_v1.Field()
+    """
+    The operation to perform.
+    """
+
+    path: str = pydantic_v1.Field()
+    """
+    The JSON path specifying the part of the profile to operate on.
+    """
+
+    value: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The value for the operation.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/message_channel_email_override.py` & `trycourier-6.0.1/src/courier/send/types/message_channel_email_override.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...brands.types.brand import Brand
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .attachment import Attachment
 from .tracking_override import TrackingOverride
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class MessageChannelEmailOverride(pydantic.BaseModel):
-    attachments: typing.Optional[typing.List[Attachment]]
-    bcc: typing.Optional[str]
-    brand: typing.Optional[Brand]
-    cc: typing.Optional[str]
-    from_: typing.Optional[str] = pydantic.Field(alias="from")
-    html: typing.Optional[str]
-    reply_to: typing.Optional[str]
-    subject: typing.Optional[str]
-    text: typing.Optional[str]
+
+class MessageChannelEmailOverride(pydantic_v1.BaseModel):
+    attachments: typing.Optional[typing.List[Attachment]] = None
+    bcc: typing.Optional[str] = None
+    brand: typing.Optional[Brand] = None
+    cc: typing.Optional[str] = None
+    from_: typing.Optional[str] = pydantic_v1.Field(alias="from", default=None)
+    html: typing.Optional[str] = None
+    reply_to: typing.Optional[str] = None
+    subject: typing.Optional[str] = None
+    text: typing.Optional[str] = None
     tracking: TrackingOverride
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/message_context.py` & `trycourier-6.0.1/src/courier/profiles/types/profile_get_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class MessageContext(pydantic.BaseModel):
-    tenant_id: typing.Optional[str] = pydantic.Field(
-        description=(
-            "An id of a tenant, see [tenants api docs](https://www.courier.com/docs/reference/tenants/).\n"
-            "Will load brand, default preferences and any other base context data associated with this tenant.\n"
-        )
-    )
+class ProfileGetResponse(pydantic_v1.BaseModel):
+    profile: typing.Dict[str, typing.Any]
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/message_metadata.py` & `trycourier-6.0.1/src/courier/send/types/message_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .utm import Utm
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class MessageMetadata(pydantic.BaseModel):
-    event: typing.Optional[str] = pydantic.Field(
-        description="An arbitrary string to tracks the event that generated this request (e.g. 'signup')."
-    )
-    tags: typing.Optional[typing.List[str]] = pydantic.Field(
-        description="An array of up to 9 tags you wish to associate with this request (and corresponding messages) for later analysis. Individual tags cannot be more than 30 characters in length."
-    )
-    utm: typing.Optional[Utm] = pydantic.Field(
-        description="Identify the campaign that refers traffic to a specific website, and attributes the browser's website session."
-    )
-    trace_id: typing.Optional[str] = pydantic.Field(
-        description="A unique ID used to correlate this request to processing on your servers. Note: Courier does not verify the uniqueness of this ID."
-    )
+
+class MessageMetadata(pydantic_v1.BaseModel):
+    event: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    An arbitrary string to tracks the event that generated this request (e.g. 'signup').
+    """
+
+    tags: typing.Optional[typing.List[str]] = pydantic_v1.Field(default=None)
+    """
+    An array of up to 9 tags you wish to associate with this request (and corresponding messages) for later analysis. Individual tags cannot be more than 30 characters in length.
+    """
+
+    utm: typing.Optional[Utm] = pydantic_v1.Field(default=None)
+    """
+    Identify the campaign that refers traffic to a specific website, and attributes the browser's website session.
+    """
+
+    trace_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A unique ID used to correlate this request to processing on your servers. Note: Courier does not verify the uniqueness of this ID.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/message_providers_type.py` & `trycourier-6.0.1/src/courier/automations/types/automation_fetch_data_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .metadata import Metadata
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class MessageProvidersType(pydantic.BaseModel):
-    override: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(description="Provider specific overrides.")
-    if_: typing.Optional[str] = pydantic.Field(
-        alias="if",
-        description=(
-            "A JavaScript conditional expression to determine if the message should be sent\n"
-            "through the channel. Has access to the data and profile object. For example,\n"
-            "`data.name === profile.name`\n"
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_fetch_data_webhook import AutomationFetchDataWebhook
+from .automation_step import AutomationStep
+from .merge_algorithm import MergeAlgorithm
+
+
+class AutomationFetchDataStep(AutomationStep):
+    """
+    from courier import AutomationFetchDataStep, AutomationFetchDataWebhook
+
+    AutomationFetchDataStep(
+        action="fetch-data",
+        merge_strategy="none",
+        webhook=AutomationFetchDataWebhook(
+            body={"foo": "bar"},
+            params={"hello": "world"},
+            headers={"content-type": "application/json"},
+            method="POST",
+            url="https://bryan-at-courier.free.beeceptor.com",
         ),
     )
-    timeouts: typing.Optional[int]
-    metadata: typing.Optional[Metadata]
+    """
+
+    action: typing.Literal["fetch-data"]
+    webhook: AutomationFetchDataWebhook
+    merge_strategy: MergeAlgorithm
+    idempotency_expiry: typing.Optional[str] = None
+    idempotency_key: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/metadata.py` & `trycourier-6.0.1/src/courier/users/tokens/types/put_user_tokens_opts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from .utm import Utm
+from ....core.pydantic_utilities import pydantic_v1
+from .user_token import UserToken
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Metadata(pydantic.BaseModel):
-    utm: typing.Optional[Utm]
+class PutUserTokensOpts(pydantic_v1.BaseModel):
+    user_id: str
+    tokens: typing.List[UserToken]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/preference.py` & `trycourier-6.0.1/src/courier/send/types/preference.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
 from ...commons.types.channel_preference import ChannelPreference
 from ...commons.types.preference_status import PreferenceStatus
 from ...commons.types.rule import Rule
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .channel_source import ChannelSource
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Preference(pydantic.BaseModel):
+class Preference(pydantic_v1.BaseModel):
     status: PreferenceStatus
-    rules: typing.Optional[typing.List[Rule]]
-    channel_preferences: typing.Optional[typing.List[ChannelPreference]]
-    source: typing.Optional[ChannelSource]
+    rules: typing.Optional[typing.List[Rule]] = None
+    channel_preferences: typing.Optional[typing.List[ChannelPreference]] = None
+    source: typing.Optional[ChannelSource] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/preferences.py` & `trycourier-6.0.1/src/courier/brands/types/brand_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...commons.types.email import Email
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .brand_colors import BrandColors
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Preferences(pydantic.BaseModel):
-    template_ids: typing.List[str] = pydantic.Field(alias="templateIds")
+class BrandSettings(pydantic_v1.BaseModel):
+    colors: typing.Optional[BrandColors] = None
+    inapp: typing.Optional[typing.Any] = None
+    email: typing.Optional[Email] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/routing.py` & `trycourier-6.0.1/src/courier/send/types/routing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .routing_channel import RoutingChannel
 from .routing_method import RoutingMethod
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Routing(pydantic.BaseModel):
+class Routing(pydantic_v1.BaseModel):
     """
     Allows you to customize which channel(s) Courier will potentially deliver the message.
     If no routing key is specified, Courier will use the default routing configuration or
     routing defined by the template.
     """
 
     method: RoutingMethod
-    channels: typing.List[RoutingChannel] = pydantic.Field(
-        description=(
-            "A list of channels or providers to send the message through. Can also recursively define\n"
-            "sub-routing methods, which can be useful for defining advanced push notification\n"
-            "delivery strategies.\n"
-        )
-    )
+    channels: typing.List[RoutingChannel] = pydantic_v1.Field()
+    """
+    A list of channels or providers to send the message through. Can also recursively define
+    sub-routing methods, which can be useful for defining advanced push notification
+    delivery strategies.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/routing_strategy_provider.py` & `trycourier-6.0.1/src/courier/send/types/i_profile_preferences.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .metadata import Metadata
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .i_preferences import IPreferences
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RoutingStrategyProvider(pydantic.BaseModel):
-    name: str
-    config: typing.Optional[typing.Dict[str, typing.Any]]
-    if_: typing.Optional[str] = pydantic.Field(alias="if")
-    metadata: Metadata
+class IProfilePreferences(pydantic_v1.BaseModel):
+    categories: typing.Optional[IPreferences] = None
+    notifications: IPreferences
+    template_id: typing.Optional[str] = pydantic_v1.Field(alias="templateId", default=None)
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/template_message.py` & `trycourier-6.0.1/src/courier/send/types/base_message_send_to.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .base_message import BaseMessage
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .message_recipient import MessageRecipient
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TemplateMessage(BaseMessage):
-    template: str = pydantic.Field(
-        description=(
-            "The id of the notification template to be rendered and sent to the recipient(s).\n"
-            "This field or the content field must be supplied.\n"
-        )
-    )
-    to: MessageRecipient = pydantic.Field(description="The recipient or a list of recipients of the message")
+class BaseMessageSendTo(pydantic_v1.BaseModel):
+    to: typing.Optional[MessageRecipient] = pydantic_v1.Field(default=None)
+    """
+    The recipient or a list of recipients of the message
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/timeout.py` & `trycourier-6.0.1/src/courier/lists/types/list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .criteria import Criteria
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Timeout(pydantic.BaseModel):
-    provider: typing.Optional[typing.Dict[str, int]]
-    channel: typing.Optional[typing.Dict[str, int]]
-    message: typing.Optional[int]
-    escalation: typing.Optional[int]
-    criteria: typing.Optional[Criteria]
+class List(pydantic_v1.BaseModel):
+    id: str
+    name: str
+    created: typing.Optional[int] = None
+    updated: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/timeouts.py` & `trycourier-6.0.1/src/courier/audiences/types/single_filter_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Timeouts(pydantic.BaseModel):
-    provider: typing.Optional[int]
-    channel: typing.Optional[int]
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .base_filter_config import BaseFilterConfig
+
+
+class SingleFilterConfig(BaseFilterConfig):
+    """
+    A single filter to use for filtering
+    """
+
+    value: str = pydantic_v1.Field()
+    """
+    The value to use for filtering
+    """
+
+    path: str = pydantic_v1.Field()
+    """
+    The attribe name from profile whose value will be operated against the filter value
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/tracking_override.py` & `trycourier-6.0.1/src/courier/profiles/types/snooze_rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .snooze_rule_type import SnoozeRuleType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TrackingOverride(pydantic.BaseModel):
-    open: bool
+class SnoozeRule(pydantic_v1.BaseModel):
+    type: SnoozeRuleType
+    start: str
+    until: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient.py` & `trycourier-6.0.1/src/courier/send/types/user_recipient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .i_profile_preferences import IProfilePreferences
 from .message_context import MessageContext
 from .message_data import MessageData
 from .user_recipient_type import UserRecipientType
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class UserRecipient(UserRecipientType):
-    account_id: typing.Optional[str] = pydantic.Field(description="Use `tenant_id` instad.")
-    context: typing.Optional[MessageContext] = pydantic.Field(
-        description="Context information such as tenant_id to send the notification with."
-    )
-    data: typing.Optional[MessageData]
-    email: typing.Optional[str]
-    locale: typing.Optional[str] = pydantic.Field(description="The user's preferred ISO 639-1 language code.")
-    user_id: typing.Optional[str]
-    phone_number: typing.Optional[str]
-    preferences: typing.Optional[IProfilePreferences]
-    tenant_id: typing.Optional[str] = pydantic.Field(
-        description=(
-            "An id of a tenant, [see tenants api docs](https://www.courier.com/docs/reference/tenants).\n"
-            "Will load brand, default preferences and any other base context data associated with this tenant.\n"
-        )
-    )
+    account_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Use `tenant_id` instad.
+    """
+
+    context: typing.Optional[MessageContext] = pydantic_v1.Field(default=None)
+    """
+    Context information such as tenant_id to send the notification with.
+    """
+
+    data: typing.Optional[MessageData] = None
+    email: typing.Optional[str] = None
+    locale: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The user's preferred ISO 639-1 language code.
+    """
+
+    user_id: typing.Optional[str] = None
+    phone_number: typing.Optional[str] = None
+    preferences: typing.Optional[IProfilePreferences] = None
+    tenant_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    An id of a tenant, [see tenants api docs](https://www.courier.com/docs/reference/tenants).
+    Will load brand, default preferences and any other base context data associated with this tenant.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/user_recipient_type.py` & `trycourier-6.0.1/src/courier/send/types/list_pattern_recipient_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UserRecipientType(pydantic.BaseModel):
+class ListPatternRecipientType(pydantic_v1.BaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/utm.py` & `trycourier-6.0.1/src/courier/automations/types/automation_send_step.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_step import AutomationStep
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Utm(pydantic.BaseModel):
-    source: typing.Optional[str]
-    medium: typing.Optional[str]
-    campaign: typing.Optional[str]
-    term: typing.Optional[str]
-    content: typing.Optional[str]
+class AutomationSendStep(AutomationStep):
+    action: typing.Literal["send"]
+    brand: typing.Optional[str] = None
+    data: typing.Optional[typing.Dict[str, typing.Any]] = None
+    override: typing.Optional[typing.Dict[str, typing.Any]] = None
+    profile: typing.Optional[typing.Any] = None
+    recipient: typing.Optional[str] = None
+    template: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/send/types/widget_background.py` & `trycourier-6.0.1/src/courier/automations/types/automation_invoke_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class WidgetBackground(pydantic.BaseModel):
-    top_color: typing.Optional[str] = pydantic.Field(alias="topColor")
-    bottom_color: typing.Optional[str] = pydantic.Field(alias="bottomColor")
+class AutomationInvokeResponse(pydantic_v1.BaseModel):
+    run_id: str = pydantic_v1.Field(alias="runId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/templates/types/__init__.py` & `trycourier-6.0.1/src/courier/templates/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/templates/types/list_templates_response.py` & `trycourier-6.0.1/src/courier/profiles/types/subscribe_to_lists_request_list_object.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ...commons.types.paging import Paging
-from .notification_templates import NotificationTemplates
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
 
-class ListTemplatesResponse(pydantic.BaseModel):
-    paging: Paging
-    results: typing.List[NotificationTemplates] = pydantic.Field(description="An array of Notification Templates")
+class SubscribeToListsRequestListObject(pydantic_v1.BaseModel):
+    list_id: str = pydantic_v1.Field(alias="listId")
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/templates/types/notification_templates.py` & `trycourier-6.0.1/src/courier/templates/types/notification_templates.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .routing_strategy import RoutingStrategy
 from .tag import Tag
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class NotificationTemplates(pydantic.BaseModel):
-    created_at: int = pydantic.Field(
-        description="A UTC timestamp at which notification was created. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970)."
-    )
-    id: str = pydantic.Field(description="A unique identifier associated with the notification.")
-    routing: RoutingStrategy = pydantic.Field(description="Routing strategy used by this notification.")
-    tags: typing.List[Tag] = pydantic.Field(description="A list of tags attached to the notification.")
-    title: str = pydantic.Field(description="The title of the notification.")
-    updated_at: int = pydantic.Field(
-        description="A UTC timestamp at which notification was updated. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970)."
-    )
+
+class NotificationTemplates(pydantic_v1.BaseModel):
+    created_at: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which notification was created. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970).
+    """
+
+    id: str = pydantic_v1.Field()
+    """
+    A unique identifier associated with the notification.
+    """
+
+    routing: RoutingStrategy = pydantic_v1.Field()
+    """
+    Routing strategy used by this notification.
+    """
+
+    tags: typing.List[Tag] = pydantic_v1.Field()
+    """
+    A list of tags attached to the notification.
+    """
+
+    title: str = pydantic_v1.Field()
+    """
+    The title of the notification.
+    """
+
+    updated_at: int = pydantic_v1.Field()
+    """
+    A UTC timestamp at which notification was updated. This is stored as a millisecond representation of the Unix epoch (the time passed since January 1, 1970).
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/templates/types/routing_strategy.py` & `trycourier-6.0.1/src/courier/tenants/types/tenant_list_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,55 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .channel_identifier import ChannelIdentifier
-from .routing_strategy_method import RoutingStrategyMethod
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class RoutingStrategy(pydantic.BaseModel):
-    method: RoutingStrategyMethod = pydantic.Field(
-        description="The method for selecting channels to send the message with. Value can be either 'single' or 'all'. If not provided will default to 'single'"
-    )
-    channels: typing.List[ChannelIdentifier] = pydantic.Field(
-        description="An array of valid channel identifiers (like email, push, sms, etc.) and additional routing nodes."
-    )
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .tenant import Tenant
+
+
+class TenantListResponse(pydantic_v1.BaseModel):
+    cursor: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A pointer to the next page of results. Defined only when has_more is set to true.
+    """
+
+    has_more: bool = pydantic_v1.Field()
+    """
+    Set to true when there are more pages that can be retrieved.
+    """
+
+    items: typing.List[Tenant] = pydantic_v1.Field()
+    """
+    An array of Tenants
+    """
+
+    next_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    A url that may be used to generate fetch the next set of results.
+    Defined only when has_more is set to true
+    """
+
+    url: str = pydantic_v1.Field()
+    """
+    A url that may be used to generate these results.
+    """
+
+    type: typing.Literal["list"] = pydantic_v1.Field()
+    """
+    Always set to "list". Represents the type of this object.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/templates/types/tag.py` & `trycourier-6.0.1/src/courier/notifications/types/notification_content_hierarchy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .tag_data import TagData
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Tag(pydantic.BaseModel):
-    data: typing.List[TagData]
+class NotificationContentHierarchy(pydantic_v1.BaseModel):
+    parent: typing.Optional[str] = None
+    children: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/templates/types/tag_data.py` & `trycourier-6.0.1/src/courier/audit_events/types/get_audit_event_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TagData(pydantic.BaseModel):
-    id: str = pydantic.Field(description="A unique identifier of the tag.")
-    name: str = pydantic.Field(description="Name of the tag.")
+class GetAuditEventParams(pydantic_v1.BaseModel):
+    audit_event_id: str = pydantic_v1.Field(alias="auditEventId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/tenants/types/__init__.py` & `trycourier-6.0.1/src/courier/tenants/types/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/tenants/types/default_preferences.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_ms_teams_channel_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .subscription_topic import SubscriptionTopic
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .ms_teams_base_properties import MsTeamsBaseProperties
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DefaultPreferences(pydantic.BaseModel):
-    items: typing.List[SubscriptionTopic]
+class SendToMsTeamsChannelId(MsTeamsBaseProperties):
+    channel_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/tenants/types/subscription_topic.py` & `trycourier-6.0.1/src/courier/send/types/icons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from .subscription_topic_status import SubscriptionTopicStatus
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SubscriptionTopic(pydantic.BaseModel):
-    id: str = pydantic.Field(description="Topic ID")
-    status: SubscriptionTopicStatus
+class Icons(pydantic_v1.BaseModel):
+    bell: typing.Optional[str] = None
+    message: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/__init__.py` & `trycourier-6.0.1/src/courier/users/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .resources import (
-    AddUserToSingleTenantsParamsProfile,
+from . import preferences, tenants, tokens
+from .preferences import (
+    TopicPreference,
+    TopicPreferenceUpdate,
+    UserPreferencesGetResponse,
+    UserPreferencesListResponse,
+    UserPreferencesUpdateResponse,
+)
+from .tenants import AddUserToSingleTenantsParamsProfile, ListTenantsForUserResponse
+from .tokens import (
     DeleteUserTokenOpts,
     Device,
     ExpiryDate,
     GetAllTokensResponse,
     GetUserTokenOpts,
     GetUserTokenResponse,
     GetUserTokensOpts,
-    ListTenantsForUserResponse,
     PatchOp,
     PatchOperation,
     PatchUserTokenOpts,
     ProviderKey,
     PutUserTokenOpts,
     PutUserTokensOpts,
     TokenStatus,
-    TopicPreference,
     Tracking,
-    UserPreferencesGetResponse,
-    UserPreferencesListResponse,
-    UserPreferencesUpdateResponse,
     UserToken,
-    preferences,
-    tenants,
-    tokens,
 )
 
 __all__ = [
     "AddUserToSingleTenantsParamsProfile",
     "DeleteUserTokenOpts",
     "Device",
     "ExpiryDate",
@@ -42,14 +42,15 @@
     "PatchOperation",
     "PatchUserTokenOpts",
     "ProviderKey",
     "PutUserTokenOpts",
     "PutUserTokensOpts",
     "TokenStatus",
     "TopicPreference",
+    "TopicPreferenceUpdate",
     "Tracking",
     "UserPreferencesGetResponse",
     "UserPreferencesListResponse",
     "UserPreferencesUpdateResponse",
     "UserToken",
     "preferences",
     "tenants",
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/client.py` & `trycourier-6.0.1/src/courier/users/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from .resources.preferences.client import AsyncPreferencesClient, PreferencesClient
-from .resources.tenants.client import AsyncTenantsClient, TenantsClient
-from .resources.tokens.client import AsyncTokensClient, TokensClient
+from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from .preferences.client import AsyncPreferencesClient, PreferencesClient
+from .tenants.client import AsyncTenantsClient, TenantsClient
+from .tokens.client import AsyncTokensClient, TokensClient
 
 
 class UsersClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
         self.preferences = PreferencesClient(client_wrapper=self._client_wrapper)
         self.tenants = TenantsClient(client_wrapper=self._client_wrapper)
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/__init__.py` & `trycourier-6.0.1/src/courier/users/tokens/types/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from . import preferences, tenants, tokens
-from .preferences import (
-    TopicPreference,
-    UserPreferencesGetResponse,
-    UserPreferencesListResponse,
-    UserPreferencesUpdateResponse,
-)
-from .tenants import AddUserToSingleTenantsParamsProfile, ListTenantsForUserResponse
-from .tokens import (
-    DeleteUserTokenOpts,
-    Device,
-    ExpiryDate,
-    GetAllTokensResponse,
-    GetUserTokenOpts,
-    GetUserTokenResponse,
-    GetUserTokensOpts,
-    PatchOp,
-    PatchOperation,
-    PatchUserTokenOpts,
-    ProviderKey,
-    PutUserTokenOpts,
-    PutUserTokensOpts,
-    TokenStatus,
-    Tracking,
-    UserToken,
-)
+from .delete_user_token_opts import DeleteUserTokenOpts
+from .device import Device
+from .expiry_date import ExpiryDate
+from .get_all_tokens_response import GetAllTokensResponse
+from .get_user_token_opts import GetUserTokenOpts
+from .get_user_token_response import GetUserTokenResponse
+from .get_user_tokens_opts import GetUserTokensOpts
+from .patch_op import PatchOp
+from .patch_operation import PatchOperation
+from .patch_user_token_opts import PatchUserTokenOpts
+from .provider_key import ProviderKey
+from .put_user_token_opts import PutUserTokenOpts
+from .put_user_tokens_opts import PutUserTokensOpts
+from .token_status import TokenStatus
+from .tracking import Tracking
+from .user_token import UserToken
 
 __all__ = [
-    "AddUserToSingleTenantsParamsProfile",
     "DeleteUserTokenOpts",
     "Device",
     "ExpiryDate",
     "GetAllTokensResponse",
     "GetUserTokenOpts",
     "GetUserTokenResponse",
     "GetUserTokensOpts",
-    "ListTenantsForUserResponse",
     "PatchOp",
     "PatchOperation",
     "PatchUserTokenOpts",
     "ProviderKey",
     "PutUserTokenOpts",
     "PutUserTokensOpts",
     "TokenStatus",
-    "TopicPreference",
     "Tracking",
-    "UserPreferencesGetResponse",
-    "UserPreferencesListResponse",
-    "UserPreferencesUpdateResponse",
     "UserToken",
-    "preferences",
-    "tenants",
-    "tokens",
 ]
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_get_response.py` & `trycourier-6.0.1/src/courier/profiles/types/send_direct_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .topic_preference import TopicPreference
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UserPreferencesGetResponse(pydantic.BaseModel):
-    topic: TopicPreference
+class SendDirectMessage(pydantic_v1.BaseModel):
+    user_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_list_response.py` & `trycourier-6.0.1/src/courier/commons/types/recipient_preferences.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.paging import Paging
-from .topic_preference import TopicPreference
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .notification_preferences import NotificationPreferences
 
 
-class UserPreferencesListResponse(pydantic.BaseModel):
-    paging: Paging
-    items: typing.List[TopicPreference] = pydantic.Field(description="The Preferences associated with the user_id.")
+class RecipientPreferences(pydantic_v1.BaseModel):
+    categories: typing.Optional[NotificationPreferences] = None
+    notifications: typing.Optional[NotificationPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/preferences/types/user_preferences_update_response.py` & `trycourier-6.0.1/src/courier/automations/types/automation_add_to_digest_step.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class UserPreferencesUpdateResponse(pydantic.BaseModel):
-    message: str
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .automation_step import AutomationStep
+
+
+class AutomationAddToDigestStep(AutomationStep):
+    """
+    from courier import AutomationAddToDigestStep
+
+    AutomationAddToDigestStep(
+        action="add-to-digest",
+        subscription_topic_id="RAJE97CMT04KDJJ88ZDS2TP1690S",
+    )
+    """
+
+    action: typing.Literal["add-to-digest"]
+    subscription_topic_id: str = pydantic_v1.Field()
+    """
+    The subscription topic that has digests enabled
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tenants/client.py` & `trycourier-6.0.1/src/courier/audit_events/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,249 +1,234 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from .....core.api_error import ApiError
-from .....core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from .....core.jsonable_encoder import jsonable_encoder
-from .....core.remove_none_from_dict import remove_none_from_dict
-from ....commons.types.user_tenant_association import UserTenantAssociation
-from .types.add_user_to_single_tenants_params_profile import AddUserToSingleTenantsParamsProfile
-from .types.list_tenants_for_user_response import ListTenantsForUserResponse
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ..core.api_error import ApiError
+from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.remove_none_from_dict import remove_none_from_dict
+from ..core.request_options import RequestOptions
+from .types.audit_event import AuditEvent
+from .types.list_audit_events_response import ListAuditEventsResponse
 
-# this is used as the default value for optional parameters
-OMIT = typing.cast(typing.Any, ...)
 
-
-class TenantsClient:
+class AuditEventsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def add_multple(self, user_id: str, *, tenants: typing.List[UserTenantAssociation]) -> None:
+    def list(
+        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> ListAuditEventsResponse:
         """
-        This endpoint is used to add a user to
-        multiple tenants in one call.
-        A custom profile can also be supplied for each tenant.
-        This profile will be merged with the user's main
-        profile when sending to the user with that tenant.
+        Fetch the list of audit events
 
         Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audit events.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
 
-            - tenants: typing.List[UserTenantAssociation].
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        client.audit_events.list(
+            cursor="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants"),
-            json=jsonable_encoder({"tenants": tenants}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(ListAuditEventsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def add(self, user_id: str, tenant_id: str, *, profile: AddUserToSingleTenantsParamsProfile) -> None:
+    def get(self, audit_event_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AuditEvent:
         """
-        This endpoint is used to add a single tenant.
-
-        A custom profile can also be supplied with the tenant.
-        This profile will be merged with the user's main profile
-        when sending to the user with that tenant.
+        Fetch a specific audit event by ID.
 
         Parameters:
-            - user_id: str. Id of the user to be added to the supplied tenant.
+            - audit_event_id: str. A unique identifier associated with the audit event you wish to retrieve
 
-            - tenant_id: str. Id of the tenant the user should be added to.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import Courier
 
-            - profile: AddUserToSingleTenantsParamsProfile.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants/{tenant_id}"),
-            json=jsonable_encoder({"profile": profile}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = Courier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def remove(self, user_id: str, tenant_id: str) -> None:
-        """
-        Removes a user from the supplied tenant.
-
-        Parameters:
-            - user_id: str. Id of the user to be removed from the supplied tenant.
-
-            - tenant_id: str. Id of the tenant the user should be removed from.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants/{tenant_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client.audit_events.get(
+            audit_event_id="string",
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def list(
-        self, user_id: str, *, limit: typing.Optional[int] = None, starting_after: typing.Optional[int] = None
-    ) -> ListTenantsForUserResponse:
-        """
-        Returns a paginated list of user tenant associations.
-
-        Parameters:
-            - user_id: str. Id of the user to retrieve all associated tenants for.
-
-            - limit: typing.Optional[int]. The number of accounts to return
-                                           (defaults to 20, maximum value of 100)
-            - starting_after: typing.Optional[int]. Value of next_page from previous response
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants"),
-            params=remove_none_from_dict({"limit": limit, "starting_after": starting_after}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audit-events/{jsonable_encoder(audit_event_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListTenantsForUserResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AuditEvent, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncTenantsClient:
+class AsyncAuditEventsClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def add_multple(self, user_id: str, *, tenants: typing.List[UserTenantAssociation]) -> None:
+    async def list(
+        self, *, cursor: typing.Optional[str] = None, request_options: typing.Optional[RequestOptions] = None
+    ) -> ListAuditEventsResponse:
         """
-        This endpoint is used to add a user to
-        multiple tenants in one call.
-        A custom profile can also be supplied for each tenant.
-        This profile will be merged with the user's main
-        profile when sending to the user with that tenant.
+        Fetch the list of audit events
 
         Parameters:
-            - user_id: str. The user's ID. This can be any uniquely identifiable string.
+            - cursor: typing.Optional[str]. A unique identifier that allows for fetching the next set of audit events.
+
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
 
-            - tenants: typing.List[UserTenantAssociation].
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
+        )
+        await client.audit_events.list(
+            cursor="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants"),
-            json=jsonable_encoder({"tenants": tenants}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            "GET",
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "audit-events"),
+            params=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        "cursor": cursor,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return
+            return pydantic_v1.parse_obj_as(ListAuditEventsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def add(self, user_id: str, tenant_id: str, *, profile: AddUserToSingleTenantsParamsProfile) -> None:
+    async def get(self, audit_event_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> AuditEvent:
         """
-        This endpoint is used to add a single tenant.
-
-        A custom profile can also be supplied with the tenant.
-        This profile will be merged with the user's main profile
-        when sending to the user with that tenant.
+        Fetch a specific audit event by ID.
 
         Parameters:
-            - user_id: str. Id of the user to be added to the supplied tenant.
+            - audit_event_id: str. A unique identifier associated with the audit event you wish to retrieve
 
-            - tenant_id: str. Id of the tenant the user should be added to.
+            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        ---
+        from courier.client import AsyncCourier
 
-            - profile: AddUserToSingleTenantsParamsProfile.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "PUT",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants/{tenant_id}"),
-            json=jsonable_encoder({"profile": profile}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        client = AsyncCourier(
+            authorization_token="YOUR_AUTHORIZATION_TOKEN",
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def remove(self, user_id: str, tenant_id: str) -> None:
-        """
-        Removes a user from the supplied tenant.
-
-        Parameters:
-            - user_id: str. Id of the user to be removed from the supplied tenant.
-
-            - tenant_id: str. Id of the tenant the user should be removed from.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants/{tenant_id}"),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+        await client.audit_events.get(
+            audit_event_id="string",
         )
-        if 200 <= _response.status_code < 300:
-            return
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def list(
-        self, user_id: str, *, limit: typing.Optional[int] = None, starting_after: typing.Optional[int] = None
-    ) -> ListTenantsForUserResponse:
-        """
-        Returns a paginated list of user tenant associations.
-
-        Parameters:
-            - user_id: str. Id of the user to retrieve all associated tenants for.
-
-            - limit: typing.Optional[int]. The number of accounts to return
-                                           (defaults to 20, maximum value of 100)
-            - starting_after: typing.Optional[int]. Value of next_page from previous response
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/tenants"),
-            params=remove_none_from_dict({"limit": limit, "starting_after": starting_after}),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"audit-events/{jsonable_encoder(audit_event_id)}"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListTenantsForUserResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AuditEvent, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/__init__.py` & `trycourier-6.0.1/src/courier/users/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/delete_user_token_opts.py` & `trycourier-6.0.1/src/courier/profiles/types/send_to_slack_channel.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .slack_base_properties import SlackBaseProperties
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DeleteUserTokenOpts(pydantic.BaseModel):
-    user_id: str
-    token: str
+class SendToSlackChannel(SlackBaseProperties):
+    channel: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/device.py` & `trycourier-6.0.1/src/courier/profiles/types/get_list_subscriptions_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
+from ...commons.types.recipient_preferences import RecipientPreferences
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+
+
+class GetListSubscriptionsList(pydantic_v1.BaseModel):
+    id: str
+    name: str = pydantic_v1.Field()
+    """
+    List name
+    """
+
+    created: str = pydantic_v1.Field()
+    """
+    The date/time of when the list was created. Represented as a string in ISO format.
+    """
+
+    updated: str = pydantic_v1.Field()
+    """
+    The date/time of when the list was updated. Represented as a string in ISO format.
+    """
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Device(pydantic.BaseModel):
-    app_id: typing.Optional[str] = pydantic.Field(description="Id of the application the token is used for")
-    ad_id: typing.Optional[str] = pydantic.Field(description="Id of the advertising identifier")
-    device_id: typing.Optional[str] = pydantic.Field(description="Id of the device the token is associated with")
-    platform: typing.Optional[str] = pydantic.Field(description="The device platform i.e. android, ios, web")
-    manufacturer: typing.Optional[str] = pydantic.Field(description="The device manufacturer")
-    model: typing.Optional[str] = pydantic.Field(description="The device model")
+    preferences: typing.Optional[RecipientPreferences] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_opts.py` & `trycourier-6.0.1/src/courier/send/types/tracking_override.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetUserTokenOpts(pydantic.BaseModel):
-    user_id: str
-    token: str
+class TrackingOverride(pydantic_v1.BaseModel):
+    open: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_token_response.py` & `trycourier-6.0.1/src/courier/types/send_message_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .token_status import TokenStatus
-from .user_token import UserToken
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
 
-class GetUserTokenResponse(UserToken):
-    status: typing.Optional[TokenStatus]
-    status_reason: typing.Optional[str] = pydantic.Field(description="The reason for the token status.")
+class SendMessageResponse(pydantic_v1.BaseModel):
+    request_id: str = pydantic_v1.Field(alias="requestId")
+    """
+    A successful call to `POST /send` returns a `202` status code along with a `requestId` in the response body.
+    
+    For send requests that have a single recipient, the `requestId` is assigned to the derived message as its message_id. Therefore the `requestId` can be supplied to the Message's API for single recipient messages.
+    
+    For send requests that have multiple recipients (accounts, audiences, lists, etc.), Courier assigns a unique id to each derived message as its `message_id`. Therefore the `requestId` cannot be supplied to the Message's API for single-recipient messages.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/get_user_tokens_opts.py` & `trycourier-6.0.1/src/courier/send/types/invalid_list_pattern_recipient.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetUserTokensOpts(pydantic.BaseModel):
+class InvalidListPatternRecipient(pydantic_v1.BaseModel):
     user_id: str
+    list_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_operation.py` & `trycourier-6.0.1/src/courier/automations/types/accessor_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PatchOperation(pydantic.BaseModel):
-    op: str = pydantic.Field(description="The operation to perform.")
-    path: str = pydantic.Field(description="The JSON path specifying the part of the profile to operate on.")
-    value: typing.Optional[str] = pydantic.Field(description="The value for the operation.")
+class AccessorType(pydantic_v1.BaseModel):
+    ref: str = pydantic_v1.Field(alias="$ref")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/patch_user_token_opts.py` & `trycourier-6.0.1/src/courier/bulk/types/bulk_get_job_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .patch_operation import PatchOperation
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PatchUserTokenOpts(pydantic.BaseModel):
-    patch: typing.List[PatchOperation]
+class BulkGetJobParams(pydantic_v1.BaseModel):
+    job_id: str = pydantic_v1.Field(alias="jobId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/src/courier/resources/users/resources/tokens/types/put_user_tokens_opts.py` & `trycourier-6.0.1/src/courier/send/types/list_filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ......core.datetime_utils import serialize_datetime
-from .user_token import UserToken
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ListFilter(pydantic_v1.BaseModel):
+    operator: typing.Literal["MEMBER_OF"] = pydantic_v1.Field()
+    """
+    Send to users only if they are member of the account
+    """
 
-class PutUserTokensOpts(pydantic.BaseModel):
-    user_id: str
-    tokens: typing.List[UserToken]
+    path: typing.Literal["account_id"]
+    value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `trycourier-6.0.0b1/PKG-INFO` & `trycourier-6.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 6.0.0b1
+Version: 6.0.1
 Summary: 
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.21.2)
-Requires-Dist: pydantic (>=1.9.2,<2.5.0)
+Requires-Dist: pydantic (>=1.9.2)
+Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 [![Courier: Your Complete Communication Stack](https://marketing-assets-public.s3.us-west-1.amazonaws.com/github_nodejs.png)](https://courier.com)
 
 [![pypi](https://img.shields.io/pypi/v/trycourier.svg)](https://pypi.python.org/pypi/trycourier)
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://buildwithfern.com/?utm_source=trycourier/courier-node/readme)
```

