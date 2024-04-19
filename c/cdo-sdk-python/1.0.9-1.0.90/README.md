# Comparing `tmp/cdo-sdk-python-1.0.9.tar.gz` & `tmp/cdo-sdk-python-1.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdo-sdk-python-1.0.9.tar", last modified: Thu Mar 21 10:28:06 2024, max compression
+gzip compressed data, was "cdo-sdk-python-1.0.90.tar", last modified: Fri Apr 19 08:30:58 2024, max compression
```

## Comparing `cdo-sdk-python-1.0.9.tar` & `cdo-sdk-python-1.0.90.tar`

### file list

```diff
@@ -1,223 +1,234 @@
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.437774 cdo-sdk-python-1.0.9/
--rw-r--r--   0 talhazi    (501) staff       (20)      487 2024-03-21 10:28:06.437679 cdo-sdk-python-1.0.9/PKG-INFO
--rw-r--r--   0 talhazi    (501) staff       (20)    17897 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/README.md
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.381449 cdo-sdk-python-1.0.9/cdo_sdk_python/
--rw-r--r--   0 talhazi    (501) staff       (20)     7187 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/__init__.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.387199 cdo-sdk-python-1.0.9/cdo_sdk_python/api/
--rw-r--r--   0 talhazi    (501) staff       (20)      741 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/__init__.py
--rw-r--r--   0 talhazi    (501) staff       (20)    47311 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/change_requests_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    28620 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/changelogs_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    25448 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/connectors_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)   288736 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/inventory_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    29485 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/meta_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    92507 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/object_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    47688 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/remote_access_monitoring_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    20940 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/search_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    64302 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/tenant_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    11540 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/transactions_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    85366 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api/users_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)    25814 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api_client.py
--rw-r--r--   0 talhazi    (501) staff       (20)      652 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/api_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)    15498 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/configuration.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5995 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/exceptions.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.403154 cdo-sdk-python-1.0.9/cdo_sdk_python/models/
--rw-r--r--   0 talhazi    (501) staff       (20)     5950 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/__init__.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2608 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/api_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4440 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3282 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mate.py
--rw-r--r--   0 talhazi    (501) staff       (20)      852 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2864 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/authentication_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3992 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2950 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_object.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4247 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2960 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3005 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region_list.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3717 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5194 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction.py
--rw-r--r--   0 talhazi    (501) staff       (20)      859 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1297 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2871 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2800 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_create_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3675 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3860 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3642 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3894 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/common_api_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1128 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/config_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      997 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_interval.py
--rw-r--r--   0 talhazi    (501) staff       (20)      906 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1069 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/connectivity_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      935 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/connector_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3702 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/create_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)    10882 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3618 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2958 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_patch_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)      865 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3617 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3370 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1403 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4330 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/event.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5134 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2665 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_registration_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4126 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/global_search_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3340 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/group_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6090 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp4_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6408 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp6_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4187 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/inventory.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4132 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ios_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2617 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/issues_dto.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3330 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/json_web_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2976 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/jwk_set.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2933 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/labels.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3788 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/list_object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3085 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/location.py
--rw-r--r--   0 talhazi    (501) staff       (20)      849 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/meraki_deployment_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2744 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/meta.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2601 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/msp_add_tenant_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3096 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/network.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2614 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/network_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     7141 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5839 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2895 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/on_prem_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2861 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/os.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3131 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/override.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2761 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/policy.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3109 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ports_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5985 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3668 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3409 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/reference_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4129 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3594 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3024 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_public_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)      876 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5594 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6005 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_value_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4210 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/shared_object_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     6359 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/single_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2673 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/sort_criteria_param.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3051 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_details.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2920 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2578 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/status_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3673 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/target.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2667 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/targets_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3531 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3618 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      921 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_pay_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4891 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_settings.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4001 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/unified_object_list_view.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3453 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/update_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2545 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/url_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3512 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3036 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3602 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1038 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)        0 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/py.typed
--rw-r--r--   0 talhazi    (501) staff       (20)     9255 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/cdo_sdk_python/rest.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.437271 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/
--rw-r--r--   0 talhazi    (501) staff       (20)      487 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 talhazi    (501) staff       (20)     7359 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 talhazi    (501) staff       (20)        1 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 talhazi    (501) staff       (20)       76 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/requires.txt
--rw-r--r--   0 talhazi    (501) staff       (20)       15 2024-03-21 10:28:06.000000 cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 talhazi    (501) staff       (20)     1956 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/pyproject.toml
--rw-r--r--   0 talhazi    (501) staff       (20)       69 2024-03-21 10:28:06.438079 cdo-sdk-python-1.0.9/setup.cfg
--rw-r--r--   0 talhazi    (501) staff       (20)     1334 2024-03-21 10:25:10.000000 cdo-sdk-python-1.0.9/setup.py
-drwxr-xr-x   0 talhazi    (501) staff       (20)        0 2024-03-21 10:28:06.436840 cdo-sdk-python-1.0.9/test/
--rw-r--r--   0 talhazi    (501) staff       (20)     1372 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_api_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2123 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_asa_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1504 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_asa_failover_mate.py
--rw-r--r--   0 talhazi    (501) staff       (20)      720 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_asa_failover_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1515 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_authentication_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1582 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cd_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1634 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cd_fmc_object.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2711 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cd_fmc_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1389 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_region.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1579 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_region_list.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1658 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_token_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2201 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_transaction.py
--rw-r--r--   0 talhazi    (501) staff       (20)      755 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_transaction_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)      741 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_cdo_transaction_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1616 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1648 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_request_create_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1793 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_request_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1338 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_change_requests_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2060 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_changelog.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2353 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_changelog_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      952 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_changelogs_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1528 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_common_api_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)      691 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_config_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      790 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_conflict_detection_interval.py
--rw-r--r--   0 talhazi    (501) staff       (20)      769 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_conflict_detection_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      733 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_connectivity_state.py
--rw-r--r--   0 talhazi    (501) staff       (20)      705 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_connector_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)      934 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_connectors_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2365 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_create_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4224 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device.py
--rw-r--r--   0 talhazi    (501) staff       (20)     4807 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1651 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device_patch_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)      684 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_device_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2219 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_duo_admin_panel_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1559 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_entity.py
--rw-r--r--   0 talhazi    (501) staff       (20)      684 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_entity_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1619 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_event.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2094 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ftd_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1558 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ftd_registration_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     3863 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_global_search_result.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1537 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_group_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1409 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_icmp4_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1413 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_icmp6_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2713 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_inventory.py
--rw-r--r--   0 talhazi    (501) staff       (20)     5153 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_inventory_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2085 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ios_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1377 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_issues_dto.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1458 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_json_web_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1579 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_jwk_set.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1422 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_labels.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2724 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_list_object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1382 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_location.py
--rw-r--r--   0 talhazi    (501) staff       (20)      755 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_meraki_deployment_mode.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1318 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_meta.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1069 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_meta_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1475 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_msp_add_tenant_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1391 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_network.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1502 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_network_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1813 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1929 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_object_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2631 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_object_response.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1444 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_on_prem_fmc_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1280 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_os.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1448 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_override.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1362 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_policy.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1372 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ports_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2429 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ra_vpn_session.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2672 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_ra_vpn_session_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1456 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_reference_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1042 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_remote_access_monitoring_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2508 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2781 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2186 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc_public_key.py
--rw-r--r--   0 talhazi    (501) staff       (20)      677 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sdc_status.py
--rw-r--r--   0 talhazi    (501) staff       (20)      964 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_search_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1520 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_service_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1763 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_service_object_value_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1748 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_shared_object_value.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1607 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_single_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1539 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_sort_criteria_param.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1663 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_state_machine_details.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1499 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_state_machine_error.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1336 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_status_info.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1390 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_target.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1427 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_targets_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1545 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1632 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_management_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1831 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      706 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_pay_type.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1816 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_tenant_settings.py
--rw-r--r--   0 talhazi    (501) staff       (20)      822 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_transactions_api.py
--rw-r--r--   0 talhazi    (501) staff       (20)     2335 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_unified_object_list_view.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1896 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_update_request.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1474 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_url_object_content.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1482 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1634 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user_create_or_update_input.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1764 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user_page.py
--rw-r--r--   0 talhazi    (501) staff       (20)      670 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_user_role.py
--rw-r--r--   0 talhazi    (501) staff       (20)     1826 2024-03-21 09:21:18.000000 cdo-sdk-python-1.0.9/test/test_users_api.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-19 08:30:58.396486 cdo-sdk-python-1.0.90/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3710 2024-04-19 08:30:58.396486 cdo-sdk-python-1.0.90/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    19243 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-19 08:30:58.360486 cdo-sdk-python-1.0.90/cdo_sdk_python/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8117 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-19 08:30:58.364486 cdo-sdk-python-1.0.90/cdo_sdk_python/api/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      899 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    47620 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/change_requests_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    28767 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/changelogs_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    56491 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/cloud_delivered_fmc_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    58557 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/connectors_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   295873 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/inventory_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    29653 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/meta_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   114554 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/object_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    85076 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/remote_access_monitoring_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21766 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/search_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    65201 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/tenant_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12108 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/transactions_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    88351 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api/users_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25780 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api_client.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      652 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/api_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15464 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/configuration.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5960 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/exceptions.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-19 08:30:58.380486 cdo-sdk-python-1.0.90/cdo_sdk_python/models/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6721 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2573 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/api_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4405 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/asa_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3247 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/asa_failover_mate.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      817 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/asa_failover_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2829 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/authentication_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2777 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/browser.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3957 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cd_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2915 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cd_fmc_object.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4212 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cd_fmc_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2925 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_region.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2970 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_region_list.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3682 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5159 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_transaction.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      824 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_transaction_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1348 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_transaction_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2836 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/change_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2765 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/change_request_create_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3633 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/change_request_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3825 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/changelog.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3600 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/changelog_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4457 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/client_device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3859 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/common_api_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1093 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/config_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      962 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/conflict_detection_interval.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      871 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/conflict_detection_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1034 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/connectivity_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      900 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/connector_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3667 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/create_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10847 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3576 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/device_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2923 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/device_patch_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      886 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/device_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3582 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3335 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/entity.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1368 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/entity_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4295 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5099 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/ftd_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2630 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/ftd_registration_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4091 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/global_search_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3305 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/group_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6055 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/icmp4_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6373 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/icmp6_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4152 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/inventory.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4097 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/ios_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2771 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/issues_dto.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3295 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/json_web_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2941 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/jwk_set.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2898 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/labels.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3746 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/list_object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2961 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/location.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      814 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/meraki_deployment_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2709 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/meta.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4550 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/mfa_event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3593 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/mfa_event_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2566 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/msp_add_tenant_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3061 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/network.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2579 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/network_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7106 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5804 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2860 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/on_prem_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2765 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/os.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3096 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/override.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2726 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/policy.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3074 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/ports_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2980 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5950 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/ra_vpn_session.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3626 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/ra_vpn_session_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3374 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/reference_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4507 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/sdc.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3552 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/sdc_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3024 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/sdc_public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      876 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/sdc_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5575 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/service_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5970 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/service_object_value_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4175 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/shared_object_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6324 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/single_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3016 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/state_machine_details.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2885 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/state_machine_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      835 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2543 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/status_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3638 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/target.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2632 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/targets_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3496 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3576 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      886 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant_pay_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4856 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant_settings.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3966 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/unified_object_list_view.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3418 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/update_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2510 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/url_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3477 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/user.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3001 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/user_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3560 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/user_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1003 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/models/user_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9220 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/cdo_sdk_python/rest.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-19 08:30:58.360486 cdo-sdk-python-1.0.90/cdo_sdk_python.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3710 2024-04-19 08:30:58.000000 cdo-sdk-python-1.0.90/cdo_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7698 2024-04-19 08:30:58.000000 cdo-sdk-python-1.0.90/cdo_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-04-19 08:30:58.000000 cdo-sdk-python-1.0.90/cdo_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       76 2024-04-19 08:30:58.000000 cdo-sdk-python-1.0.90/cdo_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       15 2024-04-19 08:30:58.000000 cdo-sdk-python-1.0.90/cdo_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1911 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/pyproject.toml
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       69 2024-04-19 08:30:58.400486 cdo-sdk-python-1.0.90/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1203 2024-04-19 08:30:45.000000 cdo-sdk-python-1.0.90/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-19 08:30:58.396486 cdo-sdk-python-1.0.90/test/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1394 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_api_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2145 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_asa_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_asa_failover_mate.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      742 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_asa_failover_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1537 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_authentication_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1367 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_browser.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cd_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1656 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cd_fmc_object.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2733 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cd_fmc_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1411 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cdo_region.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1601 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cdo_region_list.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1680 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cdo_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2223 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cdo_transaction.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      777 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cdo_transaction_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      763 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cdo_transaction_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1638 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_change_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1670 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_change_request_create_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1815 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_change_request_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1286 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_change_requests_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_changelog.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2375 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_changelog_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      930 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_changelogs_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2124 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_client_device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1840 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_cloud_delivered_fmc_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1496 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_common_api_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      713 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_config_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      812 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_conflict_detection_interval.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      791 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_conflict_detection_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      755 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_connectivity_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      727 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_connector_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      891 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_connectors_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2387 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_create_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4246 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4829 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_device_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1673 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_device_patch_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      706 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_device_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2241 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_duo_admin_panel_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1581 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_entity.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      706 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_entity_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1641 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2116 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_ftd_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1580 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_ftd_registration_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3885 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_global_search_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1559 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_group_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1431 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_icmp4_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1435 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_icmp6_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2735 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_inventory.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4407 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_inventory_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2107 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_ios_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1399 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_issues_dto.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1480 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_json_web_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1601 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_jwk_set.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1444 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_labels.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2746 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_list_object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1404 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_location.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      777 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_meraki_deployment_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1340 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_meta.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1031 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_meta_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2627 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_mfa_event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2956 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_mfa_event_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1497 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_msp_add_tenant_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1413 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_network.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1524 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_network_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1835 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1738 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_object_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2653 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1466 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_on_prem_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1302 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_os.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1470 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_override.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1384 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_policy.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1394 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_ports_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2171 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2451 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_ra_vpn_session.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2694 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_ra_vpn_session_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1478 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_reference_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1427 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_remote_access_monitoring_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2530 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_sdc.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2803 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_sdc_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2208 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_sdc_public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      699 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_sdc_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      908 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_search_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1542 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_service_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1785 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_service_object_value_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1770 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_shared_object_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1629 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_single_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1685 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_state_machine_details.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1521 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_state_machine_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      677 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1358 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_status_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1412 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_target.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1449 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_targets_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1567 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_tenant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1530 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_tenant_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1853 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_tenant_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      728 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_tenant_pay_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1838 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_tenant_settings.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      810 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_transactions_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2357 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_unified_object_list_view.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1918 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_update_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1496 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_url_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1504 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_user.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1656 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_user_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1786 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_user_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      692 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_user_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1724 2024-04-19 08:30:40.000000 cdo-sdk-python-1.0.90/test/test_users_api.py
```

### Comparing `cdo-sdk-python-1.0.9/README.md` & `cdo-sdk-python-1.0.90/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cdo-sdk-python
-Use the interactive documentation to explore the endpoints CDO has to offer
+Use the documentation to explore the endpoints CDO has to offer
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.1
-- Package version: 1.0.9
+- API version: 0.1.0
+- Package version: 1.0.90
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
@@ -75,171 +75,201 @@
 # Enter a context with an instance of the API client
 with cdo_sdk_python.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = cdo_sdk_python.ChangeRequestsApi(api_client)
     change_request_create_input = cdo_sdk_python.ChangeRequestCreateInput() # ChangeRequestCreateInput | 
 
     try:
-        # Create Change Requests.
+        # Create Change Request
         api_response = api_instance.create_change_request(change_request_create_input)
         print("The response of ChangeRequestsApi->create_change_request:\n")
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling ChangeRequestsApi->create_change_request: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://edge.us.cdo.cisco.com/api/rest*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*ChangeRequestsApi* | [**create_change_request**](docs/ChangeRequestsApi.md#create_change_request) | **POST** /v1/changeRequests | Create Change Requests.
-*ChangeRequestsApi* | [**delete_change_request**](docs/ChangeRequestsApi.md#delete_change_request) | **DELETE** /v1/changeRequests/{changeRequestUid} | Delete a Change Request by UID in the CDO tenant
-*ChangeRequestsApi* | [**get_change_request**](docs/ChangeRequestsApi.md#get_change_request) | **GET** /v1/changeRequests/{changeRequestUid} | Fetch a Change Request by UID in the CDO tenant.
-*ChangeRequestsApi* | [**list_change_requests**](docs/ChangeRequestsApi.md#list_change_requests) | **GET** /v1/changeRequests | Fetch a list of Change Requests.
-*ChangelogsApi* | [**get_changelog**](docs/ChangelogsApi.md#get_changelog) | **GET** /v1/changelogs/{changelogUid} | Fetch a Change Log by UID in the CDO tenant.
-*ChangelogsApi* | [**list_changelogs**](docs/ChangelogsApi.md#list_changelogs) | **GET** /v1/changelogs | Fetch a list of Change Logs.
-*ConnectorsApi* | [**fetch_sdc**](docs/ConnectorsApi.md#fetch_sdc) | **GET** /v1/connectors/sdcs/{sdcUid} | Fetch a SDC by UID in the CDO tenant
-*ConnectorsApi* | [**list_sdcs**](docs/ConnectorsApi.md#list_sdcs) | **GET** /v1/connectors/sdcs | Fetch a list of SDCs in the CDO tenant
-*InventoryApi* | [**create_duo_admin_panel**](docs/InventoryApi.md#create_duo_admin_panel) | **POST** /v1/inventory/devices/duoAdminPanels | Onboard a Duo Admin Panel in the CDO tenant
-*InventoryApi* | [**create_ftd_device**](docs/InventoryApi.md#create_ftd_device) | **POST** /v1/inventory/devices/ftds | Create an FTD device in the CDO tenant
-*InventoryApi* | [**delete_cd_fmc_managed_ftd_device**](docs/InventoryApi.md#delete_cd_fmc_managed_ftd_device) | **POST** /v1/inventory/devices/ftds/cdfmcManaged/{deviceUid}/delete | Delete cdFMC managed FTD device in the CDO tenant
-*InventoryApi* | [**delete_cloud_service**](docs/InventoryApi.md#delete_cloud_service) | **DELETE** /v1/inventory/services/{cloudServiceUid} | Delete a Cloud Service by UID in the CDO tenant
-*InventoryApi* | [**delete_device**](docs/InventoryApi.md#delete_device) | **DELETE** /v1/inventory/devices/{deviceUid} | Delete a device by UID in the CDO tenant
-*InventoryApi* | [**delete_device_manager**](docs/InventoryApi.md#delete_device_manager) | **DELETE** /v1/inventory/managers/{deviceManagerUid} | Delete a Device Manager by UID in the CDO tenant
-*InventoryApi* | [**delete_template_device**](docs/InventoryApi.md#delete_template_device) | **DELETE** /v1/inventory/templates/{templateDeviceUid} | Delete a template device by UID in the CDO tenant
-*InventoryApi* | [**deploy_asa_device_changes**](docs/InventoryApi.md#deploy_asa_device_changes) | **POST** /v1/inventory/devices/asas/{deviceUid}/deploy | Deploy changes to an ASA device in the CDO tenant
-*InventoryApi* | [**finish_onboarding_ftd_device**](docs/InventoryApi.md#finish_onboarding_ftd_device) | **POST** /v1/inventory/devices/ftds/register | Register an FTD device managed by an FMC to the CDO tenant. Call this API endpoint after you have created an FTD, and pasted the generated CLI output in the FTD
-*InventoryApi* | [**get_cloud_service**](docs/InventoryApi.md#get_cloud_service) | **GET** /v1/inventory/services/{cloudServiceUid} | Fetch a Cloud Service by UID in the CDO tenant
-*InventoryApi* | [**get_device**](docs/InventoryApi.md#get_device) | **GET** /v1/inventory/devices/{deviceUid} | Fetch a device by UID in the CDO tenant
-*InventoryApi* | [**get_device_manager**](docs/InventoryApi.md#get_device_manager) | **GET** /v1/inventory/managers/{deviceManagerUid} | Fetch a Device Manager by UID in the CDO tenant
-*InventoryApi* | [**get_template_device**](docs/InventoryApi.md#get_template_device) | **GET** /v1/inventory/templates/{templateDeviceUid} | Fetch a template device by UID in the CDO tenant
-*InventoryApi* | [**list_device_cloud_services**](docs/InventoryApi.md#list_device_cloud_services) | **GET** /v1/inventory/services | Fetch a list of Cloud Services in the CDO tenant
-*InventoryApi* | [**list_device_managers**](docs/InventoryApi.md#list_device_managers) | **GET** /v1/inventory/managers | Fetch a list of Device Managers (on-prem FMCs and cloud-delivered FMCs) in the CDO tenant
-*InventoryApi* | [**list_devices**](docs/InventoryApi.md#list_devices) | **GET** /v1/inventory/devices | Fetch a list of devices in the CDO tenant
-*InventoryApi* | [**list_template_devices**](docs/InventoryApi.md#list_template_devices) | **GET** /v1/inventory/templates | Fetch a list of template devices in the CDO tenant
-*InventoryApi* | [**onboard_asa_device**](docs/InventoryApi.md#onboard_asa_device) | **POST** /v1/inventory/devices/asas | Onboard a ASA device in the CDO tenant
-*InventoryApi* | [**onboard_ios_device**](docs/InventoryApi.md#onboard_ios_device) | **POST** /v1/inventory/devices/ios | Onboard a IOS device in the CDO tenant
-*InventoryApi* | [**patch_cloud_service**](docs/InventoryApi.md#patch_cloud_service) | **PATCH** /v1/inventory/services/{cloudServiceUid} | Modify a Cloud Service by UID in the CDO tenant
-*InventoryApi* | [**patch_device**](docs/InventoryApi.md#patch_device) | **PATCH** /v1/inventory/devices/{deviceUid} | Modify a device in the CDO tenant
-*InventoryApi* | [**patch_device_manager**](docs/InventoryApi.md#patch_device_manager) | **PATCH** /v1/inventory/managers/{deviceManagerUid} | Modify a device manager by UID in the CDO tenant
-*InventoryApi* | [**patch_template_device**](docs/InventoryApi.md#patch_template_device) | **PATCH** /v1/inventory/templates/{templateDeviceUid} | Modify a template device in the CDO tenant
-*InventoryApi* | [**read_from_asa_device**](docs/InventoryApi.md#read_from_asa_device) | **POST** /v1/inventory/devices/asas/{deviceUid}/read | Read configuration on ASA device into CDO
-*InventoryApi* | [**reconnect_asa_device**](docs/InventoryApi.md#reconnect_asa_device) | **POST** /v1/inventory/devices/asas/{deviceUid}/reconnect | Reconnect an ASA device in the CDO tenant
-*MetaApi* | [**get_jwks**](docs/MetaApi.md#get_jwks) | **GET** /.well-known/jwks.json | Fetch The JSON Web Key Set
-*MetaApi* | [**get_meta**](docs/MetaApi.md#get_meta) | **GET** /v1/meta | Get Meta information about CDO, including the IP addresses of CDO services
-*MetaApi* | [**list_regions**](docs/MetaApi.md#list_regions) | **GET** /v1/regions | Fetch a list of CDO regions.
-*ObjectManagementApi* | [**create_object**](docs/ObjectManagementApi.md#create_object) | **POST** /v0/objects | Creates an object in the CDO tenant
-*ObjectManagementApi* | [**create_targets**](docs/ObjectManagementApi.md#create_targets) | **POST** /v0/objects/{uid}/targets | Create targets for an object in the CDO tenant
-*ObjectManagementApi* | [**delete_object**](docs/ObjectManagementApi.md#delete_object) | **DELETE** /v0/objects/{uid} | Deletes an object in the CDO tenant
-*ObjectManagementApi* | [**get_object**](docs/ObjectManagementApi.md#get_object) | **GET** /v0/objects/{uid} | Retrieves an object in the CDO tenant
-*ObjectManagementApi* | [**get_object_usage**](docs/ObjectManagementApi.md#get_object_usage) | **GET** /v0/objects/{uid}/usage | Retrieves usages of an object in the CDO tenant
-*ObjectManagementApi* | [**list_objects**](docs/ObjectManagementApi.md#list_objects) | **GET** /v0/objects | Retrieves objects in the CDO tenant
-*ObjectManagementApi* | [**remove_targets**](docs/ObjectManagementApi.md#remove_targets) | **DELETE** /v0/objects/{uid}/targets | Removes targets from an object in the CDO tenant
-*ObjectManagementApi* | [**update_object**](docs/ObjectManagementApi.md#update_object) | **PATCH** /v0/objects/{uid} | Updates an object in the CDO tenant
-*RemoteAccessMonitoringApi* | [**get_ra_vpn_session**](docs/RemoteAccessMonitoringApi.md#get_ra_vpn_session) | **GET** /v1/vpnsessions/{raVpnSessionUid} | Fetch a RA VPN session by UID in the CDO tenant.
-*RemoteAccessMonitoringApi* | [**list_ra_vpn_sessions**](docs/RemoteAccessMonitoringApi.md#list_ra_vpn_sessions) | **GET** /v1/vpnsessions | Fetch a list of RA VPN sessions.
-*RemoteAccessMonitoringApi* | [**terminate_ra_vpn_sessions_by_device**](docs/RemoteAccessMonitoringApi.md#terminate_ra_vpn_sessions_by_device) | **POST** /v1/vpnsessions/{deviceUid}/terminate | Terminate all RA VPN sessions on a device in the CDO tenant.
-*RemoteAccessMonitoringApi* | [**terminate_ra_vpn_sessions_by_device_and_user_name**](docs/RemoteAccessMonitoringApi.md#terminate_ra_vpn_sessions_by_device_and_user_name) | **POST** /v1/vpnsessions/{deviceUid}/terminate/{userName} | Terminate all of a user&#39;s RA VPN sessions on a device in the CDO tenant
-*SearchApi* | [**initiate_full_indexing**](docs/SearchApi.md#initiate_full_indexing) | **POST** /v1/search/index | Initiate Full Indexing
-*SearchApi* | [**search**](docs/SearchApi.md#search) | **GET** /v1/search | Search for devices, services, managers, objects and policies across the CDO tenant
-*TenantManagementApi* | [**add_msp_tenant**](docs/TenantManagementApi.md#add_msp_tenant) | **POST** /v1/msp/tenants | Add a tenant to the MSP Portal
-*TenantManagementApi* | [**get_tenant**](docs/TenantManagementApi.md#get_tenant) | **GET** /v1/tenants/{tenantUid} | Fetch a tenant by UID in CDO
-*TenantManagementApi* | [**get_tenant_settings**](docs/TenantManagementApi.md#get_tenant_settings) | **GET** /v1/settings/tenant | Fetch the tenant settings in CDO
-*TenantManagementApi* | [**list_feature_flags**](docs/TenantManagementApi.md#list_feature_flags) | **GET** /v1/features | Fetch the feature flags enabled for this tenant
-*TenantManagementApi* | [**list_tenants**](docs/TenantManagementApi.md#list_tenants) | **GET** /v1/tenants | Fetch a list of tenants associated with the CDO user.
-*TenantManagementApi* | [**update_tenant_settings**](docs/TenantManagementApi.md#update_tenant_settings) | **PATCH** /v1/settings/tenant | Update the tenant settings in CDO
-*TransactionsApi* | [**get_transaction**](docs/TransactionsApi.md#get_transaction) | **GET** /v1/transactions/{transactionUid} | Get information of an in-progress CDO transaction
-*UsersApi* | [**create_user**](docs/UsersApi.md#create_user) | **POST** /v1/users | Create a user in the CDO tenant
-*UsersApi* | [**delete_user**](docs/UsersApi.md#delete_user) | **DELETE** /v1/users/{userUid} | Delete a User by UID in the CDO tenant
-*UsersApi* | [**generate_api_token**](docs/UsersApi.md#generate_api_token) | **POST** /v1/users/{apiUserId}/apiToken/generate | Generate API Token for API-only user
-*UsersApi* | [**get_token**](docs/UsersApi.md#get_token) | **GET** /v1/token | Fetch information on the current token
-*UsersApi* | [**get_user**](docs/UsersApi.md#get_user) | **GET** /v1/users/{userUid} | Fetch a user by UID in the CDO tenant.
-*UsersApi* | [**list_users**](docs/UsersApi.md#list_users) | **GET** /v1/users | Fetch a list of users associated with the CDO tenant.
-*UsersApi* | [**revoke_api_token**](docs/UsersApi.md#revoke_api_token) | **POST** /v1/users/{apiUserId}/apiToken/revoke | Revoke API Token of API-only user
-*UsersApi* | [**revoke_token**](docs/UsersApi.md#revoke_token) | **POST** /v1/token/revoke | Revoke the current token
+*ChangeRequestsApi* | [**create_change_request**](docs/ChangeRequestsApi.md#create_change_request) | **POST** /v1/changeRequests | Create Change Request
+*ChangeRequestsApi* | [**delete_change_request**](docs/ChangeRequestsApi.md#delete_change_request) | **DELETE** /v1/changeRequests/{changeRequestUid} | Delete Change Request
+*ChangeRequestsApi* | [**get_change_request**](docs/ChangeRequestsApi.md#get_change_request) | **GET** /v1/changeRequests/{changeRequestUid} | Get Change Request
+*ChangeRequestsApi* | [**get_change_requests**](docs/ChangeRequestsApi.md#get_change_requests) | **GET** /v1/changeRequests | Get Change Requests
+*ChangelogsApi* | [**get_changelog**](docs/ChangelogsApi.md#get_changelog) | **GET** /v1/changelogs/{changelogUid} | Get Change Log
+*ChangelogsApi* | [**get_changelogs**](docs/ChangelogsApi.md#get_changelogs) | **GET** /v1/changelogs | Get Change Logs
+*CloudDeliveredFMCApi* | [**proxy_fmc_request**](docs/CloudDeliveredFMCApi.md#proxy_fmc_request) | **GET** /v1/cdfmc/** | Proxy Request To Cloud-Delivered FMC
+*CloudDeliveredFMCApi* | [**proxy_fmc_request1**](docs/CloudDeliveredFMCApi.md#proxy_fmc_request1) | **POST** /v1/cdfmc/** | Proxy Request To Cloud-Delivered FMC
+*CloudDeliveredFMCApi* | [**proxy_fmc_request2**](docs/CloudDeliveredFMCApi.md#proxy_fmc_request2) | **PUT** /v1/cdfmc/** | Proxy Request To Cloud-Delivered FMC
+*CloudDeliveredFMCApi* | [**proxy_fmc_request3**](docs/CloudDeliveredFMCApi.md#proxy_fmc_request3) | **PATCH** /v1/cdfmc/** | Proxy Request To Cloud-Delivered FMC
+*CloudDeliveredFMCApi* | [**proxy_fmc_request4**](docs/CloudDeliveredFMCApi.md#proxy_fmc_request4) | **DELETE** /v1/cdfmc/** | Proxy Request To Cloud-Delivered FMC
+*CommandLineInterfaceApi* | [**get_cli_macro**](docs/CommandLineInterfaceApi.md#get_cli_macro) | **GET** /cli/macros/{macroUid} | Get CLI Macro
+*CommandLineInterfaceApi* | [**get_cli_macros**](docs/CommandLineInterfaceApi.md#get_cli_macros) | **GET** /cli/macros | Get CLI Macros
+*CommandLineInterfaceApi* | [**get_cli_result**](docs/CommandLineInterfaceApi.md#get_cli_result) | **GET** /cli/results/{cliResultUid} | Get CLI Result
+*CommandLineInterfaceApi* | [**get_cli_results**](docs/CommandLineInterfaceApi.md#get_cli_results) | **GET** /cli/results | Get CLI Results
+*ConnectorsApi* | [**create_sdc**](docs/ConnectorsApi.md#create_sdc) | **POST** /v1/connectors/sdcs | Create SDC
+*ConnectorsApi* | [**delete_sdc**](docs/ConnectorsApi.md#delete_sdc) | **DELETE** /v1/connectors/sdcs/{sdcUid} | Delete SDC
+*ConnectorsApi* | [**get_sdc**](docs/ConnectorsApi.md#get_sdc) | **GET** /v1/connectors/sdcs/{sdcUid} | Get SDC
+*ConnectorsApi* | [**get_sdcs**](docs/ConnectorsApi.md#get_sdcs) | **GET** /v1/connectors/sdcs | Get SDCs
+*ConnectorsApi* | [**modify_sdc**](docs/ConnectorsApi.md#modify_sdc) | **PATCH** /v1/connectors/sdcs/{sdcUid} | Modify SDC
+*InventoryApi* | [**create_duo_admin_panel**](docs/InventoryApi.md#create_duo_admin_panel) | **POST** /v1/inventory/devices/duoAdminPanels | Onboard Duo Admin Panel
+*InventoryApi* | [**create_ftd_device**](docs/InventoryApi.md#create_ftd_device) | **POST** /v1/inventory/devices/ftds | Create FTD device.
+*InventoryApi* | [**delete_cd_fmc_managed_ftd_device**](docs/InventoryApi.md#delete_cd_fmc_managed_ftd_device) | **POST** /v1/inventory/devices/ftds/cdfmcManaged/{deviceUid}/delete | Delete cdFMC managed FTD device
+*InventoryApi* | [**delete_cloud_service**](docs/InventoryApi.md#delete_cloud_service) | **DELETE** /v1/inventory/services/{cloudServiceUid} | Delete Cloud Service
+*InventoryApi* | [**delete_device**](docs/InventoryApi.md#delete_device) | **DELETE** /v1/inventory/devices/{deviceUid} | Delete Device
+*InventoryApi* | [**delete_device_manager**](docs/InventoryApi.md#delete_device_manager) | **DELETE** /v1/inventory/managers/{deviceManagerUid} | Delete Device Manager
+*InventoryApi* | [**delete_template_device**](docs/InventoryApi.md#delete_template_device) | **DELETE** /v1/inventory/templates/{templateDeviceUid} | Delete Template Device
+*InventoryApi* | [**deploy_asa_device_changes**](docs/InventoryApi.md#deploy_asa_device_changes) | **POST** /v1/inventory/devices/asas/{deviceUid}/deploy | Deploy ASA device changes
+*InventoryApi* | [**finish_onboarding_ftd_device**](docs/InventoryApi.md#finish_onboarding_ftd_device) | **POST** /v1/inventory/devices/ftds/register | Register FTD device.
+*InventoryApi* | [**get_cloud_service**](docs/InventoryApi.md#get_cloud_service) | **GET** /v1/inventory/services/{cloudServiceUid} | Get Cloud Service
+*InventoryApi* | [**get_cloud_services**](docs/InventoryApi.md#get_cloud_services) | **GET** /v1/inventory/services | Get Cloud Services
+*InventoryApi* | [**get_device**](docs/InventoryApi.md#get_device) | **GET** /v1/inventory/devices/{deviceUid} | Get Device
+*InventoryApi* | [**get_device_manager**](docs/InventoryApi.md#get_device_manager) | **GET** /v1/inventory/managers/{deviceManagerUid} | Get Device Manager
+*InventoryApi* | [**get_device_managers**](docs/InventoryApi.md#get_device_managers) | **GET** /v1/inventory/managers | Get Device Managers
+*InventoryApi* | [**get_devices**](docs/InventoryApi.md#get_devices) | **GET** /v1/inventory/devices | Get Devices
+*InventoryApi* | [**get_template_device**](docs/InventoryApi.md#get_template_device) | **GET** /v1/inventory/templates/{templateDeviceUid} | Get Template Device
+*InventoryApi* | [**get_template_devices**](docs/InventoryApi.md#get_template_devices) | **GET** /v1/inventory/templates | Get Template Devices
+*InventoryApi* | [**modify_cloud_service**](docs/InventoryApi.md#modify_cloud_service) | **PATCH** /v1/inventory/services/{cloudServiceUid} | Modify Cloud Service
+*InventoryApi* | [**modify_device**](docs/InventoryApi.md#modify_device) | **PATCH** /v1/inventory/devices/{deviceUid} | Modify Device
+*InventoryApi* | [**modify_device_manager**](docs/InventoryApi.md#modify_device_manager) | **PATCH** /v1/inventory/managers/{deviceManagerUid} | Modify Device Manager
+*InventoryApi* | [**modify_template_device**](docs/InventoryApi.md#modify_template_device) | **PATCH** /v1/inventory/templates/{templateDeviceUid} | Modify Template Device
+*InventoryApi* | [**onboard_asa_device**](docs/InventoryApi.md#onboard_asa_device) | **POST** /v1/inventory/devices/asas | Onboard ASA device
+*InventoryApi* | [**onboard_ios_device**](docs/InventoryApi.md#onboard_ios_device) | **POST** /v1/inventory/devices/ios | Onboard IOS Device
+*InventoryApi* | [**read_asa_device_configuration**](docs/InventoryApi.md#read_asa_device_configuration) | **POST** /v1/inventory/devices/asas/{deviceUid}/read | Read ASA device configuration
+*InventoryApi* | [**reconnect_asa_device**](docs/InventoryApi.md#reconnect_asa_device) | **POST** /v1/inventory/devices/asas/{deviceUid}/reconnect | Reconnect ASA device
+*MetaApi* | [**get_jwks**](docs/MetaApi.md#get_jwks) | **GET** /.well-known/jwks.json | Fetch JSON Web Key Set
+*MetaApi* | [**get_meta**](docs/MetaApi.md#get_meta) | **GET** /v1/meta | Get Meta information
+*MetaApi* | [**get_regions**](docs/MetaApi.md#get_regions) | **GET** /v1/regions | Get CDO Regions
+*ObjectManagementApi* | [**create_object**](docs/ObjectManagementApi.md#create_object) | **POST** /v0/objects | Create Object
+*ObjectManagementApi* | [**create_targets**](docs/ObjectManagementApi.md#create_targets) | **POST** /v0/objects/{uid}/targets | Create Targets
+*ObjectManagementApi* | [**delete_object**](docs/ObjectManagementApi.md#delete_object) | **DELETE** /v0/objects/{uid} | Delete Object
+*ObjectManagementApi* | [**delete_targets**](docs/ObjectManagementApi.md#delete_targets) | **DELETE** /v0/objects/{uid}/targets | Delete Targets
+*ObjectManagementApi* | [**get_duplicate_objects**](docs/ObjectManagementApi.md#get_duplicate_objects) | **GET** /v0/objects/{uid}/duplicates | Get Duplicate Objects
+*ObjectManagementApi* | [**get_issues_count**](docs/ObjectManagementApi.md#get_issues_count) | **GET** /v0/objects/issues-count | Get Issues Count
+*ObjectManagementApi* | [**get_object**](docs/ObjectManagementApi.md#get_object) | **GET** /v0/objects/{uid} | Get Object
+*ObjectManagementApi* | [**get_object_usages**](docs/ObjectManagementApi.md#get_object_usages) | **GET** /v0/objects/{uid}/usage | Get Object Usages
+*ObjectManagementApi* | [**get_objects**](docs/ObjectManagementApi.md#get_objects) | **GET** /v0/objects | Get Objects
+*ObjectManagementApi* | [**modify_object**](docs/ObjectManagementApi.md#modify_object) | **PATCH** /v0/objects/{uid} | Modify Object
+*RemoteAccessMonitoringApi* | [**get_mfa_event**](docs/RemoteAccessMonitoringApi.md#get_mfa_event) | **GET** /v1/mfaevents/{mfaEventUid} | Get MFA Event
+*RemoteAccessMonitoringApi* | [**get_mfa_events**](docs/RemoteAccessMonitoringApi.md#get_mfa_events) | **GET** /v1/mfaevents | Get MFA Events
+*RemoteAccessMonitoringApi* | [**get_ra_vpn_session**](docs/RemoteAccessMonitoringApi.md#get_ra_vpn_session) | **GET** /v1/vpnsessions/{raVpnSessionUid} | Get RA VPN Session
+*RemoteAccessMonitoringApi* | [**get_ra_vpn_sessions**](docs/RemoteAccessMonitoringApi.md#get_ra_vpn_sessions) | **GET** /v1/vpnsessions | Get RA VPN Sessions
+*RemoteAccessMonitoringApi* | [**refresh_ra_vpn_sessions_by_device**](docs/RemoteAccessMonitoringApi.md#refresh_ra_vpn_sessions_by_device) | **POST** /v1/vpnsessions/refresh | Refresh RA VPN Sessions
+*RemoteAccessMonitoringApi* | [**terminate_ra_vpn_sessions_by_device**](docs/RemoteAccessMonitoringApi.md#terminate_ra_vpn_sessions_by_device) | **POST** /v1/vpnsessions/{deviceUid}/terminate | Terminate RA VPN Sessions
+*RemoteAccessMonitoringApi* | [**terminate_ra_vpn_sessions_by_device_and_user_name**](docs/RemoteAccessMonitoringApi.md#terminate_ra_vpn_sessions_by_device_and_user_name) | **POST** /v1/vpnsessions/{deviceUid}/terminate/{userName} | Terminate User&#39;s RA VPN Sessions
+*SearchApi* | [**initiate_full_indexing**](docs/SearchApi.md#initiate_full_indexing) | **POST** /v1/search/index | Rebuild search index
+*SearchApi* | [**search**](docs/SearchApi.md#search) | **GET** /v1/search | Search
+*TenantManagementApi* | [**add_msp_tenant**](docs/TenantManagementApi.md#add_msp_tenant) | **POST** /v1/msp/tenants | Add Tenant to MSP Portal
+*TenantManagementApi* | [**get_feature_flags**](docs/TenantManagementApi.md#get_feature_flags) | **GET** /v1/features | Get Feature Flags
+*TenantManagementApi* | [**get_tenant**](docs/TenantManagementApi.md#get_tenant) | **GET** /v1/tenants/{tenantUid} | Get Tenant
+*TenantManagementApi* | [**get_tenant_settings**](docs/TenantManagementApi.md#get_tenant_settings) | **GET** /v1/settings/tenant | Get Tenant Settings
+*TenantManagementApi* | [**get_tenants**](docs/TenantManagementApi.md#get_tenants) | **GET** /v1/tenants | Get Tenants
+*TenantManagementApi* | [**modify_tenant_settings**](docs/TenantManagementApi.md#modify_tenant_settings) | **PATCH** /v1/settings/tenant | Modify Tenant Settings
+*TransactionsApi* | [**get_transaction**](docs/TransactionsApi.md#get_transaction) | **GET** /v1/transactions/{transactionUid} | Get Transaction
+*UsersApi* | [**create_user**](docs/UsersApi.md#create_user) | **POST** /v1/users | Create User in CDO Tenant
+*UsersApi* | [**delete_user**](docs/UsersApi.md#delete_user) | **DELETE** /v1/users/{userUid} | Remove User from CDO Tenant
+*UsersApi* | [**generate_api_token**](docs/UsersApi.md#generate_api_token) | **POST** /v1/users/{apiUserId}/apiToken/generate | Generate Token for API-only user
+*UsersApi* | [**get_token**](docs/UsersApi.md#get_token) | **GET** /v1/token | Get Token Info
+*UsersApi* | [**get_user**](docs/UsersApi.md#get_user) | **GET** /v1/users/{userUid} | Get Tenant User
+*UsersApi* | [**get_users**](docs/UsersApi.md#get_users) | **GET** /v1/users | Get Tenant Users
+*UsersApi* | [**revoke_api_token**](docs/UsersApi.md#revoke_api_token) | **POST** /v1/users/{apiUserId}/apiToken/revoke | Revoke API-only User&#39;s Token
+*UsersApi* | [**revoke_token**](docs/UsersApi.md#revoke_token) | **POST** /v1/token/revoke | Revoke Token
 
 
 ## Documentation For Models
 
  - [ApiTokenInfo](docs/ApiTokenInfo.md)
  - [AsaCreateOrUpdateInput](docs/AsaCreateOrUpdateInput.md)
  - [AsaFailoverMate](docs/AsaFailoverMate.md)
  - [AsaFailoverMode](docs/AsaFailoverMode.md)
  - [AuthenticationError](docs/AuthenticationError.md)
+ - [Browser](docs/Browser.md)
  - [CdFmcInfo](docs/CdFmcInfo.md)
  - [CdFmcObject](docs/CdFmcObject.md)
  - [CdFmcResult](docs/CdFmcResult.md)
+ - [CdoCliMacro](docs/CdoCliMacro.md)
+ - [CdoCliMacroPage](docs/CdoCliMacroPage.md)
+ - [CdoCliResult](docs/CdoCliResult.md)
+ - [CdoCliResultPage](docs/CdoCliResultPage.md)
  - [CdoRegion](docs/CdoRegion.md)
  - [CdoRegionList](docs/CdoRegionList.md)
  - [CdoTokenInfo](docs/CdoTokenInfo.md)
  - [CdoTransaction](docs/CdoTransaction.md)
  - [CdoTransactionStatus](docs/CdoTransactionStatus.md)
  - [CdoTransactionType](docs/CdoTransactionType.md)
  - [ChangeRequest](docs/ChangeRequest.md)
  - [ChangeRequestCreateInput](docs/ChangeRequestCreateInput.md)
  - [ChangeRequestPage](docs/ChangeRequestPage.md)
  - [Changelog](docs/Changelog.md)
  - [ChangelogPage](docs/ChangelogPage.md)
+ - [ClientDevice](docs/ClientDevice.md)
  - [CommonApiError](docs/CommonApiError.md)
  - [ConfigState](docs/ConfigState.md)
  - [ConflictDetectionInterval](docs/ConflictDetectionInterval.md)
  - [ConflictDetectionState](docs/ConflictDetectionState.md)
  - [ConnectivityState](docs/ConnectivityState.md)
  - [ConnectorType](docs/ConnectorType.md)
  - [CreateRequest](docs/CreateRequest.md)
  - [Device](docs/Device.md)
  - [DevicePage](docs/DevicePage.md)
  - [DevicePatchInput](docs/DevicePatchInput.md)
  - [DeviceRole](docs/DeviceRole.md)
  - [DuoAdminPanelCreateOrUpdateInput](docs/DuoAdminPanelCreateOrUpdateInput.md)
+ - [DuplicateGroupDto](docs/DuplicateGroupDto.md)
  - [Entity](docs/Entity.md)
  - [EntityType](docs/EntityType.md)
  - [Event](docs/Event.md)
  - [FtdCreateOrUpdateInput](docs/FtdCreateOrUpdateInput.md)
  - [FtdRegistrationInput](docs/FtdRegistrationInput.md)
  - [GlobalSearchResult](docs/GlobalSearchResult.md)
  - [GroupContent](docs/GroupContent.md)
  - [Icmp4Value](docs/Icmp4Value.md)
  - [Icmp6Value](docs/Icmp6Value.md)
  - [Inventory](docs/Inventory.md)
  - [IosCreateOrUpdateInput](docs/IosCreateOrUpdateInput.md)
+ - [IssuesCount](docs/IssuesCount.md)
  - [IssuesDto](docs/IssuesDto.md)
  - [JsonWebKey](docs/JsonWebKey.md)
  - [JwkSet](docs/JwkSet.md)
  - [Labels](docs/Labels.md)
  - [ListObjectResponse](docs/ListObjectResponse.md)
  - [Location](docs/Location.md)
  - [MerakiDeploymentMode](docs/MerakiDeploymentMode.md)
  - [Meta](docs/Meta.md)
+ - [MfaEvent](docs/MfaEvent.md)
+ - [MfaEventPage](docs/MfaEventPage.md)
  - [MspAddTenantInput](docs/MspAddTenantInput.md)
  - [Network](docs/Network.md)
  - [NetworkObjectContent](docs/NetworkObjectContent.md)
  - [OS](docs/OS.md)
  - [ObjectContent](docs/ObjectContent.md)
  - [ObjectResponse](docs/ObjectResponse.md)
  - [OnPremFmcInfo](docs/OnPremFmcInfo.md)
  - [Override](docs/Override.md)
  - [Policy](docs/Policy.md)
  - [PortsValue](docs/PortsValue.md)
+ - [PublicKey](docs/PublicKey.md)
+ - [RaVpnDeviceInput](docs/RaVpnDeviceInput.md)
  - [RaVpnSession](docs/RaVpnSession.md)
  - [RaVpnSessionPage](docs/RaVpnSessionPage.md)
  - [ReferenceInfo](docs/ReferenceInfo.md)
  - [Sdc](docs/Sdc.md)
+ - [SdcCreateInput](docs/SdcCreateInput.md)
  - [SdcPage](docs/SdcPage.md)
- - [SdcPublicKey](docs/SdcPublicKey.md)
- - [SdcStatus](docs/SdcStatus.md)
+ - [SdcPatchInput](docs/SdcPatchInput.md)
  - [ServiceObjectContent](docs/ServiceObjectContent.md)
  - [ServiceObjectValueContent](docs/ServiceObjectValueContent.md)
  - [SharedObjectValue](docs/SharedObjectValue.md)
  - [SingleContent](docs/SingleContent.md)
  - [StateMachineDetails](docs/StateMachineDetails.md)
  - [StateMachineError](docs/StateMachineError.md)
+ - [Status](docs/Status.md)
  - [StatusInfo](docs/StatusInfo.md)
  - [Target](docs/Target.md)
  - [TargetsRequest](docs/TargetsRequest.md)
  - [Tenant](docs/Tenant.md)
  - [TenantPage](docs/TenantPage.md)
  - [TenantPayType](docs/TenantPayType.md)
  - [TenantSettings](docs/TenantSettings.md)
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/__init__.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.9"
+__version__ = "1.0.90"
 
 # import apis into sdk package
 from cdo_sdk_python.api.change_requests_api import ChangeRequestsApi
 from cdo_sdk_python.api.changelogs_api import ChangelogsApi
+from cdo_sdk_python.api.cloud_delivered_fmc_api import CloudDeliveredFMCApi
+from cdo_sdk_python.api.command_line_interface_api import CommandLineInterfaceApi
 from cdo_sdk_python.api.connectors_api import ConnectorsApi
 from cdo_sdk_python.api.inventory_api import InventoryApi
 from cdo_sdk_python.api.meta_api import MetaApi
 from cdo_sdk_python.api.object_management_api import ObjectManagementApi
 from cdo_sdk_python.api.remote_access_monitoring_api import RemoteAccessMonitoringApi
 from cdo_sdk_python.api.search_api import SearchApi
 from cdo_sdk_python.api.tenant_management_api import TenantManagementApi
@@ -43,82 +45,95 @@
 
 # import models into sdk package
 from cdo_sdk_python.models.api_token_info import ApiTokenInfo
 from cdo_sdk_python.models.asa_create_or_update_input import AsaCreateOrUpdateInput
 from cdo_sdk_python.models.asa_failover_mate import AsaFailoverMate
 from cdo_sdk_python.models.asa_failover_mode import AsaFailoverMode
 from cdo_sdk_python.models.authentication_error import AuthenticationError
+from cdo_sdk_python.models.browser import Browser
 from cdo_sdk_python.models.cd_fmc_info import CdFmcInfo
 from cdo_sdk_python.models.cd_fmc_object import CdFmcObject
 from cdo_sdk_python.models.cd_fmc_result import CdFmcResult
+from cdo_sdk_python.models.cdo_cli_macro import CdoCliMacro
+from cdo_sdk_python.models.cdo_cli_macro_page import CdoCliMacroPage
+from cdo_sdk_python.models.cdo_cli_result import CdoCliResult
+from cdo_sdk_python.models.cdo_cli_result_page import CdoCliResultPage
 from cdo_sdk_python.models.cdo_region import CdoRegion
 from cdo_sdk_python.models.cdo_region_list import CdoRegionList
 from cdo_sdk_python.models.cdo_token_info import CdoTokenInfo
 from cdo_sdk_python.models.cdo_transaction import CdoTransaction
 from cdo_sdk_python.models.cdo_transaction_status import CdoTransactionStatus
 from cdo_sdk_python.models.cdo_transaction_type import CdoTransactionType
 from cdo_sdk_python.models.change_request import ChangeRequest
 from cdo_sdk_python.models.change_request_create_input import ChangeRequestCreateInput
 from cdo_sdk_python.models.change_request_page import ChangeRequestPage
 from cdo_sdk_python.models.changelog import Changelog
 from cdo_sdk_python.models.changelog_page import ChangelogPage
+from cdo_sdk_python.models.client_device import ClientDevice
 from cdo_sdk_python.models.common_api_error import CommonApiError
 from cdo_sdk_python.models.config_state import ConfigState
 from cdo_sdk_python.models.conflict_detection_interval import ConflictDetectionInterval
 from cdo_sdk_python.models.conflict_detection_state import ConflictDetectionState
 from cdo_sdk_python.models.connectivity_state import ConnectivityState
 from cdo_sdk_python.models.connector_type import ConnectorType
 from cdo_sdk_python.models.create_request import CreateRequest
 from cdo_sdk_python.models.device import Device
 from cdo_sdk_python.models.device_page import DevicePage
 from cdo_sdk_python.models.device_patch_input import DevicePatchInput
 from cdo_sdk_python.models.device_role import DeviceRole
 from cdo_sdk_python.models.duo_admin_panel_create_or_update_input import DuoAdminPanelCreateOrUpdateInput
+from cdo_sdk_python.models.duplicate_group_dto import DuplicateGroupDto
 from cdo_sdk_python.models.entity import Entity
 from cdo_sdk_python.models.entity_type import EntityType
 from cdo_sdk_python.models.event import Event
 from cdo_sdk_python.models.ftd_create_or_update_input import FtdCreateOrUpdateInput
 from cdo_sdk_python.models.ftd_registration_input import FtdRegistrationInput
 from cdo_sdk_python.models.global_search_result import GlobalSearchResult
 from cdo_sdk_python.models.group_content import GroupContent
 from cdo_sdk_python.models.icmp4_value import Icmp4Value
 from cdo_sdk_python.models.icmp6_value import Icmp6Value
 from cdo_sdk_python.models.inventory import Inventory
 from cdo_sdk_python.models.ios_create_or_update_input import IosCreateOrUpdateInput
+from cdo_sdk_python.models.issues_count import IssuesCount
 from cdo_sdk_python.models.issues_dto import IssuesDto
 from cdo_sdk_python.models.json_web_key import JsonWebKey
 from cdo_sdk_python.models.jwk_set import JwkSet
 from cdo_sdk_python.models.labels import Labels
 from cdo_sdk_python.models.list_object_response import ListObjectResponse
 from cdo_sdk_python.models.location import Location
 from cdo_sdk_python.models.meraki_deployment_mode import MerakiDeploymentMode
 from cdo_sdk_python.models.meta import Meta
+from cdo_sdk_python.models.mfa_event import MfaEvent
+from cdo_sdk_python.models.mfa_event_page import MfaEventPage
 from cdo_sdk_python.models.msp_add_tenant_input import MspAddTenantInput
 from cdo_sdk_python.models.network import Network
 from cdo_sdk_python.models.network_object_content import NetworkObjectContent
 from cdo_sdk_python.models.os import OS
 from cdo_sdk_python.models.object_content import ObjectContent
 from cdo_sdk_python.models.object_response import ObjectResponse
 from cdo_sdk_python.models.on_prem_fmc_info import OnPremFmcInfo
 from cdo_sdk_python.models.override import Override
 from cdo_sdk_python.models.policy import Policy
 from cdo_sdk_python.models.ports_value import PortsValue
+from cdo_sdk_python.models.public_key import PublicKey
+from cdo_sdk_python.models.ra_vpn_device_input import RaVpnDeviceInput
 from cdo_sdk_python.models.ra_vpn_session import RaVpnSession
 from cdo_sdk_python.models.ra_vpn_session_page import RaVpnSessionPage
 from cdo_sdk_python.models.reference_info import ReferenceInfo
 from cdo_sdk_python.models.sdc import Sdc
+from cdo_sdk_python.models.sdc_create_input import SdcCreateInput
 from cdo_sdk_python.models.sdc_page import SdcPage
-from cdo_sdk_python.models.sdc_public_key import SdcPublicKey
-from cdo_sdk_python.models.sdc_status import SdcStatus
+from cdo_sdk_python.models.sdc_patch_input import SdcPatchInput
 from cdo_sdk_python.models.service_object_content import ServiceObjectContent
 from cdo_sdk_python.models.service_object_value_content import ServiceObjectValueContent
 from cdo_sdk_python.models.shared_object_value import SharedObjectValue
 from cdo_sdk_python.models.single_content import SingleContent
 from cdo_sdk_python.models.state_machine_details import StateMachineDetails
 from cdo_sdk_python.models.state_machine_error import StateMachineError
+from cdo_sdk_python.models.status import Status
 from cdo_sdk_python.models.status_info import StatusInfo
 from cdo_sdk_python.models.target import Target
 from cdo_sdk_python.models.targets_request import TargetsRequest
 from cdo_sdk_python.models.tenant import Tenant
 from cdo_sdk_python.models.tenant_page import TenantPage
 from cdo_sdk_python.models.tenant_pay_type import TenantPayType
 from cdo_sdk_python.models.tenant_settings import TenantSettings
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/__init__.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # flake8: noqa
 
 # import apis into api package
 from cdo_sdk_python.api.change_requests_api import ChangeRequestsApi
 from cdo_sdk_python.api.changelogs_api import ChangelogsApi
+from cdo_sdk_python.api.cloud_delivered_fmc_api import CloudDeliveredFMCApi
+from cdo_sdk_python.api.command_line_interface_api import CommandLineInterfaceApi
 from cdo_sdk_python.api.connectors_api import ConnectorsApi
 from cdo_sdk_python.api.inventory_api import InventoryApi
 from cdo_sdk_python.api.meta_api import MetaApi
 from cdo_sdk_python.api.object_management_api import ObjectManagementApi
 from cdo_sdk_python.api.remote_access_monitoring_api import RemoteAccessMonitoringApi
 from cdo_sdk_python.api.search_api import SearchApi
 from cdo_sdk_python.api.tenant_management_api import TenantManagementApi
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/change_requests_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/change_requests_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -55,16 +55,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ChangeRequest:
-        """Create Change Requests.
+        """Create Change Request
 
+        Create a Change Request in the CDO tenant.
 
         :param change_request_create_input: (required)
         :type change_request_create_input: ChangeRequestCreateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -126,16 +127,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[ChangeRequest]:
-        """Create Change Requests.
+        """Create Change Request
 
+        Create a Change Request in the CDO tenant.
 
         :param change_request_create_input: (required)
         :type change_request_create_input: ChangeRequestCreateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -197,16 +199,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create Change Requests.
+        """Create Change Request
 
+        Create a Change Request in the CDO tenant.
 
         :param change_request_create_input: (required)
         :type change_request_create_input: ChangeRequestCreateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -338,16 +341,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Delete a Change Request by UID in the CDO tenant
+        """Delete Change Request
 
+        Delete a Change Request by UID in the CDO tenant.
 
         :param change_request_uid: The unique identifier of the Change Request in CDO. (required)
         :type change_request_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -409,16 +413,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Delete a Change Request by UID in the CDO tenant
+        """Delete Change Request
 
+        Delete a Change Request by UID in the CDO tenant.
 
         :param change_request_uid: The unique identifier of the Change Request in CDO. (required)
         :type change_request_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -480,16 +485,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a Change Request by UID in the CDO tenant
+        """Delete Change Request
 
+        Delete a Change Request by UID in the CDO tenant.
 
         :param change_request_uid: The unique identifier of the Change Request in CDO. (required)
         :type change_request_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -608,16 +614,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ChangeRequest:
-        """Fetch a Change Request by UID in the CDO tenant.
+        """Get Change Request
 
+        Get a Change Request by UID in the CDO tenant.
 
         :param change_request_uid: The unique identifier of the Change Request in CDO. (required)
         :type change_request_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -680,16 +687,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[ChangeRequest]:
-        """Fetch a Change Request by UID in the CDO tenant.
+        """Get Change Request
 
+        Get a Change Request by UID in the CDO tenant.
 
         :param change_request_uid: The unique identifier of the Change Request in CDO. (required)
         :type change_request_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -752,16 +760,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a Change Request by UID in the CDO tenant.
+        """Get Change Request
 
+        Get a Change Request by UID in the CDO tenant.
 
         :param change_request_uid: The unique identifier of the Change Request in CDO. (required)
         :type change_request_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -865,38 +874,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_change_requests(
+    def get_change_requests(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ChangeRequestPage:
-        """Fetch a list of Change Requests.
+        """Get Change Requests
 
+        Get a list of Change Requests.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -914,15 +924,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_change_requests_serialize(
+        _param = self._get_change_requests_serialize(
             limit=limit,
             offset=offset,
             q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -944,38 +954,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_change_requests_with_http_info(
+    def get_change_requests_with_http_info(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[ChangeRequestPage]:
-        """Fetch a list of Change Requests.
+        """Get Change Requests
 
+        Get a list of Change Requests.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -993,15 +1004,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_change_requests_serialize(
+        _param = self._get_change_requests_serialize(
             limit=limit,
             offset=offset,
             q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -1023,38 +1034,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_change_requests_without_preload_content(
+    def get_change_requests_without_preload_content(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of Change Requests.
+        """Get Change Requests
 
+        Get a list of Change Requests.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1072,15 +1084,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_change_requests_serialize(
+        _param = self._get_change_requests_serialize(
             limit=limit,
             offset=offset,
             q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
@@ -1097,15 +1109,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_change_requests_serialize(
+    def _get_change_requests_serialize(
         self,
         limit,
         offset,
         q,
         _request_auth,
         _content_type,
         _headers,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/changelogs_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/changelogs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -54,16 +54,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Changelog:
-        """Fetch a Change Log by UID in the CDO tenant.
+        """Get Change Log
 
+        Get a specific Change Log object by UID in the CDO tenant.
 
         :param changelog_uid: The unique identifier of the changelog in CDO. (required)
         :type changelog_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -125,16 +126,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Changelog]:
-        """Fetch a Change Log by UID in the CDO tenant.
+        """Get Change Log
 
+        Get a specific Change Log object by UID in the CDO tenant.
 
         :param changelog_uid: The unique identifier of the changelog in CDO. (required)
         :type changelog_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -196,16 +198,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a Change Log by UID in the CDO tenant.
+        """Get Change Log
 
+        Get a specific Change Log object by UID in the CDO tenant.
 
         :param changelog_uid: The unique identifier of the changelog in CDO. (required)
         :type changelog_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -308,18 +311,18 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_changelogs(
+    def get_changelogs(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         search_text: Annotated[Optional[StrictStr], Field(description="The searchText parameter serves as a flexible search option that allows for text-based filtering across all fields of the Change Log object. This parameter can be used independently to search for entries containing the specified text, or in combination with the q query parameter for more targeted results. When used with q, the search conditions of searchText are logically ANDed with the q parameter's criteria, ensuring that the returned entries satisfy both sets of conditions.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -327,20 +330,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ChangelogPage:
-        """Fetch a list of Change Logs.
+        """Get Change Logs
 
+        Get a list of Change Logs in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param search_text: The searchText parameter serves as a flexible search option that allows for text-based filtering across all fields of the Change Log object. This parameter can be used independently to search for entries containing the specified text, or in combination with the q query parameter for more targeted results. When used with q, the search conditions of searchText are logically ANDed with the q parameter's criteria, ensuring that the returned entries satisfy both sets of conditions.
         :type search_text: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -360,15 +364,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_changelogs_serialize(
+        _param = self._get_changelogs_serialize(
             limit=limit,
             offset=offset,
             search_text=search_text,
             q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -391,18 +395,18 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_changelogs_with_http_info(
+    def get_changelogs_with_http_info(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         search_text: Annotated[Optional[StrictStr], Field(description="The searchText parameter serves as a flexible search option that allows for text-based filtering across all fields of the Change Log object. This parameter can be used independently to search for entries containing the specified text, or in combination with the q query parameter for more targeted results. When used with q, the search conditions of searchText are logically ANDed with the q parameter's criteria, ensuring that the returned entries satisfy both sets of conditions.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -410,20 +414,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[ChangelogPage]:
-        """Fetch a list of Change Logs.
+        """Get Change Logs
 
+        Get a list of Change Logs in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param search_text: The searchText parameter serves as a flexible search option that allows for text-based filtering across all fields of the Change Log object. This parameter can be used independently to search for entries containing the specified text, or in combination with the q query parameter for more targeted results. When used with q, the search conditions of searchText are logically ANDed with the q parameter's criteria, ensuring that the returned entries satisfy both sets of conditions.
         :type search_text: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -443,15 +448,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_changelogs_serialize(
+        _param = self._get_changelogs_serialize(
             limit=limit,
             offset=offset,
             search_text=search_text,
             q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -474,18 +479,18 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_changelogs_without_preload_content(
+    def get_changelogs_without_preload_content(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         search_text: Annotated[Optional[StrictStr], Field(description="The searchText parameter serves as a flexible search option that allows for text-based filtering across all fields of the Change Log object. This parameter can be used independently to search for entries containing the specified text, or in combination with the q query parameter for more targeted results. When used with q, the search conditions of searchText are logically ANDed with the q parameter's criteria, ensuring that the returned entries satisfy both sets of conditions.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -493,20 +498,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of Change Logs.
+        """Get Change Logs
 
+        Get a list of Change Logs in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param search_text: The searchText parameter serves as a flexible search option that allows for text-based filtering across all fields of the Change Log object. This parameter can be used independently to search for entries containing the specified text, or in combination with the q query parameter for more targeted results. When used with q, the search conditions of searchText are logically ANDed with the q parameter's criteria, ensuring that the returned entries satisfy both sets of conditions.
         :type search_text: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -526,15 +532,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_changelogs_serialize(
+        _param = self._get_changelogs_serialize(
             limit=limit,
             offset=offset,
             search_text=search_text,
             q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -552,15 +558,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_changelogs_serialize(
+    def _get_changelogs_serialize(
         self,
         limit,
         offset,
         search_text,
         q,
         _request_auth,
         _content_type,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/connectors_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/search_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,68 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr
-from typing import List, Optional
-from typing_extensions import Annotated
-from cdo_sdk_python.models.sdc import Sdc
-from cdo_sdk_python.models.sdc_page import SdcPage
+from pydantic import StrictStr
+from cdo_sdk_python.models.cdo_transaction import CdoTransaction
+from cdo_sdk_python.models.global_search_result import GlobalSearchResult
 
 from cdo_sdk_python.api_client import ApiClient, RequestSerialized
 from cdo_sdk_python.api_response import ApiResponse
 from cdo_sdk_python.rest import RESTResponseType
 
 
-class ConnectorsApi:
+class SearchApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def fetch_sdc(
+    def initiate_full_indexing(
         self,
-        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Sdc:
-        """Fetch a SDC by UID in the CDO tenant
+    ) -> CdoTransaction:
+        """Rebuild search index
 
+        Initiate Full Indexing on the CDO tenant, to improve accuracy of search results. This operation is performed automatically on a schedule by CDO, but can be triggered on demand too. This operation is asynchronous, but its progress cannot be tracked using CDO's API.
 
-        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
-        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -81,63 +77,60 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._fetch_sdc_serialize(
-            sdc_uid=sdc_uid,
+        _param = self._initiate_full_indexing_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Sdc",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def fetch_sdc_with_http_info(
+    def initiate_full_indexing_with_http_info(
         self,
-        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Sdc]:
-        """Fetch a SDC by UID in the CDO tenant
+    ) -> ApiResponse[CdoTransaction]:
+        """Rebuild search index
 
+        Initiate Full Indexing on the CDO tenant, to improve accuracy of search results. This operation is performed automatically on a schedule by CDO, but can be triggered on demand too. This operation is asynchronous, but its progress cannot be tracked using CDO's API.
 
-        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
-        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -152,63 +145,60 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._fetch_sdc_serialize(
-            sdc_uid=sdc_uid,
+        _param = self._initiate_full_indexing_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Sdc",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def fetch_sdc_without_preload_content(
+    def initiate_full_indexing_without_preload_content(
         self,
-        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a SDC by UID in the CDO tenant
+        """Rebuild search index
 
+        Initiate Full Indexing on the CDO tenant, to improve accuracy of search results. This operation is performed automatically on a schedule by CDO, but can be triggered on demand too. This operation is asynchronous, but its progress cannot be tracked using CDO's API.
 
-        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
-        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -223,40 +213,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._fetch_sdc_serialize(
-            sdc_uid=sdc_uid,
+        _param = self._initiate_full_indexing_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Sdc",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _fetch_sdc_serialize(
+    def _initiate_full_indexing_serialize(
         self,
-        sdc_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -268,16 +256,14 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if sdc_uid is not None:
-            _path_params['sdcUid'] = sdc_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -290,16 +276,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/v1/connectors/sdcs/{sdcUid}',
+            method='POST',
+            resource_path='/v1/search/index',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -308,44 +294,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_sdcs(
+    def search(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
+        q: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> SdcPage:
-        """Fetch a list of SDCs in the CDO tenant
+    ) -> GlobalSearchResult:
+        """Search
 
+        Search for devices, services, managers, objects and policies across the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :param q: (required)
         :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -360,74 +338,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_sdcs_serialize(
-            limit=limit,
-            offset=offset,
+        _param = self._search_serialize(
             q=q,
-            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SdcPage",
+            '200': "GlobalSearchResult",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_sdcs_with_http_info(
+    def search_with_http_info(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
+        q: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[SdcPage]:
-        """Fetch a list of SDCs in the CDO tenant
+    ) -> ApiResponse[GlobalSearchResult]:
+        """Search
 
+        Search for devices, services, managers, objects and policies across the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :param q: (required)
         :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -442,74 +410,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_sdcs_serialize(
-            limit=limit,
-            offset=offset,
+        _param = self._search_serialize(
             q=q,
-            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SdcPage",
+            '200': "GlobalSearchResult",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_sdcs_without_preload_content(
+    def search_without_preload_content(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
+        q: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of SDCs in the CDO tenant
+        """Search
 
+        Search for devices, services, managers, objects and policies across the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :param q: (required)
         :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -524,82 +482,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_sdcs_serialize(
-            limit=limit,
-            offset=offset,
+        _param = self._search_serialize(
             q=q,
-            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "SdcPage",
+            '200': "GlobalSearchResult",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_sdcs_serialize(
+    def _search_serialize(
         self,
-        limit,
-        offset,
         q,
-        sort,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if limit is not None:
-            
-            _query_params.append(('limit', limit))
-            
-        if offset is not None:
-            
-            _query_params.append(('offset', offset))
-            
         if q is not None:
             
             _query_params.append(('q', q))
             
-        if sort is not None:
-            
-            _query_params.append(('sort', sort))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -612,15 +552,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/connectors/sdcs',
+            resource_path='/v1/search',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/inventory_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/inventory_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -61,17 +61,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Onboard a Duo Admin Panel in the CDO tenant
+        """Onboard Duo Admin Panel
 
-        Onboard a Duo Admin Panel to the CDO tenant. The credentials to onboard the Duo Admin Panel to CDO must be generated by creating an Admin API application on https://www.duo.com
+        Onboard a Duo Admin Panel to the CDO tenant. The credentials to onboard the Duo Admin Panel to CDO must be generated by creating an Admin API application on https://www.duo.com. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param duo_admin_panel_create_or_update_input: (required)
         :type duo_admin_panel_create_or_update_input: DuoAdminPanelCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -132,17 +132,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Onboard a Duo Admin Panel in the CDO tenant
+        """Onboard Duo Admin Panel
 
-        Onboard a Duo Admin Panel to the CDO tenant. The credentials to onboard the Duo Admin Panel to CDO must be generated by creating an Admin API application on https://www.duo.com
+        Onboard a Duo Admin Panel to the CDO tenant. The credentials to onboard the Duo Admin Panel to CDO must be generated by creating an Admin API application on https://www.duo.com. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param duo_admin_panel_create_or_update_input: (required)
         :type duo_admin_panel_create_or_update_input: DuoAdminPanelCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -203,17 +203,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Onboard a Duo Admin Panel in the CDO tenant
+        """Onboard Duo Admin Panel
 
-        Onboard a Duo Admin Panel to the CDO tenant. The credentials to onboard the Duo Admin Panel to CDO must be generated by creating an Admin API application on https://www.duo.com
+        Onboard a Duo Admin Panel to the CDO tenant. The credentials to onboard the Duo Admin Panel to CDO must be generated by creating an Admin API application on https://www.duo.com. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param duo_admin_panel_create_or_update_input: (required)
         :type duo_admin_panel_create_or_update_input: DuoAdminPanelCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -344,16 +344,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Create an FTD device in the CDO tenant
+        """Create FTD device.
 
+        This is an asynchronous operation to create a cdFMC managed FTD device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation. Onboarding a cdFMC managed FTD device is a two-step process: the first step, handled by this operation, creates an FTD device with a configure manager string that must be pasted into the FTD device's Command-Line Interface. The FTD then uses this information to register itself with the CDO tenant.
 
         :param ftd_create_or_update_input: (required)
         :type ftd_create_or_update_input: FtdCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -414,16 +415,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Create an FTD device in the CDO tenant
+        """Create FTD device.
 
+        This is an asynchronous operation to create a cdFMC managed FTD device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation. Onboarding a cdFMC managed FTD device is a two-step process: the first step, handled by this operation, creates an FTD device with a configure manager string that must be pasted into the FTD device's Command-Line Interface. The FTD then uses this information to register itself with the CDO tenant.
 
         :param ftd_create_or_update_input: (required)
         :type ftd_create_or_update_input: FtdCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -484,16 +486,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create an FTD device in the CDO tenant
+        """Create FTD device.
 
+        This is an asynchronous operation to create a cdFMC managed FTD device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation. Onboarding a cdFMC managed FTD device is a two-step process: the first step, handled by this operation, creates an FTD device with a configure manager string that must be pasted into the FTD device's Command-Line Interface. The FTD then uses this information to register itself with the CDO tenant.
 
         :param ftd_create_or_update_input: (required)
         :type ftd_create_or_update_input: FtdCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -624,16 +627,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Delete cdFMC managed FTD device in the CDO tenant
+        """Delete cdFMC managed FTD device
 
+        This is an asynchronous operation to delete cdFMC managed FTD device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation. The reason this operation is asynchronous is because the device is first removed from the cdFMC, following which it is deleted from the CDO tenant.
 
         :param device_uid: The unique identifier of the cdFMC managed FTD device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -694,16 +698,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Delete cdFMC managed FTD device in the CDO tenant
+        """Delete cdFMC managed FTD device
 
+        This is an asynchronous operation to delete cdFMC managed FTD device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation. The reason this operation is asynchronous is because the device is first removed from the cdFMC, following which it is deleted from the CDO tenant.
 
         :param device_uid: The unique identifier of the cdFMC managed FTD device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -764,16 +769,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete cdFMC managed FTD device in the CDO tenant
+        """Delete cdFMC managed FTD device
 
+        This is an asynchronous operation to delete cdFMC managed FTD device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation. The reason this operation is asynchronous is because the device is first removed from the cdFMC, following which it is deleted from the CDO tenant.
 
         :param device_uid: The unique identifier of the cdFMC managed FTD device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -891,16 +897,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Delete a Cloud Service by UID in the CDO tenant
+        """Delete Cloud Service
 
+        Delete a Cloud Service by UID in the CDO tenant.
 
         :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
         :type cloud_service_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -961,16 +968,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Delete a Cloud Service by UID in the CDO tenant
+        """Delete Cloud Service
 
+        Delete a Cloud Service by UID in the CDO tenant.
 
         :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
         :type cloud_service_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1031,16 +1039,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a Cloud Service by UID in the CDO tenant
+        """Delete Cloud Service
 
+        Delete a Cloud Service by UID in the CDO tenant.
 
         :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
         :type cloud_service_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1158,16 +1167,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Delete a device by UID in the CDO tenant
+        """Delete Device
 
+        Delete a device by UID in the CDO tenant
 
         :param device_uid: The unique identifier of the device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1229,16 +1239,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Delete a device by UID in the CDO tenant
+        """Delete Device
 
+        Delete a device by UID in the CDO tenant
 
         :param device_uid: The unique identifier of the device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1300,16 +1311,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a device by UID in the CDO tenant
+        """Delete Device
 
+        Delete a device by UID in the CDO tenant
 
         :param device_uid: The unique identifier of the device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1428,16 +1440,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Delete a Device Manager by UID in the CDO tenant
+        """Delete Device Manager
 
+        Delete a Device Manager by UID in the CDO tenant.
 
         :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
         :type device_manager_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1499,16 +1512,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Delete a Device Manager by UID in the CDO tenant
+        """Delete Device Manager
 
+        Delete a Device Manager by UID in the CDO tenant.
 
         :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
         :type device_manager_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1570,16 +1584,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a Device Manager by UID in the CDO tenant
+        """Delete Device Manager
 
+        Delete a Device Manager by UID in the CDO tenant.
 
         :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
         :type device_manager_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1698,16 +1713,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """Delete a template device by UID in the CDO tenant
+        """Delete Template Device
 
+        Delete a template device by UID in the CDO tenant.
 
         :param template_device_uid: The unique identifier of the template device in CDO. (required)
         :type template_device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1768,16 +1784,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """Delete a template device by UID in the CDO tenant
+        """Delete Template Device
 
+        Delete a template device by UID in the CDO tenant.
 
         :param template_device_uid: The unique identifier of the template device in CDO. (required)
         :type template_device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1838,16 +1855,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a template device by UID in the CDO tenant
+        """Delete Template Device
 
+        Delete a template device by UID in the CDO tenant.
 
         :param template_device_uid: The unique identifier of the template device in CDO. (required)
         :type template_device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1965,16 +1983,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Deploy changes to an ASA device in the CDO tenant
+        """Deploy ASA device changes
 
+        This is an asynchronous operation to deploy changes made to an ASA device's configuration on CDO to the device. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2036,16 +2055,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Deploy changes to an ASA device in the CDO tenant
+        """Deploy ASA device changes
 
+        This is an asynchronous operation to deploy changes made to an ASA device's configuration on CDO to the device. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2107,16 +2127,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Deploy changes to an ASA device in the CDO tenant
+        """Deploy ASA device changes
 
+        This is an asynchronous operation to deploy changes made to an ASA device's configuration on CDO to the device. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2235,16 +2256,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Register an FTD device managed by an FMC to the CDO tenant. Call this API endpoint after you have created an FTD, and pasted the generated CLI output in the FTD
+        """Register FTD device.
 
+        Complete registration of an FTD device managed by an FMC to the CDO tenant. Call this API endpoint after you have created an FTD and pasted the generated CLI output in the FTD. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param ftd_registration_input: (required)
         :type ftd_registration_input: FtdRegistrationInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2305,16 +2327,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Register an FTD device managed by an FMC to the CDO tenant. Call this API endpoint after you have created an FTD, and pasted the generated CLI output in the FTD
+        """Register FTD device.
 
+        Complete registration of an FTD device managed by an FMC to the CDO tenant. Call this API endpoint after you have created an FTD and pasted the generated CLI output in the FTD. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param ftd_registration_input: (required)
         :type ftd_registration_input: FtdRegistrationInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2375,16 +2398,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Register an FTD device managed by an FMC to the CDO tenant. Call this API endpoint after you have created an FTD, and pasted the generated CLI output in the FTD
+        """Register FTD device.
 
+        Complete registration of an FTD device managed by an FMC to the CDO tenant. Call this API endpoint after you have created an FTD and pasted the generated CLI output in the FTD. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param ftd_registration_input: (required)
         :type ftd_registration_input: FtdRegistrationInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2515,16 +2539,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Device:
-        """Fetch a Cloud Service by UID in the CDO tenant
+        """Get Cloud Service
 
+        Get a Cloud Service by UID in the CDO tenant.
 
         :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
         :type cloud_service_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2586,16 +2611,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Device]:
-        """Fetch a Cloud Service by UID in the CDO tenant
+        """Get Cloud Service
 
+        Get a Cloud Service by UID in the CDO tenant.
 
         :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
         :type cloud_service_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2657,16 +2683,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a Cloud Service by UID in the CDO tenant
+        """Get Cloud Service
 
+        Get a Cloud Service by UID in the CDO tenant.
 
         :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
         :type cloud_service_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2769,35 +2796,45 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_device(
+    def get_cloud_services(
         self,
-        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Device:
-        """Fetch a device by UID in the CDO tenant
+    ) -> DevicePage:
+        """Get Cloud Services
 
+        Get a list of Cloud Services in the CDO tenant.
 
-        :param device_uid: The unique identifier of the device in CDO. (required)
-        :type device_uid: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param sort: The fields to sort results by.
+        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2812,64 +2849,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_device_serialize(
-            device_uid=device_uid,
+        _param = self._get_cloud_services_serialize(
+            limit=limit,
+            offset=offset,
+            q=q,
+            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '200': "DevicePage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_device_with_http_info(
+    def get_cloud_services_with_http_info(
         self,
-        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Device]:
-        """Fetch a device by UID in the CDO tenant
+    ) -> ApiResponse[DevicePage]:
+        """Get Cloud Services
 
+        Get a list of Cloud Services in the CDO tenant.
 
-        :param device_uid: The unique identifier of the device in CDO. (required)
-        :type device_uid: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param sort: The fields to sort results by.
+        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2884,64 +2932,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_device_serialize(
-            device_uid=device_uid,
+        _param = self._get_cloud_services_serialize(
+            limit=limit,
+            offset=offset,
+            q=q,
+            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '200': "DevicePage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_device_without_preload_content(
+    def get_cloud_services_without_preload_content(
         self,
-        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a device by UID in the CDO tenant
+        """Get Cloud Services
 
+        Get a list of Cloud Services in the CDO tenant.
 
-        :param device_uid: The unique identifier of the device in CDO. (required)
-        :type device_uid: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param sort: The fields to sort results by.
+        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2956,63 +3015,82 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_device_serialize(
-            device_uid=device_uid,
+        _param = self._get_cloud_services_serialize(
+            limit=limit,
+            offset=offset,
+            q=q,
+            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '200': "DevicePage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_device_serialize(
+    def _get_cloud_services_serialize(
         self,
-        device_uid,
+        limit,
+        offset,
+        q,
+        sort,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
+            'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if device_uid is not None:
-            _path_params['deviceUid'] = device_uid
         # process the query parameters
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if offset is not None:
+            
+            _query_params.append(('offset', offset))
+            
+        if q is not None:
+            
+            _query_params.append(('q', q))
+            
+        if sort is not None:
+            
+            _query_params.append(('sort', sort))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -3025,15 +3103,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/inventory/devices/{deviceUid}',
+            resource_path='/v1/inventory/services',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3042,35 +3120,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_device_manager(
+    def get_device(
         self,
-        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
+        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Device:
-        """Fetch a Device Manager by UID in the CDO tenant
+        """Get Device
 
+        Get a device by UID in the CDO tenant
 
-        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
-        :type device_manager_uid: str
+        :param device_uid: The unique identifier of the device in CDO. (required)
+        :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3085,63 +3164,65 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_device_manager_serialize(
-            device_manager_uid=device_manager_uid,
+        _param = self._get_device_serialize(
+            device_uid=device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_device_manager_with_http_info(
+    def get_device_with_http_info(
         self,
-        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
+        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Device]:
-        """Fetch a Device Manager by UID in the CDO tenant
+        """Get Device
 
+        Get a device by UID in the CDO tenant
 
-        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
-        :type device_manager_uid: str
+        :param device_uid: The unique identifier of the device in CDO. (required)
+        :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3156,63 +3237,65 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_device_manager_serialize(
-            device_manager_uid=device_manager_uid,
+        _param = self._get_device_serialize(
+            device_uid=device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_device_manager_without_preload_content(
+    def get_device_without_preload_content(
         self,
-        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
+        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a Device Manager by UID in the CDO tenant
+        """Get Device
 
+        Get a device by UID in the CDO tenant
 
-        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
-        :type device_manager_uid: str
+        :param device_uid: The unique identifier of the device in CDO. (required)
+        :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3227,40 +3310,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_device_manager_serialize(
-            device_manager_uid=device_manager_uid,
+        _param = self._get_device_serialize(
+            device_uid=device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_device_manager_serialize(
+    def _get_device_serialize(
         self,
-        device_manager_uid,
+        device_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -3272,16 +3356,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if device_manager_uid is not None:
-            _path_params['deviceManagerUid'] = device_manager_uid
+        if device_uid is not None:
+            _path_params['deviceUid'] = device_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -3295,15 +3379,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/inventory/managers/{deviceManagerUid}',
+            resource_path='/v1/inventory/devices/{deviceUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3312,35 +3396,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_template_device(
+    def get_device_manager(
         self,
-        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
+        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Device:
-        """Fetch a template device by UID in the CDO tenant
+        """Get Device Manager
 
+        Get a Device Manager by UID in the CDO tenant.
 
-        :param template_device_uid: The unique identifier of the template device in CDO. (required)
-        :type template_device_uid: str
+        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
+        :type device_manager_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3355,16 +3440,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_template_device_serialize(
-            template_device_uid=template_device_uid,
+        _param = self._get_device_manager_serialize(
+            device_manager_uid=device_manager_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3383,35 +3468,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_template_device_with_http_info(
+    def get_device_manager_with_http_info(
         self,
-        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
+        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Device]:
-        """Fetch a template device by UID in the CDO tenant
+        """Get Device Manager
 
+        Get a Device Manager by UID in the CDO tenant.
 
-        :param template_device_uid: The unique identifier of the template device in CDO. (required)
-        :type template_device_uid: str
+        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
+        :type device_manager_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3426,16 +3512,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_template_device_serialize(
-            template_device_uid=template_device_uid,
+        _param = self._get_device_manager_serialize(
+            device_manager_uid=device_manager_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3454,35 +3540,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_template_device_without_preload_content(
+    def get_device_manager_without_preload_content(
         self,
-        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
+        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a template device by UID in the CDO tenant
+        """Get Device Manager
 
+        Get a Device Manager by UID in the CDO tenant.
 
-        :param template_device_uid: The unique identifier of the template device in CDO. (required)
-        :type template_device_uid: str
+        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
+        :type device_manager_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3497,16 +3584,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_template_device_serialize(
-            template_device_uid=template_device_uid,
+        _param = self._get_device_manager_serialize(
+            device_manager_uid=device_manager_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3520,17 +3607,17 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_template_device_serialize(
+    def _get_device_manager_serialize(
         self,
-        template_device_uid,
+        device_manager_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -3542,16 +3629,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if template_device_uid is not None:
-            _path_params['templateDeviceUid'] = template_device_uid
+        if device_manager_uid is not None:
+            _path_params['deviceManagerUid'] = device_manager_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -3565,15 +3652,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/inventory/templates/{templateDeviceUid}',
+            resource_path='/v1/inventory/managers/{deviceManagerUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3582,18 +3669,18 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_device_cloud_services(
+    def get_device_managers(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -3601,20 +3688,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> DevicePage:
-        """Fetch a list of Cloud Services in the CDO tenant
+        """Get Device Managers
 
+        Fetch a list of Device Managers (on-prem FMCs and cloud-delivered FMCs) in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -3634,15 +3722,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_device_cloud_services_serialize(
+        _param = self._get_device_managers_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -3664,18 +3752,18 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_device_cloud_services_with_http_info(
+    def get_device_managers_with_http_info(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -3683,20 +3771,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[DevicePage]:
-        """Fetch a list of Cloud Services in the CDO tenant
+        """Get Device Managers
 
+        Fetch a list of Device Managers (on-prem FMCs and cloud-delivered FMCs) in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -3716,15 +3805,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_device_cloud_services_serialize(
+        _param = self._get_device_managers_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -3746,18 +3835,18 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_device_cloud_services_without_preload_content(
+    def get_device_managers_without_preload_content(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -3765,20 +3854,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of Cloud Services in the CDO tenant
+        """Get Device Managers
 
+        Fetch a list of Device Managers (on-prem FMCs and cloud-delivered FMCs) in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -3798,15 +3888,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_device_cloud_services_serialize(
+        _param = self._get_device_managers_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -3823,15 +3913,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_device_cloud_services_serialize(
+    def _get_device_managers_serialize(
         self,
         limit,
         offset,
         q,
         sort,
         _request_auth,
         _content_type,
@@ -3886,15 +3976,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/inventory/services',
+            resource_path='/v1/inventory/managers',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3903,18 +3993,18 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_device_managers(
+    def get_devices(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -3922,20 +4012,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> DevicePage:
-        """Fetch a list of Device Managers (on-prem FMCs and cloud-delivered FMCs) in the CDO tenant
+        """Get Devices
 
+        Get a list of devices in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -3955,15 +4046,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_device_managers_serialize(
+        _param = self._get_devices_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -3971,32 +4062,33 @@
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "DevicePage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_device_managers_with_http_info(
+    def get_devices_with_http_info(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -4004,20 +4096,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[DevicePage]:
-        """Fetch a list of Device Managers (on-prem FMCs and cloud-delivered FMCs) in the CDO tenant
+        """Get Devices
 
+        Get a list of devices in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -4037,15 +4130,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_device_managers_serialize(
+        _param = self._get_devices_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -4053,32 +4146,33 @@
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "DevicePage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_device_managers_without_preload_content(
+    def get_devices_without_preload_content(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -4086,20 +4180,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of Device Managers (on-prem FMCs and cloud-delivered FMCs) in the CDO tenant
+        """Get Devices
 
+        Get a list of devices in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -4119,15 +4214,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_device_managers_serialize(
+        _param = self._get_devices_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -4135,24 +4230,25 @@
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "DevicePage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_device_managers_serialize(
+    def _get_devices_serialize(
         self,
         limit,
         offset,
         q,
         sort,
         _request_auth,
         _content_type,
@@ -4207,15 +4303,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/inventory/managers',
+            resource_path='/v1/inventory/devices',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -4224,44 +4320,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_devices(
+    def get_template_device(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
+        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> DevicePage:
-        """Fetch a list of devices in the CDO tenant
+    ) -> Device:
+        """Get Template Device
 
+        Get a template device by UID in the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
+        :param template_device_uid: The unique identifier of the template device in CDO. (required)
+        :type template_device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4276,75 +4364,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_devices_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
-            sort=sort,
+        _param = self._get_template_device_serialize(
+            template_device_uid=template_device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DevicePage",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_devices_with_http_info(
+    def get_template_device_with_http_info(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
+        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[DevicePage]:
-        """Fetch a list of devices in the CDO tenant
+    ) -> ApiResponse[Device]:
+        """Get Template Device
 
+        Get a template device by UID in the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
+        :param template_device_uid: The unique identifier of the template device in CDO. (required)
+        :type template_device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4359,75 +4436,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_devices_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
-            sort=sort,
+        _param = self._get_template_device_serialize(
+            template_device_uid=template_device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DevicePage",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_devices_without_preload_content(
+    def get_template_device_without_preload_content(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
+        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of devices in the CDO tenant
+        """Get Template Device
 
+        Get a template device by UID in the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
+        :param template_device_uid: The unique identifier of the template device in CDO. (required)
+        :type template_device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4442,83 +4508,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_devices_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
-            sort=sort,
+        _param = self._get_template_device_serialize(
+            template_device_uid=template_device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "DevicePage",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_devices_serialize(
+    def _get_template_device_serialize(
         self,
-        limit,
-        offset,
-        q,
-        sort,
+        template_device_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if template_device_uid is not None:
+            _path_params['templateDeviceUid'] = template_device_uid
         # process the query parameters
-        if limit is not None:
-            
-            _query_params.append(('limit', limit))
-            
-        if offset is not None:
-            
-            _query_params.append(('offset', offset))
-            
-        if q is not None:
-            
-            _query_params.append(('q', q))
-            
-        if sort is not None:
-            
-            _query_params.append(('sort', sort))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -4531,15 +4576,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/inventory/devices',
+            resource_path='/v1/inventory/templates/{templateDeviceUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -4548,18 +4593,18 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_template_devices(
+    def get_template_devices(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -4567,20 +4612,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> DevicePage:
-        """Fetch a list of template devices in the CDO tenant
+        """Get Template Devices
 
+        Get a list of template devices in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -4600,15 +4646,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_template_devices_serialize(
+        _param = self._get_template_devices_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -4630,18 +4676,18 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_template_devices_with_http_info(
+    def get_template_devices_with_http_info(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -4649,20 +4695,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[DevicePage]:
-        """Fetch a list of template devices in the CDO tenant
+        """Get Template Devices
 
+        Get a list of template devices in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -4682,15 +4729,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_template_devices_serialize(
+        _param = self._get_template_devices_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -4712,18 +4759,18 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_template_devices_without_preload_content(
+    def get_template_devices_without_preload_content(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -4731,20 +4778,21 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of template devices in the CDO tenant
+        """Get Template Devices
 
+        Get a list of template devices in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
         :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
         :type q: str
         :param sort: The fields to sort results by.
         :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -4764,15 +4812,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_template_devices_serialize(
+        _param = self._get_template_devices_serialize(
             limit=limit,
             offset=offset,
             q=q,
             sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -4789,15 +4837,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_template_devices_serialize(
+    def _get_template_devices_serialize(
         self,
         limit,
         offset,
         q,
         sort,
         _request_auth,
         _content_type,
@@ -4869,35 +4917,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def onboard_asa_device(
+    def modify_cloud_service(
         self,
-        asa_create_or_update_input: AsaCreateOrUpdateInput,
+        cloud_service_uid: Annotated[StrictStr, Field(description="The unique identifier of the cloud service in CDO.")],
+        device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CdoTransaction:
-        """Onboard a ASA device in the CDO tenant
+    ) -> Device:
+        """Modify Cloud Service
 
+        Modify a Cloud Service by UID in the CDO tenant.
 
-        :param asa_create_or_update_input: (required)
-        :type asa_create_or_update_input: AsaCreateOrUpdateInput
+        :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
+        :type cloud_service_uid: str
+        :param device_patch_input: (required)
+        :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4912,24 +4964,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._onboard_asa_device_serialize(
-            asa_create_or_update_input=asa_create_or_update_input,
+        _param = self._modify_cloud_service_serialize(
+            cloud_service_uid=cloud_service_uid,
+            device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
@@ -4940,35 +4993,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def onboard_asa_device_with_http_info(
+    def modify_cloud_service_with_http_info(
         self,
-        asa_create_or_update_input: AsaCreateOrUpdateInput,
+        cloud_service_uid: Annotated[StrictStr, Field(description="The unique identifier of the cloud service in CDO.")],
+        device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CdoTransaction]:
-        """Onboard a ASA device in the CDO tenant
+    ) -> ApiResponse[Device]:
+        """Modify Cloud Service
 
+        Modify a Cloud Service by UID in the CDO tenant.
 
-        :param asa_create_or_update_input: (required)
-        :type asa_create_or_update_input: AsaCreateOrUpdateInput
+        :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
+        :type cloud_service_uid: str
+        :param device_patch_input: (required)
+        :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -4983,24 +5040,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._onboard_asa_device_serialize(
-            asa_create_or_update_input=asa_create_or_update_input,
+        _param = self._modify_cloud_service_serialize(
+            cloud_service_uid=cloud_service_uid,
+            device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
@@ -5011,35 +5069,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def onboard_asa_device_without_preload_content(
+    def modify_cloud_service_without_preload_content(
         self,
-        asa_create_or_update_input: AsaCreateOrUpdateInput,
+        cloud_service_uid: Annotated[StrictStr, Field(description="The unique identifier of the cloud service in CDO.")],
+        device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Onboard a ASA device in the CDO tenant
+        """Modify Cloud Service
 
+        Modify a Cloud Service by UID in the CDO tenant.
 
-        :param asa_create_or_update_input: (required)
-        :type asa_create_or_update_input: AsaCreateOrUpdateInput
+        :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
+        :type cloud_service_uid: str
+        :param device_patch_input: (required)
+        :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5054,40 +5116,42 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._onboard_asa_device_serialize(
-            asa_create_or_update_input=asa_create_or_update_input,
+        _param = self._modify_cloud_service_serialize(
+            cloud_service_uid=cloud_service_uid,
+            device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _onboard_asa_device_serialize(
+    def _modify_cloud_service_serialize(
         self,
-        asa_create_or_update_input,
+        cloud_service_uid,
+        device_patch_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -5099,20 +5163,22 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if cloud_service_uid is not None:
+            _path_params['cloudServiceUid'] = cloud_service_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if asa_create_or_update_input is not None:
-            _body_params = asa_create_or_update_input
+        if device_patch_input is not None:
+            _body_params = device_patch_input
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -5134,16 +5200,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/inventory/devices/asas',
+            method='PATCH',
+            resource_path='/v1/inventory/services/{cloudServiceUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -5152,35 +5218,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def onboard_ios_device(
+    def modify_device(
         self,
-        ios_create_or_update_input: IosCreateOrUpdateInput,
+        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CdoTransaction:
-        """Onboard a IOS device in the CDO tenant
+    ) -> Device:
+        """Modify Device
 
+        Modify a device in the CDO tenant
 
-        :param ios_create_or_update_input: (required)
-        :type ios_create_or_update_input: IosCreateOrUpdateInput
+        :param device_uid: The unique identifier of the device in CDO. (required)
+        :type device_uid: str
+        :param device_patch_input: (required)
+        :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5195,62 +5265,69 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._onboard_ios_device_serialize(
-            ios_create_or_update_input=ios_create_or_update_input,
+        _param = self._modify_device_serialize(
+            device_uid=device_uid,
+            device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def onboard_ios_device_with_http_info(
+    def modify_device_with_http_info(
         self,
-        ios_create_or_update_input: IosCreateOrUpdateInput,
+        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CdoTransaction]:
-        """Onboard a IOS device in the CDO tenant
+    ) -> ApiResponse[Device]:
+        """Modify Device
 
+        Modify a device in the CDO tenant
 
-        :param ios_create_or_update_input: (required)
-        :type ios_create_or_update_input: IosCreateOrUpdateInput
+        :param device_uid: The unique identifier of the device in CDO. (required)
+        :type device_uid: str
+        :param device_patch_input: (required)
+        :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5265,62 +5342,69 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._onboard_ios_device_serialize(
-            ios_create_or_update_input=ios_create_or_update_input,
+        _param = self._modify_device_serialize(
+            device_uid=device_uid,
+            device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def onboard_ios_device_without_preload_content(
+    def modify_device_without_preload_content(
         self,
-        ios_create_or_update_input: IosCreateOrUpdateInput,
+        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Onboard a IOS device in the CDO tenant
+        """Modify Device
 
+        Modify a device in the CDO tenant
 
-        :param ios_create_or_update_input: (required)
-        :type ios_create_or_update_input: IosCreateOrUpdateInput
+        :param device_uid: The unique identifier of the device in CDO. (required)
+        :type device_uid: str
+        :param device_patch_input: (required)
+        :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -5335,39 +5419,43 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._onboard_ios_device_serialize(
-            ios_create_or_update_input=ios_create_or_update_input,
+        _param = self._modify_device_serialize(
+            device_uid=device_uid,
+            device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
+            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _onboard_ios_device_serialize(
+    def _modify_device_serialize(
         self,
-        ios_create_or_update_input,
+        device_uid,
+        device_patch_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -5379,20 +5467,22 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if device_uid is not None:
+            _path_params['deviceUid'] = device_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if ios_create_or_update_input is not None:
-            _body_params = ios_create_or_update_input
+        if device_patch_input is not None:
+            _body_params = device_patch_input
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -5414,16 +5504,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/inventory/devices/ios',
+            method='PATCH',
+            resource_path='/v1/inventory/devices/{deviceUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -5432,36 +5522,37 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def patch_cloud_service(
+    def modify_device_manager(
         self,
-        cloud_service_uid: Annotated[StrictStr, Field(description="The unique identifier of the cloud service in CDO.")],
+        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
         device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Device:
-        """Modify a Cloud Service by UID in the CDO tenant
+        """Modify Device Manager
 
+        Modify a device manager by UID in the CDO tenant.
 
-        :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
-        :type cloud_service_uid: str
+        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
+        :type device_manager_uid: str
         :param device_patch_input: (required)
         :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5478,16 +5569,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_cloud_service_serialize(
-            cloud_service_uid=cloud_service_uid,
+        _param = self._modify_device_manager_serialize(
+            device_manager_uid=device_manager_uid,
             device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -5507,36 +5598,37 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def patch_cloud_service_with_http_info(
+    def modify_device_manager_with_http_info(
         self,
-        cloud_service_uid: Annotated[StrictStr, Field(description="The unique identifier of the cloud service in CDO.")],
+        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
         device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Device]:
-        """Modify a Cloud Service by UID in the CDO tenant
+        """Modify Device Manager
 
+        Modify a device manager by UID in the CDO tenant.
 
-        :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
-        :type cloud_service_uid: str
+        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
+        :type device_manager_uid: str
         :param device_patch_input: (required)
         :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5553,16 +5645,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_cloud_service_serialize(
-            cloud_service_uid=cloud_service_uid,
+        _param = self._modify_device_manager_serialize(
+            device_manager_uid=device_manager_uid,
             device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -5582,36 +5674,37 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def patch_cloud_service_without_preload_content(
+    def modify_device_manager_without_preload_content(
         self,
-        cloud_service_uid: Annotated[StrictStr, Field(description="The unique identifier of the cloud service in CDO.")],
+        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
         device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Modify a Cloud Service by UID in the CDO tenant
+        """Modify Device Manager
 
+        Modify a device manager by UID in the CDO tenant.
 
-        :param cloud_service_uid: The unique identifier of the cloud service in CDO. (required)
-        :type cloud_service_uid: str
+        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
+        :type device_manager_uid: str
         :param device_patch_input: (required)
         :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5628,16 +5721,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_cloud_service_serialize(
-            cloud_service_uid=cloud_service_uid,
+        _param = self._modify_device_manager_serialize(
+            device_manager_uid=device_manager_uid,
             device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -5652,17 +5745,17 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _patch_cloud_service_serialize(
+    def _modify_device_manager_serialize(
         self,
-        cloud_service_uid,
+        device_manager_uid,
         device_patch_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
@@ -5675,16 +5768,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if cloud_service_uid is not None:
-            _path_params['cloudServiceUid'] = cloud_service_uid
+        if device_manager_uid is not None:
+            _path_params['deviceManagerUid'] = device_manager_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
         if device_patch_input is not None:
             _body_params = device_patch_input
 
@@ -5713,15 +5806,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PATCH',
-            resource_path='/v1/inventory/services/{cloudServiceUid}',
+            resource_path='/v1/inventory/managers/{deviceManagerUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -5730,36 +5823,37 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def patch_device(
+    def modify_template_device(
         self,
-        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
         device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Device:
-        """Modify a device in the CDO tenant
+        """Modify Template Device
 
+        Modify a template device in the CDO tenant.
 
-        :param device_uid: The unique identifier of the device in CDO. (required)
-        :type device_uid: str
+        :param template_device_uid: The unique identifier of the template device in CDO. (required)
+        :type template_device_uid: str
         :param device_patch_input: (required)
         :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5776,66 +5870,66 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_device_serialize(
-            device_uid=device_uid,
+        _param = self._modify_template_device_serialize(
+            template_device_uid=template_device_uid,
             device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def patch_device_with_http_info(
+    def modify_template_device_with_http_info(
         self,
-        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
         device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Device]:
-        """Modify a device in the CDO tenant
+        """Modify Template Device
 
+        Modify a template device in the CDO tenant.
 
-        :param device_uid: The unique identifier of the device in CDO. (required)
-        :type device_uid: str
+        :param template_device_uid: The unique identifier of the template device in CDO. (required)
+        :type template_device_uid: str
         :param device_patch_input: (required)
         :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5852,66 +5946,66 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_device_serialize(
-            device_uid=device_uid,
+        _param = self._modify_template_device_serialize(
+            template_device_uid=template_device_uid,
             device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def patch_device_without_preload_content(
+    def modify_template_device_without_preload_content(
         self,
-        device_uid: Annotated[StrictStr, Field(description="The unique identifier of the device in CDO.")],
+        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
         device_patch_input: DevicePatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Modify a device in the CDO tenant
+        """Modify Template Device
 
+        Modify a template device in the CDO tenant.
 
-        :param device_uid: The unique identifier of the device in CDO. (required)
-        :type device_uid: str
+        :param template_device_uid: The unique identifier of the template device in CDO. (required)
+        :type template_device_uid: str
         :param device_patch_input: (required)
         :type device_patch_input: DevicePatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -5928,42 +6022,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_device_serialize(
-            device_uid=device_uid,
+        _param = self._modify_template_device_serialize(
+            template_device_uid=template_device_uid,
             device_patch_input=device_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
             '200': "Device",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _patch_device_serialize(
+    def _modify_template_device_serialize(
         self,
-        device_uid,
+        template_device_uid,
         device_patch_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
@@ -5976,16 +6069,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if device_uid is not None:
-            _path_params['deviceUid'] = device_uid
+        if template_device_uid is not None:
+            _path_params['templateDeviceUid'] = template_device_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
         if device_patch_input is not None:
             _body_params = device_patch_input
 
@@ -6014,15 +6107,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PATCH',
-            resource_path='/v1/inventory/devices/{deviceUid}',
+            resource_path='/v1/inventory/templates/{templateDeviceUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -6031,38 +6124,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def patch_device_manager(
+    def onboard_asa_device(
         self,
-        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
-        device_patch_input: DevicePatchInput,
+        asa_create_or_update_input: AsaCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Device:
-        """Modify a device manager by UID in the CDO tenant
+    ) -> CdoTransaction:
+        """Onboard ASA device
 
+        This is an asynchronous operation to onboard an ASA to a CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
-        :type device_manager_uid: str
-        :param device_patch_input: (required)
-        :type device_patch_input: DevicePatchInput
+        :param asa_create_or_update_input: (required)
+        :type asa_create_or_update_input: AsaCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6077,25 +6168,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_device_manager_serialize(
-            device_manager_uid=device_manager_uid,
-            device_patch_input=device_patch_input,
+        _param = self._onboard_asa_device_serialize(
+            asa_create_or_update_input=asa_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
@@ -6106,38 +6196,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def patch_device_manager_with_http_info(
+    def onboard_asa_device_with_http_info(
         self,
-        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
-        device_patch_input: DevicePatchInput,
+        asa_create_or_update_input: AsaCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Device]:
-        """Modify a device manager by UID in the CDO tenant
+    ) -> ApiResponse[CdoTransaction]:
+        """Onboard ASA device
 
+        This is an asynchronous operation to onboard an ASA to a CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
-        :type device_manager_uid: str
-        :param device_patch_input: (required)
-        :type device_patch_input: DevicePatchInput
+        :param asa_create_or_update_input: (required)
+        :type asa_create_or_update_input: AsaCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6152,25 +6240,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_device_manager_serialize(
-            device_manager_uid=device_manager_uid,
-            device_patch_input=device_patch_input,
+        _param = self._onboard_asa_device_serialize(
+            asa_create_or_update_input=asa_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
@@ -6181,38 +6268,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def patch_device_manager_without_preload_content(
+    def onboard_asa_device_without_preload_content(
         self,
-        device_manager_uid: Annotated[StrictStr, Field(description="The unique identifier of the device manager in CDO.")],
-        device_patch_input: DevicePatchInput,
+        asa_create_or_update_input: AsaCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Modify a device manager by UID in the CDO tenant
+        """Onboard ASA device
 
+        This is an asynchronous operation to onboard an ASA to a CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param device_manager_uid: The unique identifier of the device manager in CDO. (required)
-        :type device_manager_uid: str
-        :param device_patch_input: (required)
-        :type device_patch_input: DevicePatchInput
+        :param asa_create_or_update_input: (required)
+        :type asa_create_or_update_input: AsaCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6227,42 +6312,40 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_device_manager_serialize(
-            device_manager_uid=device_manager_uid,
-            device_patch_input=device_patch_input,
+        _param = self._onboard_asa_device_serialize(
+            asa_create_or_update_input=asa_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _patch_device_manager_serialize(
+    def _onboard_asa_device_serialize(
         self,
-        device_manager_uid,
-        device_patch_input,
+        asa_create_or_update_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -6274,22 +6357,20 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if device_manager_uid is not None:
-            _path_params['deviceManagerUid'] = device_manager_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if device_patch_input is not None:
-            _body_params = device_patch_input
+        if asa_create_or_update_input is not None:
+            _body_params = asa_create_or_update_input
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -6311,16 +6392,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/v1/inventory/managers/{deviceManagerUid}',
+            method='POST',
+            resource_path='/v1/inventory/devices/asas',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -6329,38 +6410,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def patch_template_device(
+    def onboard_ios_device(
         self,
-        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
-        device_patch_input: DevicePatchInput,
+        ios_create_or_update_input: IosCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Device:
-        """Modify a template device in the CDO tenant
+    ) -> CdoTransaction:
+        """Onboard IOS Device
 
+        Onboard a IOS device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param template_device_uid: The unique identifier of the template device in CDO. (required)
-        :type template_device_uid: str
-        :param device_patch_input: (required)
-        :type device_patch_input: DevicePatchInput
+        :param ios_create_or_update_input: (required)
+        :type ios_create_or_update_input: IosCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6375,67 +6454,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_template_device_serialize(
-            template_device_uid=template_device_uid,
-            device_patch_input=device_patch_input,
+        _param = self._onboard_ios_device_serialize(
+            ios_create_or_update_input=ios_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def patch_template_device_with_http_info(
+    def onboard_ios_device_with_http_info(
         self,
-        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
-        device_patch_input: DevicePatchInput,
+        ios_create_or_update_input: IosCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Device]:
-        """Modify a template device in the CDO tenant
+    ) -> ApiResponse[CdoTransaction]:
+        """Onboard IOS Device
 
+        Onboard a IOS device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param template_device_uid: The unique identifier of the template device in CDO. (required)
-        :type template_device_uid: str
-        :param device_patch_input: (required)
-        :type device_patch_input: DevicePatchInput
+        :param ios_create_or_update_input: (required)
+        :type ios_create_or_update_input: IosCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6450,67 +6525,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_template_device_serialize(
-            template_device_uid=template_device_uid,
-            device_patch_input=device_patch_input,
+        _param = self._onboard_ios_device_serialize(
+            ios_create_or_update_input=ios_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def patch_template_device_without_preload_content(
+    def onboard_ios_device_without_preload_content(
         self,
-        template_device_uid: Annotated[StrictStr, Field(description="The unique identifier of the template device in CDO.")],
-        device_patch_input: DevicePatchInput,
+        ios_create_or_update_input: IosCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Modify a template device in the CDO tenant
+        """Onboard IOS Device
 
+        Onboard a IOS device in the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param template_device_uid: The unique identifier of the template device in CDO. (required)
-        :type template_device_uid: str
-        :param device_patch_input: (required)
-        :type device_patch_input: DevicePatchInput
+        :param ios_create_or_update_input: (required)
+        :type ios_create_or_update_input: IosCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -6525,42 +6596,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._patch_template_device_serialize(
-            template_device_uid=template_device_uid,
-            device_patch_input=device_patch_input,
+        _param = self._onboard_ios_device_serialize(
+            ios_create_or_update_input=ios_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Device",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _patch_template_device_serialize(
+    def _onboard_ios_device_serialize(
         self,
-        template_device_uid,
-        device_patch_input,
+        ios_create_or_update_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -6572,22 +6640,20 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if template_device_uid is not None:
-            _path_params['templateDeviceUid'] = template_device_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if device_patch_input is not None:
-            _body_params = device_patch_input
+        if ios_create_or_update_input is not None:
+            _body_params = ios_create_or_update_input
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -6609,16 +6675,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/v1/inventory/templates/{templateDeviceUid}',
+            method='POST',
+            resource_path='/v1/inventory/devices/ios',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -6627,15 +6693,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def read_from_asa_device(
+    def read_asa_device_configuration(
         self,
         device_uid: Annotated[StrictStr, Field(description="The unique identifier of the ASA device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -6643,16 +6709,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Read configuration on ASA device into CDO
+        """Read ASA device configuration
 
+        This is an asynchronous operation to read the latest configuration on an ASA device in to the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: The unique identifier of the ASA device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -6670,15 +6737,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._read_from_asa_device_serialize(
+        _param = self._read_asa_device_configuration_serialize(
             device_uid=device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -6697,15 +6764,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def read_from_asa_device_with_http_info(
+    def read_asa_device_configuration_with_http_info(
         self,
         device_uid: Annotated[StrictStr, Field(description="The unique identifier of the ASA device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -6713,16 +6780,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Read configuration on ASA device into CDO
+        """Read ASA device configuration
 
+        This is an asynchronous operation to read the latest configuration on an ASA device in to the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: The unique identifier of the ASA device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -6740,15 +6808,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._read_from_asa_device_serialize(
+        _param = self._read_asa_device_configuration_serialize(
             device_uid=device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -6767,15 +6835,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def read_from_asa_device_without_preload_content(
+    def read_asa_device_configuration_without_preload_content(
         self,
         device_uid: Annotated[StrictStr, Field(description="The unique identifier of the ASA device in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -6783,16 +6851,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Read configuration on ASA device into CDO
+        """Read ASA device configuration
 
+        This is an asynchronous operation to read the latest configuration on an ASA device in to the CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: The unique identifier of the ASA device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -6810,15 +6879,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._read_from_asa_device_serialize(
+        _param = self._read_asa_device_configuration_serialize(
             device_uid=device_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -6832,15 +6901,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _read_from_asa_device_serialize(
+    def _read_asa_device_configuration_serialize(
         self,
         device_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
@@ -6910,16 +6979,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Reconnect an ASA device in the CDO tenant
+        """Reconnect ASA device
 
+        This is an asynchronous operation to re-establish the connection between an ASA and the CDO cloud. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: The unique identifier of the ASA device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -6980,16 +7050,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Reconnect an ASA device in the CDO tenant
+        """Reconnect ASA device
 
+        This is an asynchronous operation to re-establish the connection between an ASA and the CDO cloud. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: The unique identifier of the ASA device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -7050,16 +7121,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Reconnect an ASA device in the CDO tenant
+        """Reconnect ASA device
 
+        This is an asynchronous operation to re-establish the connection between an ASA and the CDO cloud. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
         :param device_uid: The unique identifier of the ASA device in CDO. (required)
         :type device_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/meta_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/meta_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
@@ -51,15 +51,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> JwkSet:
-        """Fetch The JSON Web Key Set
+        """Fetch JSON Web Key Set
 
         Retrieves the JSON Web Key Set (JWKS), which is a set of keys containing the public keys used to verify any JSON Web Token (JWT) issued by the Authorization Server and signed using the RS256 signing algorithm. Note: Verification of the token using a JSON Web Key does not guarantee validity due to the possibility of revocation.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -115,15 +115,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[JwkSet]:
-        """Fetch The JSON Web Key Set
+        """Fetch JSON Web Key Set
 
         Retrieves the JSON Web Key Set (JWKS), which is a set of keys containing the public keys used to verify any JSON Web Token (JWT) issued by the Authorization Server and signed using the RS256 signing algorithm. Note: Verification of the token using a JSON Web Key does not guarantee validity due to the possibility of revocation.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -179,15 +179,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch The JSON Web Key Set
+        """Fetch JSON Web Key Set
 
         Retrieves the JSON Web Key Set (JWKS), which is a set of keys containing the public keys used to verify any JSON Web Token (JWT) issued by the Authorization Server and signed using the RS256 signing algorithm. Note: Verification of the token using a JSON Web Key does not guarantee validity due to the possibility of revocation.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -296,16 +296,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Meta:
-        """Get Meta information about CDO, including the IP addresses of CDO services
+        """Get Meta information
 
+        Get Meta information about CDO, including the IP addresses of CDO services.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -359,16 +360,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Meta]:
-        """Get Meta information about CDO, including the IP addresses of CDO services
+        """Get Meta information
 
+        Get Meta information about CDO, including the IP addresses of CDO services.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -422,16 +424,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get Meta information about CDO, including the IP addresses of CDO services
+        """Get Meta information
 
+        Get Meta information about CDO, including the IP addresses of CDO services.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -523,31 +526,32 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_regions(
+    def get_regions(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoRegionList:
-        """Fetch a list of CDO regions.
+        """Get CDO Regions
 
+        Get the list of regions that CDO is deployed in.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -563,15 +567,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_regions_serialize(
+        _param = self._get_regions_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -586,31 +590,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_regions_with_http_info(
+    def get_regions_with_http_info(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoRegionList]:
-        """Fetch a list of CDO regions.
+        """Get CDO Regions
 
+        Get the list of regions that CDO is deployed in.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -626,15 +631,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_regions_serialize(
+        _param = self._get_regions_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -649,31 +654,32 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_regions_without_preload_content(
+    def get_regions_without_preload_content(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of CDO regions.
+        """Get CDO Regions
 
+        Get the list of regions that CDO is deployed in.
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -689,15 +695,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_regions_serialize(
+        _param = self._get_regions_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -707,15 +713,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_regions_serialize(
+    def _get_regions_serialize(
         self,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/object_management_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/users_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
-from typing import List, Optional
+from typing import Optional
 from typing_extensions import Annotated
-from cdo_sdk_python.models.create_request import CreateRequest
-from cdo_sdk_python.models.list_object_response import ListObjectResponse
-from cdo_sdk_python.models.object_response import ObjectResponse
-from cdo_sdk_python.models.reference_info import ReferenceInfo
-from cdo_sdk_python.models.targets_request import TargetsRequest
-from cdo_sdk_python.models.update_request import UpdateRequest
+from cdo_sdk_python.models.api_token_info import ApiTokenInfo
+from cdo_sdk_python.models.cdo_token_info import CdoTokenInfo
+from cdo_sdk_python.models.status_info import StatusInfo
+from cdo_sdk_python.models.user import User
+from cdo_sdk_python.models.user_create_or_update_input import UserCreateOrUpdateInput
+from cdo_sdk_python.models.user_page import UserPage
 
 from cdo_sdk_python.api_client import ApiClient, RequestSerialized
 from cdo_sdk_python.api_response import ApiResponse
 from cdo_sdk_python.rest import RESTResponseType
 
 
-class ObjectManagementApi:
+class UsersApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def create_object(
+    def create_user(
         self,
-        create_request: CreateRequest,
+        user_create_or_update_input: UserCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ObjectResponse:
-        """Creates an object in the CDO tenant
+    ) -> User:
+        """Create User in CDO Tenant
 
+        Create a user in the CDO tenant. The user may already exist and have access to other tenants, in which case this endpoint adds the user to this tenant.
 
-        :param create_request: (required)
-        :type create_request: CreateRequest
+        :param user_create_or_update_input: (required)
+        :type user_create_or_update_input: UserCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -85,24 +86,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_object_serialize(
-            create_request=create_request,
+        _param = self._create_user_serialize(
+            user_create_or_update_input=user_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "ObjectResponse",
+            '201': "User",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -112,35 +113,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_object_with_http_info(
+    def create_user_with_http_info(
         self,
-        create_request: CreateRequest,
+        user_create_or_update_input: UserCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ObjectResponse]:
-        """Creates an object in the CDO tenant
+    ) -> ApiResponse[User]:
+        """Create User in CDO Tenant
 
+        Create a user in the CDO tenant. The user may already exist and have access to other tenants, in which case this endpoint adds the user to this tenant.
 
-        :param create_request: (required)
-        :type create_request: CreateRequest
+        :param user_create_or_update_input: (required)
+        :type user_create_or_update_input: UserCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -155,24 +157,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_object_serialize(
-            create_request=create_request,
+        _param = self._create_user_serialize(
+            user_create_or_update_input=user_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "ObjectResponse",
+            '201': "User",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -182,35 +184,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_object_without_preload_content(
+    def create_user_without_preload_content(
         self,
-        create_request: CreateRequest,
+        user_create_or_update_input: UserCreateOrUpdateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Creates an object in the CDO tenant
+        """Create User in CDO Tenant
 
+        Create a user in the CDO tenant. The user may already exist and have access to other tenants, in which case this endpoint adds the user to this tenant.
 
-        :param create_request: (required)
-        :type create_request: CreateRequest
+        :param user_create_or_update_input: (required)
+        :type user_create_or_update_input: UserCreateOrUpdateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -225,39 +228,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_object_serialize(
-            create_request=create_request,
+        _param = self._create_user_serialize(
+            user_create_or_update_input=user_create_or_update_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "ObjectResponse",
+            '201': "User",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_object_serialize(
+    def _create_user_serialize(
         self,
-        create_request,
+        user_create_or_update_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -273,16 +276,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_request is not None:
-            _body_params = create_request
+        if user_create_or_update_input is not None:
+            _body_params = user_create_or_update_input
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -300,19 +303,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/v0/objects',
+            resource_path='/v1/users',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -321,38 +325,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def create_targets(
+    def delete_user(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object for which the targets are being added to.")],
-        targets_request: TargetsRequest,
+        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """Create targets for an object in the CDO tenant
+    ) -> None:
+        """Remove User from CDO Tenant
 
+        Delete a User by UID in the CDO tenant. If the user is associated with multiple tenants, they will continue to have access to every other tenant.
 
-        :param uid: The request UID of the object for which the targets are being added to. (required)
-        :type uid: str
-        :param targets_request: (required)
-        :type targets_request: TargetsRequest
+        :param user_uid: The unique identifier of the user in CDO. (required)
+        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -367,67 +369,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_targets_serialize(
-            uid=uid,
-            targets_request=targets_request,
+        _param = self._delete_user_serialize(
+            user_uid=user_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '204': None,
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_targets_with_http_info(
+    def delete_user_with_http_info(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object for which the targets are being added to.")],
-        targets_request: TargetsRequest,
+        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """Create targets for an object in the CDO tenant
+    ) -> ApiResponse[None]:
+        """Remove User from CDO Tenant
 
+        Delete a User by UID in the CDO tenant. If the user is associated with multiple tenants, they will continue to have access to every other tenant.
 
-        :param uid: The request UID of the object for which the targets are being added to. (required)
-        :type uid: str
-        :param targets_request: (required)
-        :type targets_request: TargetsRequest
+        :param user_uid: The unique identifier of the user in CDO. (required)
+        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -442,67 +440,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_targets_serialize(
-            uid=uid,
-            targets_request=targets_request,
+        _param = self._delete_user_serialize(
+            user_uid=user_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '204': None,
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_targets_without_preload_content(
+    def delete_user_without_preload_content(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object for which the targets are being added to.")],
-        targets_request: TargetsRequest,
+        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create targets for an object in the CDO tenant
+        """Remove User from CDO Tenant
 
+        Delete a User by UID in the CDO tenant. If the user is associated with multiple tenants, they will continue to have access to every other tenant.
 
-        :param uid: The request UID of the object for which the targets are being added to. (required)
-        :type uid: str
-        :param targets_request: (required)
-        :type targets_request: TargetsRequest
+        :param user_uid: The unique identifier of the user in CDO. (required)
+        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -517,42 +511,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_targets_serialize(
-            uid=uid,
-            targets_request=targets_request,
+        _param = self._delete_user_serialize(
+            user_uid=user_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '204': None,
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_targets_serialize(
+    def _delete_user_serialize(
         self,
-        uid,
-        targets_request,
+        user_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -564,53 +555,38 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if uid is not None:
-            _path_params['uid'] = uid
+        if user_uid is not None:
+            _path_params['userUid'] = user_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if targets_request is not None:
-            _body_params = targets_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                '*/*', 
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v0/objects/{uid}/targets',
+            method='DELETE',
+            resource_path='/v1/users/{userUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -619,35 +595,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def delete_object(
+    def generate_api_token(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being deleted.")],
+        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API-only user in CDO")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """Deletes an object in the CDO tenant
+    ) -> ApiTokenInfo:
+        """Generate Token for API-only user
 
+        Generate API Token for API-only user. API-only users are used for building automations with CDO. If the user ID provided is not that of an API-only user, this operation will fail.
 
-        :param uid: The request UID of the object being deleted. (required)
-        :type uid: str
+        :param api_user_id: The unique identifier of the API-only user in CDO (required)
+        :type api_user_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -662,24 +639,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_object_serialize(
-            uid=uid,
+        _param = self._generate_api_token_serialize(
+            api_user_id=api_user_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': "object",
+            '201': "ApiTokenInfo",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -689,35 +666,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def delete_object_with_http_info(
+    def generate_api_token_with_http_info(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being deleted.")],
+        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API-only user in CDO")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """Deletes an object in the CDO tenant
+    ) -> ApiResponse[ApiTokenInfo]:
+        """Generate Token for API-only user
 
+        Generate API Token for API-only user. API-only users are used for building automations with CDO. If the user ID provided is not that of an API-only user, this operation will fail.
 
-        :param uid: The request UID of the object being deleted. (required)
-        :type uid: str
+        :param api_user_id: The unique identifier of the API-only user in CDO (required)
+        :type api_user_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -732,24 +710,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_object_serialize(
-            uid=uid,
+        _param = self._generate_api_token_serialize(
+            api_user_id=api_user_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': "object",
+            '201': "ApiTokenInfo",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -759,35 +737,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def delete_object_without_preload_content(
+    def generate_api_token_without_preload_content(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being deleted.")],
+        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API-only user in CDO")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Deletes an object in the CDO tenant
+        """Generate Token for API-only user
 
+        Generate API Token for API-only user. API-only users are used for building automations with CDO. If the user ID provided is not that of an API-only user, this operation will fail.
 
-        :param uid: The request UID of the object being deleted. (required)
-        :type uid: str
+        :param api_user_id: The unique identifier of the API-only user in CDO (required)
+        :type api_user_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -802,39 +781,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_object_serialize(
-            uid=uid,
+        _param = self._generate_api_token_serialize(
+            api_user_id=api_user_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': "object",
+            '201': "ApiTokenInfo",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _delete_object_serialize(
+    def _generate_api_token_serialize(
         self,
-        uid,
+        api_user_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -846,38 +825,38 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if uid is not None:
-            _path_params['uid'] = uid
+        if api_user_id is not None:
+            _path_params['apiUserId'] = api_user_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                '*/*', 
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/v0/objects/{uid}',
+            method='POST',
+            resource_path='/v1/users/{apiUserId}/apiToken/generate',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -886,38 +865,33 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_object(
+    def get_token(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being retrieved.")],
-        fields: Annotated[Optional[StrictStr], Field(description="The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ObjectResponse:
-        """Retrieves an object in the CDO tenant
+    ) -> CdoTokenInfo:
+        """Get Token Info
 
+        Fetch information on the current token. Each CDO token is associated with a specific user and a specific tenant. A token can only be used to perform operations on the tenant it is associated with.
 
-        :param uid: The request UID of the object being retrieved. (required)
-        :type uid: str
-        :param fields: The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".
-        :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -932,66 +906,57 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_object_serialize(
-            uid=uid,
-            fields=fields,
+        _param = self._get_token_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ObjectResponse",
-            '400': "CommonApiError",
+            '200': "CdoTokenInfo",
             '401': "AuthenticationError",
-            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_object_with_http_info(
+    def get_token_with_http_info(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being retrieved.")],
-        fields: Annotated[Optional[StrictStr], Field(description="The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ObjectResponse]:
-        """Retrieves an object in the CDO tenant
+    ) -> ApiResponse[CdoTokenInfo]:
+        """Get Token Info
 
+        Fetch information on the current token. Each CDO token is associated with a specific user and a specific tenant. A token can only be used to perform operations on the tenant it is associated with.
 
-        :param uid: The request UID of the object being retrieved. (required)
-        :type uid: str
-        :param fields: The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".
-        :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1006,66 +971,57 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_object_serialize(
-            uid=uid,
-            fields=fields,
+        _param = self._get_token_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ObjectResponse",
-            '400': "CommonApiError",
+            '200': "CdoTokenInfo",
             '401': "AuthenticationError",
-            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_object_without_preload_content(
+    def get_token_without_preload_content(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being retrieved.")],
-        fields: Annotated[Optional[StrictStr], Field(description="The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Retrieves an object in the CDO tenant
+        """Get Token Info
 
+        Fetch information on the current token. Each CDO token is associated with a specific user and a specific tenant. A token can only be used to perform operations on the tenant it is associated with.
 
-        :param uid: The request UID of the object being retrieved. (required)
-        :type uid: str
-        :param fields: The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".
-        :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1080,41 +1036,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_object_serialize(
-            uid=uid,
-            fields=fields,
+        _param = self._get_token_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ObjectResponse",
-            '400': "CommonApiError",
+            '200': "CdoTokenInfo",
             '401': "AuthenticationError",
-            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_object_serialize(
+    def _get_token_serialize(
         self,
-        uid,
-        fields,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1126,21 +1076,15 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if uid is not None:
-            _path_params['uid'] = uid
         # process the query parameters
-        if fields is not None:
-            
-            _query_params.append(('fields', fields))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1148,19 +1092,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v0/objects/{uid}',
+            resource_path='/v1/token',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1169,35 +1114,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_object_usage(
+    def get_user(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object to retrieve usages for.")],
+        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[ReferenceInfo]:
-        """Retrieves usages of an object in the CDO tenant
+    ) -> User:
+        """Get Tenant User
 
+        Fetch a user by UID in the CDO tenant. This will only return 200 responses for users associated with the CDO tenant.
 
-        :param uid: The request UID of the object to retrieve usages for. (required)
-        :type uid: str
+        :param user_uid: The unique identifier of the user in CDO. (required)
+        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1212,62 +1158,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_object_usage_serialize(
-            uid=uid,
+        _param = self._get_user_serialize(
+            user_uid=user_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ReferenceInfo]",
+            '200': "User",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_object_usage_with_http_info(
+    def get_user_with_http_info(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object to retrieve usages for.")],
+        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[ReferenceInfo]]:
-        """Retrieves usages of an object in the CDO tenant
+    ) -> ApiResponse[User]:
+        """Get Tenant User
 
+        Fetch a user by UID in the CDO tenant. This will only return 200 responses for users associated with the CDO tenant.
 
-        :param uid: The request UID of the object to retrieve usages for. (required)
-        :type uid: str
+        :param user_uid: The unique identifier of the user in CDO. (required)
+        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1282,62 +1230,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_object_usage_serialize(
-            uid=uid,
+        _param = self._get_user_serialize(
+            user_uid=user_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ReferenceInfo]",
+            '200': "User",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_object_usage_without_preload_content(
+    def get_user_without_preload_content(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object to retrieve usages for.")],
+        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Retrieves usages of an object in the CDO tenant
+        """Get Tenant User
 
+        Fetch a user by UID in the CDO tenant. This will only return 200 responses for users associated with the CDO tenant.
 
-        :param uid: The request UID of the object to retrieve usages for. (required)
-        :type uid: str
+        :param user_uid: The unique identifier of the user in CDO. (required)
+        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1352,39 +1302,40 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_object_usage_serialize(
-            uid=uid,
+        _param = self._get_user_serialize(
+            user_uid=user_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ReferenceInfo]",
+            '200': "User",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_object_usage_serialize(
+    def _get_user_serialize(
         self,
-        uid,
+        user_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1396,16 +1347,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if uid is not None:
-            _path_params['uid'] = uid
+        if user_uid is not None:
+            _path_params['userUid'] = user_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1414,19 +1365,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v0/objects/{uid}/usage',
+            resource_path='/v1/users/{userUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1435,44 +1387,42 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_objects(
+    def get_users(
         self,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        sort_by: Annotated[Optional[StrictStr], Field(description="The fields to sort results by.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ListObjectResponse:
-        """Retrieves objects in the CDO tenant
+    ) -> UserPage:
+        """Get Tenant Users
 
+        Get a list of users associated with the CDO tenant.
 
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param sort_by: The fields to sort results by.
-        :type sort_by: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1487,27 +1437,26 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_objects_serialize(
-            q=q,
-            offset=offset,
+        _param = self._get_users_serialize(
             limit=limit,
-            sort_by=sort_by,
+            offset=offset,
+            q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListObjectResponse",
+            '200': "UserPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1517,44 +1466,42 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_objects_with_http_info(
+    def get_users_with_http_info(
         self,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        sort_by: Annotated[Optional[StrictStr], Field(description="The fields to sort results by.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ListObjectResponse]:
-        """Retrieves objects in the CDO tenant
+    ) -> ApiResponse[UserPage]:
+        """Get Tenant Users
 
+        Get a list of users associated with the CDO tenant.
 
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param sort_by: The fields to sort results by.
-        :type sort_by: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1569,27 +1516,26 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_objects_serialize(
-            q=q,
-            offset=offset,
+        _param = self._get_users_serialize(
             limit=limit,
-            sort_by=sort_by,
+            offset=offset,
+            q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListObjectResponse",
+            '200': "UserPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1599,44 +1545,42 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_objects_without_preload_content(
+    def get_users_without_preload_content(
         self,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        sort_by: Annotated[Optional[StrictStr], Field(description="The fields to sort results by.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Retrieves objects in the CDO tenant
+        """Get Tenant Users
 
+        Get a list of users associated with the CDO tenant.
 
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param sort_by: The fields to sort results by.
-        :type sort_by: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1651,45 +1595,43 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_objects_serialize(
-            q=q,
-            offset=offset,
+        _param = self._get_users_serialize(
             limit=limit,
-            sort_by=sort_by,
+            offset=offset,
+            q=q,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ListObjectResponse",
+            '200': "UserPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_objects_serialize(
+    def _get_users_serialize(
         self,
-        q,
-        offset,
         limit,
-        sort_by,
+        offset,
+        q,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1702,29 +1644,25 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if q is not None:
+        if limit is not None:
             
-            _query_params.append(('q', q))
+            _query_params.append(('limit', limit))
             
         if offset is not None:
             
             _query_params.append(('offset', offset))
             
-        if limit is not None:
-            
-            _query_params.append(('limit', limit))
-            
-        if sort_by is not None:
+        if q is not None:
             
-            _query_params.append(('sortBy', sort_by))
+            _query_params.append(('q', q))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1733,19 +1671,20 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v0/objects',
+            resource_path='/v1/users',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1754,38 +1693,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def remove_targets(
+    def revoke_api_token(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object for which the targets are being removed from.")],
-        target_uuids: Annotated[List[StrictStr], Field(description="The list of UIDs of the targets being removed.")],
+        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """Removes targets from an object in the CDO tenant
+    ) -> StatusInfo:
+        """Revoke API-only User's Token
 
+        Revoke API Token of API-only user. If the user ID provided is not that of an API-only user, this operation will fail.
 
-        :param uid: The request UID of the object for which the targets are being removed from. (required)
-        :type uid: str
-        :param target_uuids: The list of UIDs of the targets being removed. (required)
-        :type target_uuids: List[str]
+        :param api_user_id: The unique identifier of the API user in CDO. (required)
+        :type api_user_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1800,67 +1737,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._remove_targets_serialize(
-            uid=uid,
-            target_uuids=target_uuids,
+        _param = self._revoke_api_token_serialize(
+            api_user_id=api_user_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': "object",
+            '201': "StatusInfo",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def remove_targets_with_http_info(
+    def revoke_api_token_with_http_info(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object for which the targets are being removed from.")],
-        target_uuids: Annotated[List[StrictStr], Field(description="The list of UIDs of the targets being removed.")],
+        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """Removes targets from an object in the CDO tenant
+    ) -> ApiResponse[StatusInfo]:
+        """Revoke API-only User's Token
 
+        Revoke API Token of API-only user. If the user ID provided is not that of an API-only user, this operation will fail.
 
-        :param uid: The request UID of the object for which the targets are being removed from. (required)
-        :type uid: str
-        :param target_uuids: The list of UIDs of the targets being removed. (required)
-        :type target_uuids: List[str]
+        :param api_user_id: The unique identifier of the API user in CDO. (required)
+        :type api_user_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1875,67 +1808,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._remove_targets_serialize(
-            uid=uid,
-            target_uuids=target_uuids,
+        _param = self._revoke_api_token_serialize(
+            api_user_id=api_user_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': "object",
+            '201': "StatusInfo",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def remove_targets_without_preload_content(
+    def revoke_api_token_without_preload_content(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object for which the targets are being removed from.")],
-        target_uuids: Annotated[List[StrictStr], Field(description="The list of UIDs of the targets being removed.")],
+        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Removes targets from an object in the CDO tenant
+        """Revoke API-only User's Token
 
+        Revoke API Token of API-only user. If the user ID provided is not that of an API-only user, this operation will fail.
 
-        :param uid: The request UID of the object for which the targets are being removed from. (required)
-        :type uid: str
-        :param target_uuids: The list of UIDs of the targets being removed. (required)
-        :type target_uuids: List[str]
+        :param api_user_id: The unique identifier of the API user in CDO. (required)
+        :type api_user_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1950,90 +1879,82 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._remove_targets_serialize(
-            uid=uid,
-            target_uuids=target_uuids,
+        _param = self._revoke_api_token_serialize(
+            api_user_id=api_user_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': "object",
+            '201': "StatusInfo",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _remove_targets_serialize(
+    def _revoke_api_token_serialize(
         self,
-        uid,
-        target_uuids,
+        api_user_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'targetUuids': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if uid is not None:
-            _path_params['uid'] = uid
+        if api_user_id is not None:
+            _path_params['apiUserId'] = api_user_id
         # process the query parameters
-        if target_uuids is not None:
-            
-            _query_params.append(('targetUuids', target_uuids))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                '*/*', 
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/v0/objects/{uid}/targets',
+            method='POST',
+            resource_path='/v1/users/{apiUserId}/apiToken/revoke',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2042,38 +1963,33 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def update_object(
+    def revoke_token(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being updated.")],
-        update_request: UpdateRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ObjectResponse:
-        """Updates an object in the CDO tenant
+    ) -> None:
+        """Revoke Token
 
+        Revoke the current token. All subsequent requests with a revoked token will fail with 401 Unauthorized errors.
 
-        :param uid: The request UID of the object being updated. (required)
-        :type uid: str
-        :param update_request: (required)
-        :type update_request: UpdateRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2088,66 +2004,57 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_object_serialize(
-            uid=uid,
-            update_request=update_request,
+        _param = self._revoke_token_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ObjectResponse",
-            '400': "CommonApiError",
+            '200': None,
             '401': "AuthenticationError",
-            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def update_object_with_http_info(
+    def revoke_token_with_http_info(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being updated.")],
-        update_request: UpdateRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ObjectResponse]:
-        """Updates an object in the CDO tenant
+    ) -> ApiResponse[None]:
+        """Revoke Token
 
+        Revoke the current token. All subsequent requests with a revoked token will fail with 401 Unauthorized errors.
 
-        :param uid: The request UID of the object being updated. (required)
-        :type uid: str
-        :param update_request: (required)
-        :type update_request: UpdateRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2162,66 +2069,57 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_object_serialize(
-            uid=uid,
-            update_request=update_request,
+        _param = self._revoke_token_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ObjectResponse",
-            '400': "CommonApiError",
+            '200': None,
             '401': "AuthenticationError",
-            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def update_object_without_preload_content(
+    def revoke_token_without_preload_content(
         self,
-        uid: Annotated[StrictStr, Field(description="The request UID of the object being updated.")],
-        update_request: UpdateRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Updates an object in the CDO tenant
+        """Revoke Token
 
+        Revoke the current token. All subsequent requests with a revoked token will fail with 401 Unauthorized errors.
 
-        :param uid: The request UID of the object being updated. (required)
-        :type uid: str
-        :param update_request: (required)
-        :type update_request: UpdateRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2236,41 +2134,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_object_serialize(
-            uid=uid,
-            update_request=update_request,
+        _param = self._revoke_token_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ObjectResponse",
-            '400': "CommonApiError",
+            '200': None,
             '401': "AuthenticationError",
-            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _update_object_serialize(
+    def _revoke_token_serialize(
         self,
-        uid,
-        update_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -2282,52 +2174,36 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if uid is not None:
-            _path_params['uid'] = uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if update_request is not None:
-            _body_params = update_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/v0/objects/{uid}',
+            method='POST',
+            resource_path='/v1/token/revoke',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/remote_access_monitoring_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/tenant_management_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
-from typing import List, Optional
+from typing import Optional
 from typing_extensions import Annotated
-from cdo_sdk_python.models.cdo_transaction import CdoTransaction
-from cdo_sdk_python.models.ra_vpn_session import RaVpnSession
-from cdo_sdk_python.models.ra_vpn_session_page import RaVpnSessionPage
+from cdo_sdk_python.models.msp_add_tenant_input import MspAddTenantInput
+from cdo_sdk_python.models.status_info import StatusInfo
+from cdo_sdk_python.models.tenant import Tenant
+from cdo_sdk_python.models.tenant_page import TenantPage
+from cdo_sdk_python.models.tenant_settings import TenantSettings
 
 from cdo_sdk_python.api_client import ApiClient, RequestSerialized
 from cdo_sdk_python.api_response import ApiResponse
 from cdo_sdk_python.rest import RESTResponseType
 
 
-class RemoteAccessMonitoringApi:
+class TenantManagementApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def get_ra_vpn_session(
+    def add_msp_tenant(
         self,
-        ra_vpn_session_uid: Annotated[StrictStr, Field(description="The unique identifier of the RA VPN session in CDO.")],
+        msp_add_tenant_input: MspAddTenantInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RaVpnSession:
-        """Fetch a RA VPN session by UID in the CDO tenant.
+    ) -> StatusInfo:
+        """Add Tenant to MSP Portal
 
+        Add a tenant to the MSP Portal. This endpoint requires that the token provided is that of an MSP tenant.
 
-        :param ra_vpn_session_uid: The unique identifier of the RA VPN session in CDO. (required)
-        :type ra_vpn_session_uid: str
+        :param msp_add_tenant_input: (required)
+        :type msp_add_tenant_input: MspAddTenantInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -82,64 +85,596 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_ra_vpn_session_serialize(
-            ra_vpn_session_uid=ra_vpn_session_uid,
+        _param = self._add_msp_tenant_serialize(
+            msp_add_tenant_input=msp_add_tenant_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RaVpnSession",
+            '201': "StatusInfo",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def add_msp_tenant_with_http_info(
+        self,
+        msp_add_tenant_input: MspAddTenantInput,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[StatusInfo]:
+        """Add Tenant to MSP Portal
+
+        Add a tenant to the MSP Portal. This endpoint requires that the token provided is that of an MSP tenant.
+
+        :param msp_add_tenant_input: (required)
+        :type msp_add_tenant_input: MspAddTenantInput
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._add_msp_tenant_serialize(
+            msp_add_tenant_input=msp_add_tenant_input,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "StatusInfo",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def add_msp_tenant_without_preload_content(
+        self,
+        msp_add_tenant_input: MspAddTenantInput,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Add Tenant to MSP Portal
+
+        Add a tenant to the MSP Portal. This endpoint requires that the token provided is that of an MSP tenant.
+
+        :param msp_add_tenant_input: (required)
+        :type msp_add_tenant_input: MspAddTenantInput
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._add_msp_tenant_serialize(
+            msp_add_tenant_input=msp_add_tenant_input,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "StatusInfo",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _add_msp_tenant_serialize(
+        self,
+        msp_add_tenant_input,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if msp_add_tenant_input is not None:
+            _body_params = msp_add_tenant_input
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'bearerAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/v1/msp/tenants',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def get_feature_flags(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> List[str]:
+        """Get Feature Flags
+
+        Get the feature flags enabled in the CDO tenant.
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_feature_flags_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[str]",
+            '401': "AuthenticationError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def get_feature_flags_with_http_info(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[List[str]]:
+        """Get Feature Flags
+
+        Get the feature flags enabled in the CDO tenant.
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_feature_flags_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[str]",
+            '401': "AuthenticationError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def get_feature_flags_without_preload_content(
+        self,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Get Feature Flags
+
+        Get the feature flags enabled in the CDO tenant.
+
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_feature_flags_serialize(
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "List[str]",
+            '401': "AuthenticationError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _get_feature_flags_serialize(
+        self,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'bearerAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/v1/features',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def get_tenant(
+        self,
+        tenant_uid: Annotated[StrictStr, Field(description="The unique identifier of the tenant in CDO.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Tenant:
+        """Get Tenant
+
+        Fetch a tenant by UID in CDO. This will return a 200 response only if the user is associated with the tenant.
+
+        :param tenant_uid: The unique identifier of the tenant in CDO. (required)
+        :type tenant_uid: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._get_tenant_serialize(
+            tenant_uid=tenant_uid,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Tenant",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_ra_vpn_session_with_http_info(
+    def get_tenant_with_http_info(
         self,
-        ra_vpn_session_uid: Annotated[StrictStr, Field(description="The unique identifier of the RA VPN session in CDO.")],
+        tenant_uid: Annotated[StrictStr, Field(description="The unique identifier of the tenant in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[RaVpnSession]:
-        """Fetch a RA VPN session by UID in the CDO tenant.
+    ) -> ApiResponse[Tenant]:
+        """Get Tenant
 
+        Fetch a tenant by UID in CDO. This will return a 200 response only if the user is associated with the tenant.
 
-        :param ra_vpn_session_uid: The unique identifier of the RA VPN session in CDO. (required)
-        :type ra_vpn_session_uid: str
+        :param tenant_uid: The unique identifier of the tenant in CDO. (required)
+        :type tenant_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -154,64 +689,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_ra_vpn_session_serialize(
-            ra_vpn_session_uid=ra_vpn_session_uid,
+        _param = self._get_tenant_serialize(
+            tenant_uid=tenant_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RaVpnSession",
+            '200': "Tenant",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_ra_vpn_session_without_preload_content(
+    def get_tenant_without_preload_content(
         self,
-        ra_vpn_session_uid: Annotated[StrictStr, Field(description="The unique identifier of the RA VPN session in CDO.")],
+        tenant_uid: Annotated[StrictStr, Field(description="The unique identifier of the tenant in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a RA VPN session by UID in the CDO tenant.
+        """Get Tenant
 
+        Fetch a tenant by UID in CDO. This will return a 200 response only if the user is associated with the tenant.
 
-        :param ra_vpn_session_uid: The unique identifier of the RA VPN session in CDO. (required)
-        :type ra_vpn_session_uid: str
+        :param tenant_uid: The unique identifier of the tenant in CDO. (required)
+        :type tenant_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -226,41 +761,40 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_ra_vpn_session_serialize(
-            ra_vpn_session_uid=ra_vpn_session_uid,
+        _param = self._get_tenant_serialize(
+            tenant_uid=tenant_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RaVpnSession",
+            '200': "Tenant",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '404': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_ra_vpn_session_serialize(
+    def _get_tenant_serialize(
         self,
-        ra_vpn_session_uid,
+        tenant_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -272,16 +806,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if ra_vpn_session_uid is not None:
-            _path_params['raVpnSessionUid'] = ra_vpn_session_uid
+        if tenant_uid is not None:
+            _path_params['tenantUid'] = tenant_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -295,15 +829,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/vpnsessions/{raVpnSessionUid}',
+            resource_path='/v1/tenants/{tenantUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -312,44 +846,33 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_ra_vpn_sessions(
+    def get_tenant_settings(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RaVpnSessionPage:
-        """Fetch a list of RA VPN sessions.
+    ) -> TenantSettings:
+        """Get Tenant Settings
 
+        Get the settings for the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -364,75 +887,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_ra_vpn_sessions_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
-            sort=sort,
+        _param = self._get_tenant_settings_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RaVpnSessionPage",
+            '200': "TenantSettings",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_ra_vpn_sessions_with_http_info(
+    def get_tenant_settings_with_http_info(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[RaVpnSessionPage]:
-        """Fetch a list of RA VPN sessions.
+    ) -> ApiResponse[TenantSettings]:
+        """Get Tenant Settings
 
+        Get the settings for the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -447,75 +954,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_ra_vpn_sessions_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
-            sort=sort,
+        _param = self._get_tenant_settings_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RaVpnSessionPage",
+            '200': "TenantSettings",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_ra_vpn_sessions_without_preload_content(
+    def get_tenant_settings_without_preload_content(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
-        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of RA VPN sessions.
+        """Get Tenant Settings
 
+        Get the settings for the CDO tenant.
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
-        :param sort: The fields to sort results by.
-        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -530,83 +1021,57 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_ra_vpn_sessions_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
-            sort=sort,
+        _param = self._get_tenant_settings_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "RaVpnSessionPage",
+            '200': "TenantSettings",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_ra_vpn_sessions_serialize(
+    def _get_tenant_settings_serialize(
         self,
-        limit,
-        offset,
-        q,
-        sort,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if limit is not None:
-            
-            _query_params.append(('limit', limit))
-            
-        if offset is not None:
-            
-            _query_params.append(('offset', offset))
-            
-        if q is not None:
-            
-            _query_params.append(('q', q))
-            
-        if sort is not None:
-            
-            _query_params.append(('sort', sort))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -619,15 +1084,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/vpnsessions',
+            resource_path='/v1/settings/tenant',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -636,35 +1101,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def terminate_ra_vpn_sessions_by_device(
+    def get_tenants(
         self,
-        device_uid: StrictStr,
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CdoTransaction:
-        """Terminate all RA VPN sessions on a device in the CDO tenant.
+    ) -> TenantPage:
+        """Get Tenants
 
+        Get a list of tenants with which the CDO user is associated.
 
-        :param device_uid: (required)
-        :type device_uid: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -679,63 +1148,67 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._terminate_ra_vpn_sessions_by_device_serialize(
-            device_uid=device_uid,
+        _param = self._get_tenants_serialize(
+            limit=limit,
+            offset=offset,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "TenantPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def terminate_ra_vpn_sessions_by_device_with_http_info(
+    def get_tenants_with_http_info(
         self,
-        device_uid: StrictStr,
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CdoTransaction]:
-        """Terminate all RA VPN sessions on a device in the CDO tenant.
+    ) -> ApiResponse[TenantPage]:
+        """Get Tenants
 
+        Get a list of tenants with which the CDO user is associated.
 
-        :param device_uid: (required)
-        :type device_uid: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -750,63 +1223,67 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._terminate_ra_vpn_sessions_by_device_serialize(
-            device_uid=device_uid,
+        _param = self._get_tenants_serialize(
+            limit=limit,
+            offset=offset,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "TenantPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def terminate_ra_vpn_sessions_by_device_without_preload_content(
+    def get_tenants_without_preload_content(
         self,
-        device_uid: StrictStr,
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Terminate all RA VPN sessions on a device in the CDO tenant.
+        """Get Tenants
 
+        Get a list of tenants with which the CDO user is associated.
 
-        :param device_uid: (required)
-        :type device_uid: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -821,40 +1298,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._terminate_ra_vpn_sessions_by_device_serialize(
-            device_uid=device_uid,
+        _param = self._get_tenants_serialize(
+            limit=limit,
+            offset=offset,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "TenantPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _terminate_ra_vpn_sessions_by_device_serialize(
+    def _get_tenants_serialize(
         self,
-        device_uid,
+        limit,
+        offset,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -866,17 +1344,23 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if device_uid is not None:
-            _path_params['deviceUid'] = device_uid
         # process the query parameters
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if offset is not None:
+            
+            _query_params.append(('offset', offset))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -888,16 +1372,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/vpnsessions/{deviceUid}/terminate',
+            method='GET',
+            resource_path='/v1/tenants',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -906,38 +1390,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def terminate_ra_vpn_sessions_by_device_and_user_name(
+    def modify_tenant_settings(
         self,
-        device_uid: StrictStr,
-        user_name: StrictStr,
+        tenant_settings: TenantSettings,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CdoTransaction:
-        """Terminate all of a user's RA VPN sessions on a device in the CDO tenant
+    ) -> TenantSettings:
+        """Modify Tenant Settings
 
+        Modify the settings for the CDO tenant.
 
-        :param device_uid: (required)
-        :type device_uid: str
-        :param user_name: (required)
-        :type user_name: str
+        :param tenant_settings: (required)
+        :type tenant_settings: TenantSettings
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -952,67 +1434,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._terminate_ra_vpn_sessions_by_device_and_user_name_serialize(
-            device_uid=device_uid,
-            user_name=user_name,
+        _param = self._modify_tenant_settings_serialize(
+            tenant_settings=tenant_settings,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "TenantSettings",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def terminate_ra_vpn_sessions_by_device_and_user_name_with_http_info(
+    def modify_tenant_settings_with_http_info(
         self,
-        device_uid: StrictStr,
-        user_name: StrictStr,
+        tenant_settings: TenantSettings,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CdoTransaction]:
-        """Terminate all of a user's RA VPN sessions on a device in the CDO tenant
+    ) -> ApiResponse[TenantSettings]:
+        """Modify Tenant Settings
 
+        Modify the settings for the CDO tenant.
 
-        :param device_uid: (required)
-        :type device_uid: str
-        :param user_name: (required)
-        :type user_name: str
+        :param tenant_settings: (required)
+        :type tenant_settings: TenantSettings
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1027,67 +1505,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._terminate_ra_vpn_sessions_by_device_and_user_name_serialize(
-            device_uid=device_uid,
-            user_name=user_name,
+        _param = self._modify_tenant_settings_serialize(
+            tenant_settings=tenant_settings,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "TenantSettings",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def terminate_ra_vpn_sessions_by_device_and_user_name_without_preload_content(
+    def modify_tenant_settings_without_preload_content(
         self,
-        device_uid: StrictStr,
-        user_name: StrictStr,
+        tenant_settings: TenantSettings,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Terminate all of a user's RA VPN sessions on a device in the CDO tenant
+        """Modify Tenant Settings
 
+        Modify the settings for the CDO tenant.
 
-        :param device_uid: (required)
-        :type device_uid: str
-        :param user_name: (required)
-        :type user_name: str
+        :param tenant_settings: (required)
+        :type tenant_settings: TenantSettings
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1102,42 +1576,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._terminate_ra_vpn_sessions_by_device_and_user_name_serialize(
-            device_uid=device_uid,
-            user_name=user_name,
+        _param = self._modify_tenant_settings_serialize(
+            tenant_settings=tenant_settings,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '202': "CdoTransaction",
+            '200': "TenantSettings",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _terminate_ra_vpn_sessions_by_device_and_user_name_serialize(
+    def _modify_tenant_settings_serialize(
         self,
-        device_uid,
-        user_name,
+        tenant_settings,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1149,40 +1620,51 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if device_uid is not None:
-            _path_params['deviceUid'] = device_uid
-        if user_name is not None:
-            _path_params['userName'] = user_name
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if tenant_settings is not None:
+            _body_params = tenant_settings
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/vpnsessions/{deviceUid}/terminate/{userName}',
+            method='PATCH',
+            resource_path='/v1/settings/tenant',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/search_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/transactions_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import StrictStr
 from cdo_sdk_python.models.cdo_transaction import CdoTransaction
-from cdo_sdk_python.models.global_search_result import GlobalSearchResult
 
 from cdo_sdk_python.api_client import ApiClient, RequestSerialized
 from cdo_sdk_python.api_response import ApiResponse
 from cdo_sdk_python.rest import RESTResponseType
 
 
-class SearchApi:
+class TransactionsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def initiate_full_indexing(
+    def get_transaction(
         self,
+        transaction_uid: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> CdoTransaction:
-        """Initiate Full Indexing
+        """Get Transaction
 
+        Get information of an in-progress CDO transaction. A CDO transaction is an entity used to monitor progress of, and provide feedback on, long-running operations. All asynchronous operations in CDO's API create CDO transactions.
 
+        :param transaction_uid: (required)
+        :type transaction_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -76,59 +79,65 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._initiate_full_indexing_serialize(
+        _param = self._get_transaction_serialize(
+            transaction_uid=transaction_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "CdoTransaction",
             '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def initiate_full_indexing_with_http_info(
+    def get_transaction_with_http_info(
         self,
+        transaction_uid: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[CdoTransaction]:
-        """Initiate Full Indexing
+        """Get Transaction
 
+        Get information of an in-progress CDO transaction. A CDO transaction is an entity used to monitor progress of, and provide feedback on, long-running operations. All asynchronous operations in CDO's API create CDO transactions.
 
+        :param transaction_uid: (required)
+        :type transaction_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -143,59 +152,65 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._initiate_full_indexing_serialize(
+        _param = self._get_transaction_serialize(
+            transaction_uid=transaction_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "CdoTransaction",
             '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def initiate_full_indexing_without_preload_content(
+    def get_transaction_without_preload_content(
         self,
+        transaction_uid: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Initiate Full Indexing
+        """Get Transaction
 
+        Get information of an in-progress CDO transaction. A CDO transaction is an entity used to monitor progress of, and provide feedback on, long-running operations. All asynchronous operations in CDO's API create CDO transactions.
 
+        :param transaction_uid: (required)
+        :type transaction_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -210,38 +225,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._initiate_full_indexing_serialize(
+        _param = self._get_transaction_serialize(
+            transaction_uid=transaction_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "CdoTransaction",
             '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '405': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _initiate_full_indexing_serialize(
+    def _get_transaction_serialize(
         self,
+        transaction_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -253,14 +271,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if transaction_uid is not None:
+            _path_params['transactionUid'] = transaction_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -273,288 +293,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/search/index',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def search(
-        self,
-        q: StrictStr,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GlobalSearchResult:
-        """Search for devices, services, managers, objects and policies across the CDO tenant
-
-
-        :param q: (required)
-        :type q: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._search_serialize(
-            q=q,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GlobalSearchResult",
-            '400': "CommonApiError",
-            '401': "AuthenticationError",
-            '403': "CommonApiError",
-            '405': "CommonApiError",
-            '500': "CommonApiError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def search_with_http_info(
-        self,
-        q: StrictStr,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GlobalSearchResult]:
-        """Search for devices, services, managers, objects and policies across the CDO tenant
-
-
-        :param q: (required)
-        :type q: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._search_serialize(
-            q=q,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GlobalSearchResult",
-            '400': "CommonApiError",
-            '401': "AuthenticationError",
-            '403': "CommonApiError",
-            '405': "CommonApiError",
-            '500': "CommonApiError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def search_without_preload_content(
-        self,
-        q: StrictStr,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Search for devices, services, managers, objects and policies across the CDO tenant
-
-
-        :param q: (required)
-        :type q: str
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._search_serialize(
-            q=q,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GlobalSearchResult",
-            '400': "CommonApiError",
-            '401': "AuthenticationError",
-            '403': "CommonApiError",
-            '405': "CommonApiError",
-            '500': "CommonApiError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _search_serialize(
-        self,
-        q,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if q is not None:
-            
-            _query_params.append(('q', q))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'bearerAuth'
-        ]
-
-        return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/search',
+            resource_path='/v1/transactions/{transactionUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/tenant_management_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/connectors_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
-from cdo_sdk_python.models.msp_add_tenant_input import MspAddTenantInput
-from cdo_sdk_python.models.status_info import StatusInfo
-from cdo_sdk_python.models.tenant import Tenant
-from cdo_sdk_python.models.tenant_page import TenantPage
-from cdo_sdk_python.models.tenant_settings import TenantSettings
+from cdo_sdk_python.models.cdo_transaction import CdoTransaction
+from cdo_sdk_python.models.sdc import Sdc
+from cdo_sdk_python.models.sdc_create_input import SdcCreateInput
+from cdo_sdk_python.models.sdc_page import SdcPage
+from cdo_sdk_python.models.sdc_patch_input import SdcPatchInput
 
 from cdo_sdk_python.api_client import ApiClient, RequestSerialized
 from cdo_sdk_python.api_response import ApiResponse
 from cdo_sdk_python.rest import RESTResponseType
 
 
-class TenantManagementApi:
+class ConnectorsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def add_msp_tenant(
+    def create_sdc(
         self,
-        msp_add_tenant_input: MspAddTenantInput,
+        sdc_create_input: SdcCreateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> StatusInfo:
-        """Add a tenant to the MSP Portal
+    ) -> CdoTransaction:
+        """Create SDC
 
+        This is an asynchronous operation to create an SDC to a CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param msp_add_tenant_input: (required)
-        :type msp_add_tenant_input: MspAddTenantInput
+        :param sdc_create_input: (required)
+        :type sdc_create_input: SdcCreateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -84,24 +85,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._add_msp_tenant_serialize(
-            msp_add_tenant_input=msp_add_tenant_input,
+        _param = self._create_sdc_serialize(
+            sdc_create_input=sdc_create_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "StatusInfo",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -111,35 +112,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def add_msp_tenant_with_http_info(
+    def create_sdc_with_http_info(
         self,
-        msp_add_tenant_input: MspAddTenantInput,
+        sdc_create_input: SdcCreateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[StatusInfo]:
-        """Add a tenant to the MSP Portal
+    ) -> ApiResponse[CdoTransaction]:
+        """Create SDC
 
+        This is an asynchronous operation to create an SDC to a CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param msp_add_tenant_input: (required)
-        :type msp_add_tenant_input: MspAddTenantInput
+        :param sdc_create_input: (required)
+        :type sdc_create_input: SdcCreateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -154,24 +156,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._add_msp_tenant_serialize(
-            msp_add_tenant_input=msp_add_tenant_input,
+        _param = self._create_sdc_serialize(
+            sdc_create_input=sdc_create_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "StatusInfo",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -181,35 +183,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def add_msp_tenant_without_preload_content(
+    def create_sdc_without_preload_content(
         self,
-        msp_add_tenant_input: MspAddTenantInput,
+        sdc_create_input: SdcCreateInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Add a tenant to the MSP Portal
+        """Create SDC
 
+        This is an asynchronous operation to create an SDC to a CDO tenant. This operation returns a link to a transaction object that can be used to monitor the progress of the operation.
 
-        :param msp_add_tenant_input: (required)
-        :type msp_add_tenant_input: MspAddTenantInput
+        :param sdc_create_input: (required)
+        :type sdc_create_input: SdcCreateInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -224,39 +227,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._add_msp_tenant_serialize(
-            msp_add_tenant_input=msp_add_tenant_input,
+        _param = self._create_sdc_serialize(
+            sdc_create_input=sdc_create_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "StatusInfo",
+            '202': "CdoTransaction",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _add_msp_tenant_serialize(
+    def _create_sdc_serialize(
         self,
-        msp_add_tenant_input,
+        sdc_create_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -272,16 +275,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if msp_add_tenant_input is not None:
-            _body_params = msp_add_tenant_input
+        if sdc_create_input is not None:
+            _body_params = sdc_create_input
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -304,15 +307,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/v1/msp/tenants',
+            resource_path='/v1/connectors/sdcs',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -321,35 +324,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_tenant(
+    def delete_sdc(
         self,
-        tenant_uid: Annotated[StrictStr, Field(description="The unique identifier of the tenant in CDO.")],
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Tenant:
-        """Fetch a tenant by UID in CDO
+    ) -> None:
+        """Delete SDC
 
+        Delete an SDC in the CDO tenant
 
-        :param tenant_uid: The unique identifier of the tenant in CDO. (required)
-        :type tenant_uid: str
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -364,63 +368,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_tenant_serialize(
-            tenant_uid=tenant_uid,
+        _param = self._delete_sdc_serialize(
+            sdc_uid=sdc_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Tenant",
+            '204': None,
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_tenant_with_http_info(
+    def delete_sdc_with_http_info(
         self,
-        tenant_uid: Annotated[StrictStr, Field(description="The unique identifier of the tenant in CDO.")],
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Tenant]:
-        """Fetch a tenant by UID in CDO
+    ) -> ApiResponse[None]:
+        """Delete SDC
 
+        Delete an SDC in the CDO tenant
 
-        :param tenant_uid: The unique identifier of the tenant in CDO. (required)
-        :type tenant_uid: str
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -435,63 +439,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_tenant_serialize(
-            tenant_uid=tenant_uid,
+        _param = self._delete_sdc_serialize(
+            sdc_uid=sdc_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Tenant",
+            '204': None,
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_tenant_without_preload_content(
+    def delete_sdc_without_preload_content(
         self,
-        tenant_uid: Annotated[StrictStr, Field(description="The unique identifier of the tenant in CDO.")],
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a tenant by UID in CDO
+        """Delete SDC
 
+        Delete an SDC in the CDO tenant
 
-        :param tenant_uid: The unique identifier of the tenant in CDO. (required)
-        :type tenant_uid: str
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -506,40 +510,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_tenant_serialize(
-            tenant_uid=tenant_uid,
+        _param = self._delete_sdc_serialize(
+            sdc_uid=sdc_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Tenant",
+            '204': None,
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_tenant_serialize(
+    def _delete_sdc_serialize(
         self,
-        tenant_uid,
+        sdc_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -551,16 +554,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if tenant_uid is not None:
-            _path_params['tenantUid'] = tenant_uid
+        if sdc_uid is not None:
+            _path_params['sdcUid'] = sdc_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -573,16 +576,16 @@
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/v1/tenants/{tenantUid}',
+            method='DELETE',
+            resource_path='/v1/connectors/sdcs/{sdcUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -591,32 +594,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_tenant_settings(
+    def get_sdc(
         self,
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> TenantSettings:
-        """Fetch the tenant settings in CDO
+    ) -> Sdc:
+        """Get SDC
 
+        Get a SDC by UID in the CDO tenant.
 
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -631,58 +638,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_tenant_settings_serialize(
+        _param = self._get_sdc_serialize(
+            sdc_uid=sdc_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantSettings",
+            '200': "Sdc",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_tenant_settings_with_http_info(
+    def get_sdc_with_http_info(
         self,
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[TenantSettings]:
-        """Fetch the tenant settings in CDO
+    ) -> ApiResponse[Sdc]:
+        """Get SDC
 
+        Get a SDC by UID in the CDO tenant.
 
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -697,58 +710,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_tenant_settings_serialize(
+        _param = self._get_sdc_serialize(
+            sdc_uid=sdc_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantSettings",
+            '200': "Sdc",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_tenant_settings_without_preload_content(
+    def get_sdc_without_preload_content(
         self,
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch the tenant settings in CDO
+        """Get SDC
 
+        Get a SDC by UID in the CDO tenant.
 
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -763,283 +782,40 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_tenant_settings_serialize(
+        _param = self._get_sdc_serialize(
+            sdc_uid=sdc_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantSettings",
+            '200': "Sdc",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_tenant_settings_serialize(
-        self,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'bearerAuth'
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/v1/settings/tenant',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def list_feature_flags(
-        self,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[str]:
-        """Fetch the feature flags enabled for this tenant
-
-
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._list_feature_flags_serialize(
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[str]",
-            '401': "AuthenticationError",
-            '500': "CommonApiError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def list_feature_flags_with_http_info(
-        self,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[str]]:
-        """Fetch the feature flags enabled for this tenant
-
-
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._list_feature_flags_serialize(
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[str]",
-            '401': "AuthenticationError",
-            '500': "CommonApiError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def list_feature_flags_without_preload_content(
-        self,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Fetch the feature flags enabled for this tenant
-
-
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._list_feature_flags_serialize(
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[str]",
-            '401': "AuthenticationError",
-            '500': "CommonApiError",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _list_feature_flags_serialize(
+    def _get_sdc_serialize(
         self,
+        sdc_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1051,14 +827,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if sdc_uid is not None:
+            _path_params['sdcUid'] = sdc_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1072,15 +850,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/features',
+            resource_path='/v1/connectors/sdcs/{sdcUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1089,38 +867,45 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_tenants(
+    def get_sdcs(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> TenantPage:
-        """Fetch a list of tenants associated with the CDO user.
+    ) -> SdcPage:
+        """Get SDCs
 
+        Get a list of on-prem SDCs in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param sort: The fields to sort results by.
+        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1135,25 +920,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_tenants_serialize(
+        _param = self._get_sdcs_serialize(
             limit=limit,
             offset=offset,
+            q=q,
+            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantPage",
+            '200': "SdcPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1163,38 +950,45 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_tenants_with_http_info(
+    def get_sdcs_with_http_info(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[TenantPage]:
-        """Fetch a list of tenants associated with the CDO user.
+    ) -> ApiResponse[SdcPage]:
+        """Get SDCs
 
+        Get a list of on-prem SDCs in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param sort: The fields to sort results by.
+        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1209,25 +1003,27 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_tenants_serialize(
+        _param = self._get_sdcs_serialize(
             limit=limit,
             offset=offset,
+            q=q,
+            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantPage",
+            '200': "SdcPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1237,38 +1033,45 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_tenants_without_preload_content(
+    def get_sdcs_without_preload_content(
         self,
         limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        sort: Annotated[Optional[List[StrictStr]], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of tenants associated with the CDO user.
+        """Get SDCs
 
+        Get a list of on-prem SDCs in the CDO tenant.
 
         :param limit: The number of results to retrieve.
         :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
         :type offset: str
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param sort: The fields to sort results by.
+        :type sort: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1283,50 +1086,55 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_tenants_serialize(
+        _param = self._get_sdcs_serialize(
             limit=limit,
             offset=offset,
+            q=q,
+            sort=sort,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantPage",
+            '200': "SdcPage",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_tenants_serialize(
+    def _get_sdcs_serialize(
         self,
         limit,
         offset,
+        q,
+        sort,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
+            'sort': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
@@ -1338,14 +1146,22 @@
             
             _query_params.append(('limit', limit))
             
         if offset is not None:
             
             _query_params.append(('offset', offset))
             
+        if q is not None:
+            
+            _query_params.append(('q', q))
+            
+        if sort is not None:
+            
+            _query_params.append(('sort', sort))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1358,15 +1174,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/tenants',
+            resource_path='/v1/connectors/sdcs',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1375,35 +1191,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def update_tenant_settings(
+    def modify_sdc(
         self,
-        tenant_settings: TenantSettings,
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
+        sdc_patch_input: SdcPatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> TenantSettings:
-        """Update the tenant settings in CDO
+    ) -> Sdc:
+        """Modify SDC
 
+        Modify a SDC in the CDO tenant
 
-        :param tenant_settings: (required)
-        :type tenant_settings: TenantSettings
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
+        :param sdc_patch_input: (required)
+        :type sdc_patch_input: SdcPatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1418,62 +1238,68 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_tenant_settings_serialize(
-            tenant_settings=tenant_settings,
+        _param = self._modify_sdc_serialize(
+            sdc_uid=sdc_uid,
+            sdc_patch_input=sdc_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantSettings",
+            '200': "Sdc",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def update_tenant_settings_with_http_info(
+    def modify_sdc_with_http_info(
         self,
-        tenant_settings: TenantSettings,
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
+        sdc_patch_input: SdcPatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[TenantSettings]:
-        """Update the tenant settings in CDO
+    ) -> ApiResponse[Sdc]:
+        """Modify SDC
 
+        Modify a SDC in the CDO tenant
 
-        :param tenant_settings: (required)
-        :type tenant_settings: TenantSettings
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
+        :param sdc_patch_input: (required)
+        :type sdc_patch_input: SdcPatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1488,62 +1314,68 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_tenant_settings_serialize(
-            tenant_settings=tenant_settings,
+        _param = self._modify_sdc_serialize(
+            sdc_uid=sdc_uid,
+            sdc_patch_input=sdc_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantSettings",
+            '200': "Sdc",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def update_tenant_settings_without_preload_content(
+    def modify_sdc_without_preload_content(
         self,
-        tenant_settings: TenantSettings,
+        sdc_uid: Annotated[StrictStr, Field(description="The unique identifier of the SDC in CDO.")],
+        sdc_patch_input: SdcPatchInput,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Update the tenant settings in CDO
+        """Modify SDC
 
+        Modify a SDC in the CDO tenant
 
-        :param tenant_settings: (required)
-        :type tenant_settings: TenantSettings
+        :param sdc_uid: The unique identifier of the SDC in CDO. (required)
+        :type sdc_uid: str
+        :param sdc_patch_input: (required)
+        :type sdc_patch_input: SdcPatchInput
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1558,39 +1390,42 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._update_tenant_settings_serialize(
-            tenant_settings=tenant_settings,
+        _param = self._modify_sdc_serialize(
+            sdc_uid=sdc_uid,
+            sdc_patch_input=sdc_patch_input,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "TenantSettings",
+            '200': "Sdc",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _update_tenant_settings_serialize(
+    def _modify_sdc_serialize(
         self,
-        tenant_settings,
+        sdc_uid,
+        sdc_patch_input,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1602,20 +1437,22 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if sdc_uid is not None:
+            _path_params['sdcUid'] = sdc_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if tenant_settings is not None:
-            _body_params = tenant_settings
+        if sdc_patch_input is not None:
+            _body_params = sdc_patch_input
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1638,15 +1475,15 @@
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PATCH',
-            resource_path='/v1/settings/tenant',
+            resource_path='/v1/connectors/sdcs/{sdcUid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api/users_api.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api/object_management_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
-from cdo_sdk_python.models.api_token_info import ApiTokenInfo
-from cdo_sdk_python.models.cdo_token_info import CdoTokenInfo
-from cdo_sdk_python.models.status_info import StatusInfo
-from cdo_sdk_python.models.user import User
-from cdo_sdk_python.models.user_create_or_update_input import UserCreateOrUpdateInput
-from cdo_sdk_python.models.user_page import UserPage
+from cdo_sdk_python.models.create_request import CreateRequest
+from cdo_sdk_python.models.duplicate_group_dto import DuplicateGroupDto
+from cdo_sdk_python.models.issues_count import IssuesCount
+from cdo_sdk_python.models.list_object_response import ListObjectResponse
+from cdo_sdk_python.models.object_response import ObjectResponse
+from cdo_sdk_python.models.reference_info import ReferenceInfo
+from cdo_sdk_python.models.targets_request import TargetsRequest
+from cdo_sdk_python.models.update_request import UpdateRequest
 
 from cdo_sdk_python.api_client import ApiClient, RequestSerialized
 from cdo_sdk_python.api_response import ApiResponse
 from cdo_sdk_python.rest import RESTResponseType
 
 
-class UsersApi:
+class ObjectManagementApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def create_user(
+    def create_object(
         self,
-        user_create_or_update_input: UserCreateOrUpdateInput,
+        create_request: CreateRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> User:
-        """Create a user in the CDO tenant
+    ) -> ObjectResponse:
+        """Create Object
 
+        Create an object in the CDO tenant.
 
-        :param user_create_or_update_input: (required)
-        :type user_create_or_update_input: UserCreateOrUpdateInput
+        :param create_request: (required)
+        :type create_request: CreateRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -85,24 +88,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_user_serialize(
-            user_create_or_update_input=user_create_or_update_input,
+        _param = self._create_object_serialize(
+            create_request=create_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "User",
+            '201': "ObjectResponse",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -112,35 +115,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_user_with_http_info(
+    def create_object_with_http_info(
         self,
-        user_create_or_update_input: UserCreateOrUpdateInput,
+        create_request: CreateRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[User]:
-        """Create a user in the CDO tenant
+    ) -> ApiResponse[ObjectResponse]:
+        """Create Object
 
+        Create an object in the CDO tenant.
 
-        :param user_create_or_update_input: (required)
-        :type user_create_or_update_input: UserCreateOrUpdateInput
+        :param create_request: (required)
+        :type create_request: CreateRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -155,24 +159,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_user_serialize(
-            user_create_or_update_input=user_create_or_update_input,
+        _param = self._create_object_serialize(
+            create_request=create_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "User",
+            '201': "ObjectResponse",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -182,35 +186,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_user_without_preload_content(
+    def create_object_without_preload_content(
         self,
-        user_create_or_update_input: UserCreateOrUpdateInput,
+        create_request: CreateRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create a user in the CDO tenant
+        """Create Object
 
+        Create an object in the CDO tenant.
 
-        :param user_create_or_update_input: (required)
-        :type user_create_or_update_input: UserCreateOrUpdateInput
+        :param create_request: (required)
+        :type create_request: CreateRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -225,39 +230,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_user_serialize(
-            user_create_or_update_input=user_create_or_update_input,
+        _param = self._create_object_serialize(
+            create_request=create_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "User",
+            '201': "ObjectResponse",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_user_serialize(
+    def _create_object_serialize(
         self,
-        user_create_or_update_input,
+        create_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -273,16 +278,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if user_create_or_update_input is not None:
-            _body_params = user_create_or_update_input
+        if create_request is not None:
+            _body_params = create_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -300,20 +305,19 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/v1/users',
+            resource_path='/v0/objects',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -322,35 +326,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def delete_user(
+    def create_targets(
         self,
-        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="the unique identifier of the object for which the targets are being added to.")],
+        targets_request: TargetsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> None:
-        """Delete a User by UID in the CDO tenant
+    ) -> object:
+        """Create Targets
 
+        Create targets for an object in the CDO tenant.
 
-        :param user_uid: The unique identifier of the user in CDO. (required)
-        :type user_uid: str
+        :param uid: the unique identifier of the object for which the targets are being added to. (required)
+        :type uid: str
+        :param targets_request: (required)
+        :type targets_request: TargetsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -365,62 +373,68 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_user_serialize(
-            user_uid=user_uid,
+        _param = self._create_targets_serialize(
+            uid=uid,
+            targets_request=targets_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': None,
+            '200': "object",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def delete_user_with_http_info(
+    def create_targets_with_http_info(
         self,
-        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="the unique identifier of the object for which the targets are being added to.")],
+        targets_request: TargetsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[None]:
-        """Delete a User by UID in the CDO tenant
+    ) -> ApiResponse[object]:
+        """Create Targets
 
+        Create targets for an object in the CDO tenant.
 
-        :param user_uid: The unique identifier of the user in CDO. (required)
-        :type user_uid: str
+        :param uid: the unique identifier of the object for which the targets are being added to. (required)
+        :type uid: str
+        :param targets_request: (required)
+        :type targets_request: TargetsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -435,62 +449,68 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_user_serialize(
-            user_uid=user_uid,
+        _param = self._create_targets_serialize(
+            uid=uid,
+            targets_request=targets_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': None,
+            '200': "object",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def delete_user_without_preload_content(
+    def create_targets_without_preload_content(
         self,
-        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="the unique identifier of the object for which the targets are being added to.")],
+        targets_request: TargetsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Delete a User by UID in the CDO tenant
+        """Create Targets
 
+        Create targets for an object in the CDO tenant.
 
-        :param user_uid: The unique identifier of the user in CDO. (required)
-        :type user_uid: str
+        :param uid: the unique identifier of the object for which the targets are being added to. (required)
+        :type uid: str
+        :param targets_request: (required)
+        :type targets_request: TargetsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -505,39 +525,42 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._delete_user_serialize(
-            user_uid=user_uid,
+        _param = self._create_targets_serialize(
+            uid=uid,
+            targets_request=targets_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': None,
+            '200': "object",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _delete_user_serialize(
+    def _create_targets_serialize(
         self,
-        user_uid,
+        uid,
+        targets_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -549,38 +572,323 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if user_uid is not None:
-            _path_params['userUid'] = user_uid
+        if uid is not None:
+            _path_params['uid'] = uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if targets_request is not None:
+            _body_params = targets_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
+                '*/*', 
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/v0/objects/{uid}/targets',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def delete_object(
+        self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being deleted.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> object:
+        """Delete Object
+
+        Delete an object in the CDO tenant
+
+        :param uid: The unique identifier of the object being deleted. (required)
+        :type uid: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_object_serialize(
+            uid=uid,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '204': "object",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def delete_object_with_http_info(
+        self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being deleted.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[object]:
+        """Delete Object
+
+        Delete an object in the CDO tenant
+
+        :param uid: The unique identifier of the object being deleted. (required)
+        :type uid: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_object_serialize(
+            uid=uid,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '204': "object",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def delete_object_without_preload_content(
+        self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being deleted.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Delete Object
+
+        Delete an object in the CDO tenant
+
+        :param uid: The unique identifier of the object being deleted. (required)
+        :type uid: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._delete_object_serialize(
+            uid=uid,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '204': "object",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _delete_object_serialize(
+        self,
+        uid,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if uid is not None:
+            _path_params['uid'] = uid
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                '*/*', 
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/v1/users/{userUid}',
+            resource_path='/v0/objects/{uid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -589,35 +897,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def generate_api_token(
+    def delete_targets(
         self,
-        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="the unique identifier of the object for which the targets are being removed from.")],
+        target_uuids: Annotated[List[StrictStr], Field(description="The list of UIDs of the targets being removed.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiTokenInfo:
-        """Generate API Token for API-only user
+    ) -> object:
+        """Delete Targets
 
+        Delete targets from an object in the CDO tenant.
 
-        :param api_user_id: The unique identifier of the API user in CDO. (required)
-        :type api_user_id: str
+        :param uid: the unique identifier of the object for which the targets are being removed from. (required)
+        :type uid: str
+        :param target_uuids: The list of UIDs of the targets being removed. (required)
+        :type target_uuids: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -632,62 +944,68 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._generate_api_token_serialize(
-            api_user_id=api_user_id,
+        _param = self._delete_targets_serialize(
+            uid=uid,
+            target_uuids=target_uuids,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "ApiTokenInfo",
+            '204': "object",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def generate_api_token_with_http_info(
+    def delete_targets_with_http_info(
         self,
-        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="the unique identifier of the object for which the targets are being removed from.")],
+        target_uuids: Annotated[List[StrictStr], Field(description="The list of UIDs of the targets being removed.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ApiTokenInfo]:
-        """Generate API Token for API-only user
+    ) -> ApiResponse[object]:
+        """Delete Targets
 
+        Delete targets from an object in the CDO tenant.
 
-        :param api_user_id: The unique identifier of the API user in CDO. (required)
-        :type api_user_id: str
+        :param uid: the unique identifier of the object for which the targets are being removed from. (required)
+        :type uid: str
+        :param target_uuids: The list of UIDs of the targets being removed. (required)
+        :type target_uuids: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -702,62 +1020,68 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._generate_api_token_serialize(
-            api_user_id=api_user_id,
+        _param = self._delete_targets_serialize(
+            uid=uid,
+            target_uuids=target_uuids,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "ApiTokenInfo",
+            '204': "object",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def generate_api_token_without_preload_content(
+    def delete_targets_without_preload_content(
         self,
-        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="the unique identifier of the object for which the targets are being removed from.")],
+        target_uuids: Annotated[List[StrictStr], Field(description="The list of UIDs of the targets being removed.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Generate API Token for API-only user
+        """Delete Targets
 
+        Delete targets from an object in the CDO tenant.
 
-        :param api_user_id: The unique identifier of the API user in CDO. (required)
-        :type api_user_id: str
+        :param uid: the unique identifier of the object for which the targets are being removed from. (required)
+        :type uid: str
+        :param target_uuids: The list of UIDs of the targets being removed. (required)
+        :type target_uuids: List[str]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -772,82 +1096,90 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._generate_api_token_serialize(
-            api_user_id=api_user_id,
+        _param = self._delete_targets_serialize(
+            uid=uid,
+            target_uuids=target_uuids,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "ApiTokenInfo",
+            '204': "object",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
+            '404': "object",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _generate_api_token_serialize(
+    def _delete_targets_serialize(
         self,
-        api_user_id,
+        uid,
+        target_uuids,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
+            'targetUuids': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if api_user_id is not None:
-            _path_params['apiUserId'] = api_user_id
+        if uid is not None:
+            _path_params['uid'] = uid
         # process the query parameters
+        if target_uuids is not None:
+            
+            _query_params.append(('targetUuids', target_uuids))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
+                '*/*', 
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/users/{apiUserId}/apiToken/generate',
+            method='DELETE',
+            resource_path='/v0/objects/{uid}/targets',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -856,32 +1188,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_token(
+    def get_duplicate_objects(
         self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object to retrieve duplicates for.")],
+        target_uid: Annotated[StrictStr, Field(description="the unique identifier of the target to restrict the duplicate search to.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CdoTokenInfo:
-        """Fetch information on the current token
+    ) -> List[DuplicateGroupDto]:
+        """Get Duplicate Objects
 
+        Get objects in the CDO tenant that are duplicates of the given object.
 
+        :param uid: The unique identifier of the object to retrieve duplicates for. (required)
+        :type uid: str
+        :param target_uid: the unique identifier of the target to restrict the duplicate search to. (required)
+        :type target_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -896,56 +1235,67 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_token_serialize(
+        _param = self._get_duplicate_objects_serialize(
+            uid=uid,
+            target_uid=target_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CdoTokenInfo",
+            '200': "List[DuplicateGroupDto]",
+            '400': "CommonApiError",
             '401': "AuthenticationError",
+            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_token_with_http_info(
+    def get_duplicate_objects_with_http_info(
         self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object to retrieve duplicates for.")],
+        target_uid: Annotated[StrictStr, Field(description="the unique identifier of the target to restrict the duplicate search to.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CdoTokenInfo]:
-        """Fetch information on the current token
+    ) -> ApiResponse[List[DuplicateGroupDto]]:
+        """Get Duplicate Objects
 
+        Get objects in the CDO tenant that are duplicates of the given object.
 
+        :param uid: The unique identifier of the object to retrieve duplicates for. (required)
+        :type uid: str
+        :param target_uid: the unique identifier of the target to restrict the duplicate search to. (required)
+        :type target_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -960,56 +1310,67 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_token_serialize(
+        _param = self._get_duplicate_objects_serialize(
+            uid=uid,
+            target_uid=target_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CdoTokenInfo",
+            '200': "List[DuplicateGroupDto]",
+            '400': "CommonApiError",
             '401': "AuthenticationError",
+            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_token_without_preload_content(
+    def get_duplicate_objects_without_preload_content(
         self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object to retrieve duplicates for.")],
+        target_uid: Annotated[StrictStr, Field(description="the unique identifier of the target to restrict the duplicate search to.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch information on the current token
+        """Get Duplicate Objects
 
+        Get objects in the CDO tenant that are duplicates of the given object.
 
+        :param uid: The unique identifier of the object to retrieve duplicates for. (required)
+        :type uid: str
+        :param target_uid: the unique identifier of the target to restrict the duplicate search to. (required)
+        :type target_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1024,35 +1385,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_token_serialize(
+        _param = self._get_duplicate_objects_serialize(
+            uid=uid,
+            target_uid=target_uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CdoTokenInfo",
+            '200': "List[DuplicateGroupDto]",
+            '400': "CommonApiError",
             '401': "AuthenticationError",
+            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_token_serialize(
+    def _get_duplicate_objects_serialize(
         self,
+        uid,
+        target_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1064,15 +1431,21 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if uid is not None:
+            _path_params['uid'] = uid
         # process the query parameters
+        if target_uid is not None:
+            
+            _query_params.append(('targetUid', target_uid))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1080,20 +1453,19 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/token',
+            resource_path='/v0/objects/{uid}/duplicates',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1102,35 +1474,33 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_user(
+    def get_issues_count(
         self,
-        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> User:
-        """Fetch a user by UID in the CDO tenant.
+    ) -> IssuesCount:
+        """Get Issues Count
 
+        Get issues count in the CDO tenant.
 
-        :param user_uid: The unique identifier of the user in CDO. (required)
-        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1145,63 +1515,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_user_serialize(
-            user_uid=user_uid,
+        _param = self._get_issues_count_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
+            '200': "IssuesCount",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_user_with_http_info(
+    def get_issues_count_with_http_info(
         self,
-        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[User]:
-        """Fetch a user by UID in the CDO tenant.
+    ) -> ApiResponse[IssuesCount]:
+        """Get Issues Count
 
+        Get issues count in the CDO tenant.
 
-        :param user_uid: The unique identifier of the user in CDO. (required)
-        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1216,63 +1582,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_user_serialize(
-            user_uid=user_uid,
+        _param = self._get_issues_count_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
+            '200': "IssuesCount",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_user_without_preload_content(
+    def get_issues_count_without_preload_content(
         self,
-        user_uid: Annotated[StrictStr, Field(description="The unique identifier of the user in CDO.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a user by UID in the CDO tenant.
+        """Get Issues Count
 
+        Get issues count in the CDO tenant.
 
-        :param user_uid: The unique identifier of the user in CDO. (required)
-        :type user_uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1287,40 +1649,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_user_serialize(
-            user_uid=user_uid,
+        _param = self._get_issues_count_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "User",
+            '200': "IssuesCount",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
-            '404': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_user_serialize(
+    def _get_issues_count_serialize(
         self,
-        user_uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1332,16 +1691,14 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if user_uid is not None:
-            _path_params['userUid'] = user_uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1350,20 +1707,19 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/users/{userUid}',
+            resource_path='/v0/objects/issues-count',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1372,41 +1728,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def list_users(
+    def get_object(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being retrieved.")],
+        fields: Annotated[Optional[StrictStr], Field(description="The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> UserPage:
-        """Fetch a list of users associated with the CDO tenant.
+    ) -> ObjectResponse:
+        """Get Object
 
+        Gets an object in the CDO tenant
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
+        :param uid: The unique identifier of the object being retrieved. (required)
+        :type uid: str
+        :param fields: The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".
+        :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1421,26 +1775,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_users_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
+        _param = self._get_object_serialize(
+            uid=uid,
+            fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "UserPage",
+            '200': "ObjectResponse",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1450,41 +1803,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def list_users_with_http_info(
+    def get_object_with_http_info(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being retrieved.")],
+        fields: Annotated[Optional[StrictStr], Field(description="The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[UserPage]:
-        """Fetch a list of users associated with the CDO tenant.
+    ) -> ApiResponse[ObjectResponse]:
+        """Get Object
 
+        Gets an object in the CDO tenant
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
+        :param uid: The unique identifier of the object being retrieved. (required)
+        :type uid: str
+        :param fields: The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".
+        :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1499,26 +1850,25 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_users_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
+        _param = self._get_object_serialize(
+            uid=uid,
+            fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "UserPage",
+            '200': "ObjectResponse",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1528,41 +1878,39 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def list_users_without_preload_content(
+    def get_object_without_preload_content(
         self,
-        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
-        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
-        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being retrieved.")],
+        fields: Annotated[Optional[StrictStr], Field(description="The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Fetch a list of users associated with the CDO tenant.
+        """Get Object
 
+        Gets an object in the CDO tenant
 
-        :param limit: The number of results to retrieve.
-        :type limit: str
-        :param offset: The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
-        :type offset: str
-        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
-        :type q: str
+        :param uid: The unique identifier of the object being retrieved. (required)
+        :type uid: str
+        :param fields: The scope of the fields to be retrieved. One of [\"@basic\", \"@detailed\"]. Defaults to \"@basic\".
+        :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1577,43 +1925,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._list_users_serialize(
-            limit=limit,
-            offset=offset,
-            q=q,
+        _param = self._get_object_serialize(
+            uid=uid,
+            fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "UserPage",
+            '200': "ObjectResponse",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _list_users_serialize(
+    def _get_object_serialize(
         self,
-        limit,
-        offset,
-        q,
+        uid,
+        fields,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1625,26 +1971,20 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if uid is not None:
+            _path_params['uid'] = uid
         # process the query parameters
-        if limit is not None:
+        if fields is not None:
             
-            _query_params.append(('limit', limit))
-            
-        if offset is not None:
-            
-            _query_params.append(('offset', offset))
-            
-        if q is not None:
-            
-            _query_params.append(('q', q))
+            _query_params.append(('fields', fields))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1653,20 +1993,19 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/v1/users',
+            resource_path='/v0/objects/{uid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1675,35 +2014,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def revoke_api_token(
+    def get_object_usages(
         self,
-        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object to retrieve usages for.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> StatusInfo:
-        """Revoke API Token of API-only user
+    ) -> List[ReferenceInfo]:
+        """Get Object Usages
 
+        Get usages of an object in the CDO tenant.
 
-        :param api_user_id: The unique identifier of the API user in CDO. (required)
-        :type api_user_id: str
+        :param uid: The unique identifier of the object to retrieve usages for. (required)
+        :type uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1718,24 +2058,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._revoke_api_token_serialize(
-            api_user_id=api_user_id,
+        _param = self._get_object_usages_serialize(
+            uid=uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "StatusInfo",
+            '200': "List[ReferenceInfo]",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1745,35 +2085,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def revoke_api_token_with_http_info(
+    def get_object_usages_with_http_info(
         self,
-        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object to retrieve usages for.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[StatusInfo]:
-        """Revoke API Token of API-only user
+    ) -> ApiResponse[List[ReferenceInfo]]:
+        """Get Object Usages
 
+        Get usages of an object in the CDO tenant.
 
-        :param api_user_id: The unique identifier of the API user in CDO. (required)
-        :type api_user_id: str
+        :param uid: The unique identifier of the object to retrieve usages for. (required)
+        :type uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1788,24 +2129,24 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._revoke_api_token_serialize(
-            api_user_id=api_user_id,
+        _param = self._get_object_usages_serialize(
+            uid=uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "StatusInfo",
+            '200': "List[ReferenceInfo]",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -1815,35 +2156,36 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def revoke_api_token_without_preload_content(
+    def get_object_usages_without_preload_content(
         self,
-        api_user_id: Annotated[StrictStr, Field(description="The unique identifier of the API user in CDO.")],
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object to retrieve usages for.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Revoke API Token of API-only user
+        """Get Object Usages
 
+        Get usages of an object in the CDO tenant.
 
-        :param api_user_id: The unique identifier of the API user in CDO. (required)
-        :type api_user_id: str
+        :param uid: The unique identifier of the object to retrieve usages for. (required)
+        :type uid: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1858,39 +2200,39 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._revoke_api_token_serialize(
-            api_user_id=api_user_id,
+        _param = self._get_object_usages_serialize(
+            uid=uid,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "StatusInfo",
+            '200': "List[ReferenceInfo]",
             '400': "CommonApiError",
             '401': "AuthenticationError",
             '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _revoke_api_token_serialize(
+    def _get_object_usages_serialize(
         self,
-        api_user_id,
+        uid,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -1902,16 +2244,16 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if api_user_id is not None:
-            _path_params['apiUserId'] = api_user_id
+        if uid is not None:
+            _path_params['uid'] = uid
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1920,20 +2262,19 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/users/{apiUserId}/apiToken/revoke',
+            method='GET',
+            resource_path='/v0/objects/{uid}/usage',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1942,32 +2283,45 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def revoke_token(
+    def get_objects(
         self,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        sort_by: Annotated[Optional[StrictStr], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> None:
-        """Revoke the current token
+    ) -> ListObjectResponse:
+        """Get Objects
 
+        Get objects in the CDO tenant.
 
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param sort_by: The fields to sort results by.
+        :type sort_by: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1982,56 +2336,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._revoke_token_serialize(
+        _param = self._get_objects_serialize(
+            q=q,
+            offset=offset,
+            limit=limit,
+            sort_by=sort_by,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': None,
+            '200': "ListObjectResponse",
+            '400': "CommonApiError",
             '401': "AuthenticationError",
+            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def revoke_token_with_http_info(
+    def get_objects_with_http_info(
         self,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        sort_by: Annotated[Optional[StrictStr], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[None]:
-        """Revoke the current token
+    ) -> ApiResponse[ListObjectResponse]:
+        """Get Objects
 
+        Get objects in the CDO tenant.
 
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param sort_by: The fields to sort results by.
+        :type sort_by: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2046,56 +2419,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._revoke_token_serialize(
+        _param = self._get_objects_serialize(
+            q=q,
+            offset=offset,
+            limit=limit,
+            sort_by=sort_by,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': None,
+            '200': "ListObjectResponse",
+            '400': "CommonApiError",
             '401': "AuthenticationError",
+            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def revoke_token_without_preload_content(
+    def get_objects_without_preload_content(
         self,
+        q: Annotated[Optional[StrictStr], Field(description="The query to execute. Use the Lucene Query Syntax to construct your query.")] = None,
+        offset: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")] = None,
+        limit: Annotated[Optional[Annotated[str, Field(strict=True)]], Field(description="The number of results to retrieve.")] = None,
+        sort_by: Annotated[Optional[StrictStr], Field(description="The fields to sort results by.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Revoke the current token
+        """Get Objects
 
+        Get objects in the CDO tenant.
 
+        :param q: The query to execute. Use the Lucene Query Syntax to construct your query.
+        :type q: str
+        :param offset: The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.
+        :type offset: str
+        :param limit: The number of results to retrieve.
+        :type limit: str
+        :param sort_by: The fields to sort results by.
+        :type sort_by: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2110,35 +2502,45 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._revoke_token_serialize(
+        _param = self._get_objects_serialize(
+            q=q,
+            offset=offset,
+            limit=limit,
+            sort_by=sort_by,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': None,
+            '200': "ListObjectResponse",
+            '400': "CommonApiError",
             '401': "AuthenticationError",
+            '403': "CommonApiError",
             '500': "CommonApiError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _revoke_token_serialize(
+    def _get_objects_serialize(
         self,
+        q,
+        offset,
+        limit,
+        sort_by,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -2151,14 +2553,30 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if q is not None:
+            
+            _query_params.append(('q', q))
+            
+        if offset is not None:
+            
+            _query_params.append(('offset', offset))
+            
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if sort_by is not None:
+            
+            _query_params.append(('sortBy', sort_by))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -2166,20 +2584,316 @@
                 'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
-            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/v1/token/revoke',
+            method='GET',
+            resource_path='/v0/objects',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def modify_object(
+        self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being updated.")],
+        update_request: UpdateRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ObjectResponse:
+        """Modify Object
+
+        Modify an object in the CDO tenant
+
+        :param uid: The unique identifier of the object being updated. (required)
+        :type uid: str
+        :param update_request: (required)
+        :type update_request: UpdateRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_object_serialize(
+            uid=uid,
+            update_request=update_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ObjectResponse",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def modify_object_with_http_info(
+        self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being updated.")],
+        update_request: UpdateRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ObjectResponse]:
+        """Modify Object
+
+        Modify an object in the CDO tenant
+
+        :param uid: The unique identifier of the object being updated. (required)
+        :type uid: str
+        :param update_request: (required)
+        :type update_request: UpdateRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_object_serialize(
+            uid=uid,
+            update_request=update_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ObjectResponse",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def modify_object_without_preload_content(
+        self,
+        uid: Annotated[StrictStr, Field(description="The unique identifier of the object being updated.")],
+        update_request: UpdateRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Modify Object
+
+        Modify an object in the CDO tenant
+
+        :param uid: The unique identifier of the object being updated. (required)
+        :type uid: str
+        :param update_request: (required)
+        :type update_request: UpdateRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._modify_object_serialize(
+            uid=uid,
+            update_request=update_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ObjectResponse",
+            '400': "CommonApiError",
+            '401': "AuthenticationError",
+            '403': "CommonApiError",
+            '500': "CommonApiError",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _modify_object_serialize(
+        self,
+        uid,
+        update_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if uid is not None:
+            _path_params['uid'] = uid
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if update_request is not None:
+            _body_params = update_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+        ]
+
+        return self.api_client.param_serialize(
+            method='PATCH',
+            resource_path='/v0/objects/{uid}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api_client.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.9/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.90/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/api_response.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/api_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/configuration.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -375,16 +375,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.1\n"\
-               "SDK Package Version: 1.0.9".\
+               "Version of the API: 0.1.0\n"\
+               "SDK Package Version: 1.0.90".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/exceptions.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/__init__.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,110 @@
 # coding: utf-8
 
 # flake8: noqa
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from cdo_sdk_python.models.api_token_info import ApiTokenInfo
 from cdo_sdk_python.models.asa_create_or_update_input import AsaCreateOrUpdateInput
 from cdo_sdk_python.models.asa_failover_mate import AsaFailoverMate
 from cdo_sdk_python.models.asa_failover_mode import AsaFailoverMode
 from cdo_sdk_python.models.authentication_error import AuthenticationError
+from cdo_sdk_python.models.browser import Browser
 from cdo_sdk_python.models.cd_fmc_info import CdFmcInfo
 from cdo_sdk_python.models.cd_fmc_object import CdFmcObject
 from cdo_sdk_python.models.cd_fmc_result import CdFmcResult
+from cdo_sdk_python.models.cdo_cli_macro import CdoCliMacro
+from cdo_sdk_python.models.cdo_cli_macro_page import CdoCliMacroPage
+from cdo_sdk_python.models.cdo_cli_result import CdoCliResult
+from cdo_sdk_python.models.cdo_cli_result_page import CdoCliResultPage
 from cdo_sdk_python.models.cdo_region import CdoRegion
 from cdo_sdk_python.models.cdo_region_list import CdoRegionList
 from cdo_sdk_python.models.cdo_token_info import CdoTokenInfo
 from cdo_sdk_python.models.cdo_transaction import CdoTransaction
 from cdo_sdk_python.models.cdo_transaction_status import CdoTransactionStatus
 from cdo_sdk_python.models.cdo_transaction_type import CdoTransactionType
 from cdo_sdk_python.models.change_request import ChangeRequest
 from cdo_sdk_python.models.change_request_create_input import ChangeRequestCreateInput
 from cdo_sdk_python.models.change_request_page import ChangeRequestPage
 from cdo_sdk_python.models.changelog import Changelog
 from cdo_sdk_python.models.changelog_page import ChangelogPage
+from cdo_sdk_python.models.client_device import ClientDevice
 from cdo_sdk_python.models.common_api_error import CommonApiError
 from cdo_sdk_python.models.config_state import ConfigState
 from cdo_sdk_python.models.conflict_detection_interval import ConflictDetectionInterval
 from cdo_sdk_python.models.conflict_detection_state import ConflictDetectionState
 from cdo_sdk_python.models.connectivity_state import ConnectivityState
 from cdo_sdk_python.models.connector_type import ConnectorType
 from cdo_sdk_python.models.create_request import CreateRequest
 from cdo_sdk_python.models.device import Device
 from cdo_sdk_python.models.device_page import DevicePage
 from cdo_sdk_python.models.device_patch_input import DevicePatchInput
 from cdo_sdk_python.models.device_role import DeviceRole
 from cdo_sdk_python.models.duo_admin_panel_create_or_update_input import DuoAdminPanelCreateOrUpdateInput
+from cdo_sdk_python.models.duplicate_group_dto import DuplicateGroupDto
 from cdo_sdk_python.models.entity import Entity
 from cdo_sdk_python.models.entity_type import EntityType
 from cdo_sdk_python.models.event import Event
 from cdo_sdk_python.models.ftd_create_or_update_input import FtdCreateOrUpdateInput
 from cdo_sdk_python.models.ftd_registration_input import FtdRegistrationInput
 from cdo_sdk_python.models.global_search_result import GlobalSearchResult
 from cdo_sdk_python.models.group_content import GroupContent
 from cdo_sdk_python.models.icmp4_value import Icmp4Value
 from cdo_sdk_python.models.icmp6_value import Icmp6Value
 from cdo_sdk_python.models.inventory import Inventory
 from cdo_sdk_python.models.ios_create_or_update_input import IosCreateOrUpdateInput
+from cdo_sdk_python.models.issues_count import IssuesCount
 from cdo_sdk_python.models.issues_dto import IssuesDto
 from cdo_sdk_python.models.json_web_key import JsonWebKey
 from cdo_sdk_python.models.jwk_set import JwkSet
 from cdo_sdk_python.models.labels import Labels
 from cdo_sdk_python.models.list_object_response import ListObjectResponse
 from cdo_sdk_python.models.location import Location
 from cdo_sdk_python.models.meraki_deployment_mode import MerakiDeploymentMode
 from cdo_sdk_python.models.meta import Meta
+from cdo_sdk_python.models.mfa_event import MfaEvent
+from cdo_sdk_python.models.mfa_event_page import MfaEventPage
 from cdo_sdk_python.models.msp_add_tenant_input import MspAddTenantInput
 from cdo_sdk_python.models.network import Network
 from cdo_sdk_python.models.network_object_content import NetworkObjectContent
 from cdo_sdk_python.models.os import OS
 from cdo_sdk_python.models.object_content import ObjectContent
 from cdo_sdk_python.models.object_response import ObjectResponse
 from cdo_sdk_python.models.on_prem_fmc_info import OnPremFmcInfo
 from cdo_sdk_python.models.override import Override
 from cdo_sdk_python.models.policy import Policy
 from cdo_sdk_python.models.ports_value import PortsValue
+from cdo_sdk_python.models.public_key import PublicKey
+from cdo_sdk_python.models.ra_vpn_device_input import RaVpnDeviceInput
 from cdo_sdk_python.models.ra_vpn_session import RaVpnSession
 from cdo_sdk_python.models.ra_vpn_session_page import RaVpnSessionPage
 from cdo_sdk_python.models.reference_info import ReferenceInfo
 from cdo_sdk_python.models.sdc import Sdc
+from cdo_sdk_python.models.sdc_create_input import SdcCreateInput
 from cdo_sdk_python.models.sdc_page import SdcPage
-from cdo_sdk_python.models.sdc_public_key import SdcPublicKey
-from cdo_sdk_python.models.sdc_status import SdcStatus
+from cdo_sdk_python.models.sdc_patch_input import SdcPatchInput
 from cdo_sdk_python.models.service_object_content import ServiceObjectContent
 from cdo_sdk_python.models.service_object_value_content import ServiceObjectValueContent
 from cdo_sdk_python.models.shared_object_value import SharedObjectValue
 from cdo_sdk_python.models.single_content import SingleContent
 from cdo_sdk_python.models.state_machine_details import StateMachineDetails
 from cdo_sdk_python.models.state_machine_error import StateMachineError
+from cdo_sdk_python.models.status import Status
 from cdo_sdk_python.models.status_info import StatusInfo
 from cdo_sdk_python.models.target import Target
 from cdo_sdk_python.models.targets_request import TargetsRequest
 from cdo_sdk_python.models.tenant import Tenant
 from cdo_sdk_python.models.tenant_page import TenantPage
 from cdo_sdk_python.models.tenant_pay_type import TenantPayType
 from cdo_sdk_python.models.tenant_settings import TenantSettings
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/api_token_info.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/api_token_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_create_or_update_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/asa_create_or_update_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mate.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/asa_failover_mate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/asa_failover_mode.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/sdc_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class AsaFailoverMode(str, Enum):
+class SdcStatus(str, Enum):
     """
-    (ASAs only) Failover mode of the device.
+    The status of the SDC.
     """
 
     """
     allowed enum values
     """
-    OFF = 'OFF'
-    ACTIVE_STANDBY = 'ACTIVE_STANDBY'
-    ACTIVE_ACTIVE = 'ACTIVE_ACTIVE'
+    NEW = 'NEW'
+    ONBOARDING = 'ONBOARDING'
+    ACTIVE = 'ACTIVE'
+    INACTIVE = 'INACTIVE'
+    DISABLED = 'DISABLED'
+    UNKNOWN = 'UNKNOWN'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of AsaFailoverMode from a JSON string"""
+        """Create an instance of SdcStatus from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/authentication_error.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/authentication_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_info.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cd_fmc_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_object.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cd_fmc_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cd_fmc_result.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cd_fmc_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_region.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_region_list.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_region_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_token_info.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_token_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_status.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_transaction_status.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/cdo_transaction_type.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/cdo_transaction_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -34,15 +34,17 @@
     REGISTER_FTD = 'REGISTER_FTD'
     DELETE_CDFMC_MANAGED_FTD = 'DELETE_CDFMC_MANAGED_FTD'
     RECONNECT_ASA = 'RECONNECT_ASA'
     READ_ASA = 'READ_ASA'
     DEPLOY_ASA_DEVICE_CHANGES = 'DEPLOY_ASA_DEVICE_CHANGES'
     INDEX_TENANT = 'INDEX_TENANT'
     TERMINATE_DEVICE_RA_VPN_SESSIONS = 'TERMINATE_DEVICE_RA_VPN_SESSIONS'
+    REFRESH_RA_VPN_SESSIONS = 'REFRESH_RA_VPN_SESSIONS'
     TERMINATE_USER_RA_VPN_SESSIONS = 'TERMINATE_USER_RA_VPN_SESSIONS'
+    CREATE_SDC = 'CREATE_SDC'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Create an instance of CdoTransactionType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/change_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_create_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/change_request_create_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/change_request_page.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/change_request_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,15 +26,15 @@
 
 class ChangeRequestPage(BaseModel):
     """
     ChangeRequestPage
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
     items: Optional[List[ChangeRequest]] = Field(default=None, description="The list of items retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/changelog_page.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/changelog_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,15 +26,15 @@
 
 class ChangelogPage(BaseModel):
     """
     ChangelogPage
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
     items: Optional[List[Changelog]] = Field(default=None, description="The list of items retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/common_api_error.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/common_api_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/config_state.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/config_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_interval.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/conflict_detection_interval.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/conflict_detection_state.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/conflict_detection_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/connectivity_state.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/connectivity_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/connector_type.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class ConnectorType(str, Enum):
+class Status(str, Enum):
     """
-    The type of the connector that will be used to communicate with the device. CDO can communicate with your device using either a Cloud Connector (CDG) or a Secure Device Connector (SDC).
+    The status of the SDC.
     """
 
     """
     allowed enum values
     """
-    SDC = 'SDC'
-    CDG = 'CDG'
+    NEW = 'NEW'
+    ONBOARDING = 'ONBOARDING'
+    ACTIVE = 'ACTIVE'
+    INACTIVE = 'INACTIVE'
+    DISABLED = 'DISABLED'
+    UNKNOWN = 'UNKNOWN'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ConnectorType from a JSON string"""
+        """Create an instance of Status from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/create_request.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_page.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/device_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,15 +26,15 @@
 
 class DevicePage(BaseModel):
     """
     DevicePage
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
     items: Optional[List[Device]] = Field(default=None, description="The list of items retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_patch_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/device_patch_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/device_role.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/device_role.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,14 +26,15 @@
 
     """
     allowed enum values
     """
     RA_VPN_HEADEND = 'RA_VPN_HEADEND'
     MFA_PROVIDER = 'MFA_PROVIDER'
     ZTNA_PROVIDER = 'ZTNA_PROVIDER'
+    ANYCONNECT_VPN_HEAD_END = 'ANYCONNECT_VPN_HEAD_END'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Create an instance of DeviceRole from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/entity_type.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/entity_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/event.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_create_or_update_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/ftd_create_or_update_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ftd_registration_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/ftd_registration_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/global_search_result.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/global_search_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/group_content.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/group_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp4_value.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/icmp4_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/icmp6_value.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/icmp6_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/inventory.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ios_create_or_update_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/ios_create_or_update_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/issues_dto.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,20 +19,21 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class IssuesDto(BaseModel):
+class Policy(BaseModel):
     """
-    The issues for the object
+    Results from the CDO policies that match the search term.
     """ # noqa: E501
-    unused_target_ids: Optional[List[StrictStr]] = Field(default=None, alias="unusedTargetIds")
-    __properties: ClassVar[List[str]] = ["unusedTargetIds"]
+    uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the policy in CDO.")
+    name: Optional[StrictStr] = Field(default=None, description="The name of the policy in CDO.")
+    __properties: ClassVar[List[str]] = ["uid", "name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of IssuesDto from a JSON string"""
+        """Create an instance of Policy from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of IssuesDto from a dict"""
+        """Create an instance of Policy from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "unusedTargetIds": obj.get("unusedTargetIds")
+            "uid": obj.get("uid"),
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/json_web_key.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from cdo_sdk_python.models.user_role import UserRole
 from typing import Optional, Set
 from typing_extensions import Self
 
-class JsonWebKey(BaseModel):
+class User(BaseModel):
     """
-    The JSON Web Key Set.
+    User
     """ # noqa: E501
-    kty: Optional[StrictStr] = Field(default=None, description="The family of cryptographic algorithms used with the key.")
-    e: Optional[StrictStr] = Field(default=None, description="The exponent for the RSA public key.")
-    use: Optional[StrictStr] = Field(default=None, description="How the key was meant to be used.")
-    kid: Optional[StrictStr] = Field(default=None, description="The unique identifier for the key.")
-    alg: Optional[StrictStr] = Field(default=None, description="The specific cryptographic algorithm used with the key.")
-    n: Optional[StrictStr] = Field(default=None, description="The modulus for the RSA public key.")
-    __properties: ClassVar[List[str]] = ["kty", "e", "use", "kid", "alg", "n"]
+    uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the SDC in CDO.")
+    name: Optional[StrictStr] = Field(default=None, description="The name of the user in CDO.")
+    roles: Optional[List[UserRole]] = Field(default=None, description="Roles associated with this user in CDO.")
+    api_only_user: Optional[StrictBool] = Field(default=None, description="Whether the user is API-only, an API-only user cannot access CDO in the UI.", alias="apiOnlyUser")
+    last_successful_login: Optional[datetime] = Field(default=None, description="The time (UTC; represented using the RFC-3339 standard) that indicate the last time the user successfully login CDO.", alias="lastSuccessfulLogin")
+    __properties: ClassVar[List[str]] = ["uid", "name", "roles", "apiOnlyUser", "lastSuccessfulLogin"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -49,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of JsonWebKey from a JSON string"""
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,25 +75,24 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of JsonWebKey from a dict"""
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "kty": obj.get("kty"),
-            "e": obj.get("e"),
-            "use": obj.get("use"),
-            "kid": obj.get("kid"),
-            "alg": obj.get("alg"),
-            "n": obj.get("n")
+            "uid": obj.get("uid"),
+            "name": obj.get("name"),
+            "roles": obj.get("roles"),
+            "apiOnlyUser": obj.get("apiOnlyUser"),
+            "lastSuccessfulLogin": obj.get("lastSuccessfulLogin")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/jwk_set.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/jwk_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/labels.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/list_object_response.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/list_object_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -27,15 +27,15 @@
 
 class ListObjectResponse(BaseModel):
     """
     ListObjectResponse
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[Annotated[int, Field(le=200, strict=True)]] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
     items: Optional[List[UnifiedObjectListView]] = Field(default=None, description="The list of objects retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/location.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/targets_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,22 +19,20 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Location(BaseModel):
+class TargetsRequest(BaseModel):
     """
-    The location information of the device associated with the RA VPN session.
+    TargetsRequest
     """ # noqa: E501
-    city: Optional[StrictStr] = Field(default=None, description="The city where the device associated with the RA VPN session is located.")
-    subdivision: Optional[StrictStr] = Field(default=None, description="The subdivision (e.g., state or province) where the device is located.")
-    country: Optional[StrictStr] = Field(default=None, description="The country where the device associated with the RA VPN session is located.")
-    __properties: ClassVar[List[str]] = ["city", "subdivision", "country"]
+    targets_uuids: Optional[List[StrictStr]] = Field(default=None, description="The list of UIDs of the targets to be deleted.", alias="targetsUuids")
+    __properties: ClassVar[List[str]] = ["targetsUuids"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Location from a JSON string"""
+        """Create an instance of TargetsRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,22 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Location from a dict"""
+        """Create an instance of TargetsRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "city": obj.get("city"),
-            "subdivision": obj.get("subdivision"),
-            "country": obj.get("country")
+            "targetsUuids": obj.get("targetsUuids")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/meraki_deployment_mode.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/meraki_deployment_mode.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/meta.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/msp_add_tenant_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/msp_add_tenant_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/network.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/network_object_content.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/network_object_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_content.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/object_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/object_response.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/object_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/on_prem_fmc_info.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/on_prem_fmc_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/os.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/browser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,21 +19,21 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OS(BaseModel):
+class Browser(BaseModel):
     """
-    The operating system information of the device associated with the RA VPN session.
+    The web browser running on the client device.
     """ # noqa: E501
-    type: Optional[StrictStr] = Field(default=None, description="The type of operating system running on the device associated with the RA VPN session.")
-    version: Optional[StrictStr] = Field(default=None, description="The version of the operating system running on the device.")
-    __properties: ClassVar[List[str]] = ["type", "version"]
+    name: Optional[StrictStr] = Field(default=None, description="The name of the web browser running on the client device.")
+    version: Optional[StrictStr] = Field(default=None, description="The version of the web browser running on the client device.")
+    __properties: ClassVar[List[str]] = ["name", "version"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OS from a JSON string"""
+        """Create an instance of Browser from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OS from a dict"""
+        """Create an instance of Browser from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
+            "name": obj.get("name"),
             "version": obj.get("version")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/override.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/override.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/policy.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/public_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,21 +19,21 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Policy(BaseModel):
+class PublicKey(BaseModel):
     """
-    Results from the CDO policies that match the search term.
+    Information on the public key used to encrypt credentials sent to the SDC.
     """ # noqa: E501
-    uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the policy in CDO.")
-    name: Optional[StrictStr] = Field(default=None, description="The name of the policy in CDO.")
-    __properties: ClassVar[List[str]] = ["uid", "name"]
+    base64_encoded_key: Optional[StrictStr] = Field(default=None, description="Base64 RSA public key to use to encrypt device credentials sent to the SDC.", alias="base64EncodedKey")
+    key_id: Optional[StrictStr] = Field(default=None, description="The identifier of the RSA public key. This identifier is used by the SDC to know which private key to use to decrypt a string.", alias="keyId")
+    __properties: ClassVar[List[str]] = ["base64EncodedKey", "keyId"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Policy from a JSON string"""
+        """Create an instance of PublicKey from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Policy from a dict"""
+        """Create an instance of PublicKey from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "uid": obj.get("uid"),
-            "name": obj.get("name")
+            "base64EncodedKey": obj.get("base64EncodedKey"),
+            "keyId": obj.get("keyId")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ports_value.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/ports_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/ra_vpn_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/ra_vpn_session_page.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/ra_vpn_session_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,15 +26,15 @@
 
 class RaVpnSessionPage(BaseModel):
     """
     RaVpnSessionPage
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
     items: Optional[List[RaVpnSession]] = Field(default=None, description="The list of items retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/reference_info.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/reference_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/unified_object_list_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from cdo_sdk_python.models.sdc_public_key import SdcPublicKey
-from cdo_sdk_python.models.sdc_status import SdcStatus
+from cdo_sdk_python.models.issues_dto import IssuesDto
+from cdo_sdk_python.models.shared_object_value import SharedObjectValue
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Sdc(BaseModel):
+class UnifiedObjectListView(BaseModel):
     """
-    Sdc
+    The list of objects retrieved.
     """ # noqa: E501
-    sdc_public_key: Optional[SdcPublicKey] = Field(default=None, alias="sdcPublicKey")
-    uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the SDC in CDO.")
-    name: StrictStr = Field(description="The name of the SDC in CDO. SDC names are unique in CDO.")
-    software_version: Optional[StrictStr] = Field(default=None, description="The software version running on the SDC.", alias="softwareVersion")
-    ip_address: Optional[StrictStr] = Field(default=None, description="The IP address of the SDC.", alias="ipAddress")
-    sdc_status: Optional[SdcStatus] = Field(default=None, alias="sdcStatus")
-    last_heartbeat: Optional[datetime] = Field(default=None, description="The time (UTC; represented using the RFC-3339 standard) that a heartbeat was last received from the SDC. This serves as an indicator of the health of the SDC.", alias="lastHeartbeat")
-    __properties: ClassVar[List[str]] = ["sdcPublicKey", "uid", "name", "softwareVersion", "ipAddress", "sdcStatus", "lastHeartbeat"]
+    uid: Optional[StrictStr] = None
+    name: Optional[StrictStr] = None
+    description: Optional[StrictStr] = None
+    value: Optional[SharedObjectValue] = None
+    target_ids: Optional[List[StrictStr]] = Field(default=None, alias="targetIds")
+    override_ids: Optional[List[StrictStr]] = Field(default=None, alias="overrideIds")
+    tags: Optional[Dict[str, List[StrictStr]]] = None
+    labels: Optional[List[StrictStr]] = None
+    issues: Optional[IssuesDto] = None
+    __properties: ClassVar[List[str]] = ["uid", "name", "description", "value", "targetIds", "overrideIds", "tags", "labels", "issues"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -53,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Sdc from a JSON string"""
+        """Create an instance of UnifiedObjectListView from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,33 +75,38 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of sdc_public_key
-        if self.sdc_public_key:
-            _dict['sdcPublicKey'] = self.sdc_public_key.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of value
+        if self.value:
+            _dict['value'] = self.value.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of issues
+        if self.issues:
+            _dict['issues'] = self.issues.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Sdc from a dict"""
+        """Create an instance of UnifiedObjectListView from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "sdcPublicKey": SdcPublicKey.from_dict(obj["sdcPublicKey"]) if obj.get("sdcPublicKey") is not None else None,
             "uid": obj.get("uid"),
             "name": obj.get("name"),
-            "softwareVersion": obj.get("softwareVersion"),
-            "ipAddress": obj.get("ipAddress"),
-            "sdcStatus": obj.get("sdcStatus"),
-            "lastHeartbeat": obj.get("lastHeartbeat")
+            "description": obj.get("description"),
+            "value": SharedObjectValue.from_dict(obj["value"]) if obj.get("value") is not None else None,
+            "targetIds": obj.get("targetIds"),
+            "overrideIds": obj.get("overrideIds"),
+            "tags": obj.get("tags"),
+            "labels": obj.get("labels"),
+            "issues": IssuesDto.from_dict(obj["issues"]) if obj.get("issues") is not None else None
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_page.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/sdc_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,15 +26,15 @@
 
 class SdcPage(BaseModel):
     """
     SdcPage
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
     items: Optional[List[Sdc]] = Field(default=None, description="The list of items retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sdc_public_key.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/sdc_public_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_content.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/service_object_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -34,16 +34,16 @@
 
     @field_validator('protocol')
     def protocol_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['TCP', 'UDP', 'ICMP4', 'ICMP6', 'TCP_UDP', 'IGMP', 'GGP', 'ST2', 'CBT', 'EGP', 'IGP', 'BBNRCCMON', 'NVP2', 'PUP', 'ARGUS', 'EMCON', 'XNET', 'CHAOS', 'MUX', 'DCNMEAS', 'HMP', 'PRM', 'XNSIDP', 'TRUNK1', 'TRUNK2', 'LEAF1', 'LEAF2', 'RDP', 'IRTP', 'ISOTP4', 'NETBLT', 'MFENSP', 'MERITINP', 'SEP', 'THREEPC', 'IDPR', 'XTP', 'DDP', 'IDPRCMTP', 'TPPLUSPLUS', 'IL', 'SDRP', 'IDRP', 'RSVP', 'GRE', 'MHRP', 'BNA', 'ESP', 'AH', 'INLSP', 'SWIPE', 'NARP', 'MOBILE', 'TLSP', 'SKIP', 'IPv6NONXT', 'CFTP', 'SATEXPAK', 'KRYPTOLAN', 'RVD', 'IPPC', 'SATMON', 'VISA', 'IPCV', 'CPNX', 'CPHB', 'WSN', 'PVP', 'BRSATMON', 'SUNND', 'WBMON', 'WBEXPAK', 'ISOIP', 'VMTP', 'SECUREVMTP', 'VINES', 'TTP', 'NSFNETIGP', 'DGP', 'TCF', 'EIGRP', 'OSPFIGP', 'SPRITERPC', 'LARP', 'MTP', 'AX25', 'IPIP', 'MICP', 'SCCSP', 'ETHERIP', 'ENCAP', 'GMTP', 'IFMP', 'PNNI', 'PIM', 'ARIS', 'SCPS', 'QNX', 'AN', 'IPCOMP', 'SNP', 'COMPAQPEER', 'IPXINIP', 'VRRP', 'PGM', 'L2TP', 'DDX', 'IATP', 'ST', 'SRP', 'UTI', 'SMP', 'SM', 'PTP', 'ISIS', 'FIRE', 'CRTP', 'CRUDP', 'SSCOPMCE', 'IPLT', 'SPS', 'PIPE', 'SCTP', 'FC', 'DIVERT']):
-            raise ValueError("must be one of enum values ('TCP', 'UDP', 'ICMP4', 'ICMP6', 'TCP_UDP', 'IGMP', 'GGP', 'ST2', 'CBT', 'EGP', 'IGP', 'BBNRCCMON', 'NVP2', 'PUP', 'ARGUS', 'EMCON', 'XNET', 'CHAOS', 'MUX', 'DCNMEAS', 'HMP', 'PRM', 'XNSIDP', 'TRUNK1', 'TRUNK2', 'LEAF1', 'LEAF2', 'RDP', 'IRTP', 'ISOTP4', 'NETBLT', 'MFENSP', 'MERITINP', 'SEP', 'THREEPC', 'IDPR', 'XTP', 'DDP', 'IDPRCMTP', 'TPPLUSPLUS', 'IL', 'SDRP', 'IDRP', 'RSVP', 'GRE', 'MHRP', 'BNA', 'ESP', 'AH', 'INLSP', 'SWIPE', 'NARP', 'MOBILE', 'TLSP', 'SKIP', 'IPv6NONXT', 'CFTP', 'SATEXPAK', 'KRYPTOLAN', 'RVD', 'IPPC', 'SATMON', 'VISA', 'IPCV', 'CPNX', 'CPHB', 'WSN', 'PVP', 'BRSATMON', 'SUNND', 'WBMON', 'WBEXPAK', 'ISOIP', 'VMTP', 'SECUREVMTP', 'VINES', 'TTP', 'NSFNETIGP', 'DGP', 'TCF', 'EIGRP', 'OSPFIGP', 'SPRITERPC', 'LARP', 'MTP', 'AX25', 'IPIP', 'MICP', 'SCCSP', 'ETHERIP', 'ENCAP', 'GMTP', 'IFMP', 'PNNI', 'PIM', 'ARIS', 'SCPS', 'QNX', 'AN', 'IPCOMP', 'SNP', 'COMPAQPEER', 'IPXINIP', 'VRRP', 'PGM', 'L2TP', 'DDX', 'IATP', 'ST', 'SRP', 'UTI', 'SMP', 'SM', 'PTP', 'ISIS', 'FIRE', 'CRTP', 'CRUDP', 'SSCOPMCE', 'IPLT', 'SPS', 'PIPE', 'SCTP', 'FC', 'DIVERT')")
+        if value not in set(['TCP', 'UDP', 'ICMP', 'ICMP4', 'ICMP6', 'TCP_UDP', 'IGMP', 'GGP', 'ST2', 'CBT', 'EGP', 'IGP', 'BBNRCCMON', 'NVP2', 'PUP', 'ARGUS', 'EMCON', 'XNET', 'CHAOS', 'MUX', 'DCNMEAS', 'HMP', 'PRM', 'XNSIDP', 'TRUNK1', 'TRUNK2', 'LEAF1', 'LEAF2', 'RDP', 'IRTP', 'ISOTP4', 'NETBLT', 'MFENSP', 'MERITINP', 'SEP', 'THREEPC', 'IDPR', 'XTP', 'DDP', 'IDPRCMTP', 'TPPLUSPLUS', 'IL', 'SDRP', 'IDRP', 'RSVP', 'GRE', 'MHRP', 'BNA', 'ESP', 'AH', 'INLSP', 'SWIPE', 'NARP', 'MOBILE', 'TLSP', 'SKIP', 'IPv6NONXT', 'CFTP', 'SATEXPAK', 'KRYPTOLAN', 'RVD', 'IPPC', 'SATMON', 'VISA', 'IPCV', 'CPNX', 'CPHB', 'WSN', 'PVP', 'BRSATMON', 'SUNND', 'WBMON', 'WBEXPAK', 'ISOIP', 'VMTP', 'SECUREVMTP', 'VINES', 'TTP', 'NSFNETIGP', 'DGP', 'TCF', 'EIGRP', 'OSPFIGP', 'SPRITERPC', 'LARP', 'MTP', 'AX25', 'IPIP', 'MICP', 'SCCSP', 'ETHERIP', 'ENCAP', 'GMTP', 'IFMP', 'PNNI', 'PIM', 'ARIS', 'SCPS', 'QNX', 'AN', 'IPCOMP', 'SNP', 'COMPAQPEER', 'IPXINIP', 'VRRP', 'PGM', 'L2TP', 'DDX', 'IATP', 'ST', 'SRP', 'UTI', 'SMP', 'SM', 'PTP', 'ISIS', 'FIRE', 'CRTP', 'CRUDP', 'SSCOPMCE', 'IPLT', 'SPS', 'PIPE', 'SCTP', 'FC', 'DIVERT']):
+            raise ValueError("must be one of enum values ('TCP', 'UDP', 'ICMP', 'ICMP4', 'ICMP6', 'TCP_UDP', 'IGMP', 'GGP', 'ST2', 'CBT', 'EGP', 'IGP', 'BBNRCCMON', 'NVP2', 'PUP', 'ARGUS', 'EMCON', 'XNET', 'CHAOS', 'MUX', 'DCNMEAS', 'HMP', 'PRM', 'XNSIDP', 'TRUNK1', 'TRUNK2', 'LEAF1', 'LEAF2', 'RDP', 'IRTP', 'ISOTP4', 'NETBLT', 'MFENSP', 'MERITINP', 'SEP', 'THREEPC', 'IDPR', 'XTP', 'DDP', 'IDPRCMTP', 'TPPLUSPLUS', 'IL', 'SDRP', 'IDRP', 'RSVP', 'GRE', 'MHRP', 'BNA', 'ESP', 'AH', 'INLSP', 'SWIPE', 'NARP', 'MOBILE', 'TLSP', 'SKIP', 'IPv6NONXT', 'CFTP', 'SATEXPAK', 'KRYPTOLAN', 'RVD', 'IPPC', 'SATMON', 'VISA', 'IPCV', 'CPNX', 'CPHB', 'WSN', 'PVP', 'BRSATMON', 'SUNND', 'WBMON', 'WBEXPAK', 'ISOIP', 'VMTP', 'SECUREVMTP', 'VINES', 'TTP', 'NSFNETIGP', 'DGP', 'TCF', 'EIGRP', 'OSPFIGP', 'SPRITERPC', 'LARP', 'MTP', 'AX25', 'IPIP', 'MICP', 'SCCSP', 'ETHERIP', 'ENCAP', 'GMTP', 'IFMP', 'PNNI', 'PIM', 'ARIS', 'SCPS', 'QNX', 'AN', 'IPCOMP', 'SNP', 'COMPAQPEER', 'IPXINIP', 'VRRP', 'PGM', 'L2TP', 'DDX', 'IATP', 'ST', 'SRP', 'UTI', 'SMP', 'SM', 'PTP', 'ISIS', 'FIRE', 'CRTP', 'CRUDP', 'SSCOPMCE', 'IPLT', 'SPS', 'PIPE', 'SCTP', 'FC', 'DIVERT')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/service_object_value_content.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/service_object_value_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/shared_object_value.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/shared_object_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/single_content.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/single_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/sort_criteria_param.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/issues_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    API Docs
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,21 +19,21 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SortCriteriaParam(BaseModel):
+class IssuesDto(BaseModel):
     """
-    SortCriteriaParam
+    The issues for the object
     """ # noqa: E501
-    sort: Optional[List[StrictStr]] = None
-    sort_fields: Optional[List[StrictStr]] = Field(default=None, alias="sortFields")
-    __properties: ClassVar[List[str]] = ["sort", "sortFields"]
+    unused_target_ids: Optional[List[StrictStr]] = Field(default=None, alias="unusedTargetIds")
+    duplicate_target_ids: Optional[List[StrictStr]] = Field(default=None, alias="duplicateTargetIds")
+    __properties: ClassVar[List[str]] = ["unusedTargetIds", "duplicateTargetIds"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SortCriteriaParam from a JSON string"""
+        """Create an instance of IssuesDto from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SortCriteriaParam from a dict"""
+        """Create an instance of IssuesDto from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "sort": obj.get("sort"),
-            "sortFields": obj.get("sortFields")
+            "unusedTargetIds": obj.get("unusedTargetIds"),
+            "duplicateTargetIds": obj.get("duplicateTargetIds")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_details.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/state_machine_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/state_machine_error.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/state_machine_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/status_info.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/status_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/target.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/target.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/targets_request.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/url_object_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TargetsRequest(BaseModel):
+class UrlObjectContent(BaseModel):
     """
-    TargetsRequest
+    UrlObjectContent
     """ # noqa: E501
-    targets_uuids: Optional[List[StrictStr]] = Field(default=None, description="The list of UIDs of the targets to be deleted.", alias="targetsUuids")
-    __properties: ClassVar[List[str]] = ["targetsUuids"]
+    url: StrictStr = Field(description="The URL literal")
+    __properties: ClassVar[List[str]] = ["url"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TargetsRequest from a JSON string"""
+        """Create an instance of UrlObjectContent from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TargetsRequest from a dict"""
+        """Create an instance of UrlObjectContent from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "targetsUuids": obj.get("targetsUuids")
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_page.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -26,15 +26,15 @@
 
 class TenantPage(BaseModel):
     """
     TenantPage
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
     items: Optional[List[Tenant]] = Field(default=None, description="The list of items retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_pay_type.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant_pay_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/tenant_settings.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/tenant_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/unified_object_list_view.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/client_device.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from cdo_sdk_python.models.issues_dto import IssuesDto
-from cdo_sdk_python.models.shared_object_value import SharedObjectValue
+from cdo_sdk_python.models.browser import Browser
+from cdo_sdk_python.models.location import Location
+from cdo_sdk_python.models.os import OS
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UnifiedObjectListView(BaseModel):
+class ClientDevice(BaseModel):
     """
-    The list of objects retrieved.
+    The client device that triggered this MFA event.
     """ # noqa: E501
-    uid: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    description: Optional[StrictStr] = None
-    value: Optional[SharedObjectValue] = None
-    target_ids: Optional[List[StrictStr]] = Field(default=None, alias="targetIds")
-    override_ids: Optional[List[StrictStr]] = Field(default=None, alias="overrideIds")
-    tags: Optional[Dict[str, List[StrictStr]]] = None
-    labels: Optional[List[StrictStr]] = None
-    issues: Optional[IssuesDto] = None
-    __properties: ClassVar[List[str]] = ["uid", "name", "description", "value", "targetIds", "overrideIds", "tags", "labels", "issues"]
+    uid: StrictStr = Field(description="The unique identifier of the device.")
+    location: Optional[Location] = None
+    ip_address: Optional[StrictStr] = Field(default=None, description="The IP address of the client device that has triggered this MFA event.", alias="ipAddress")
+    password_set: Optional[StrictBool] = Field(default=None, description="Indicates whether a password is set on the client device.", alias="passwordSet")
+    encrypted: Optional[StrictBool] = Field(default=None, description="Indicates whether encryption is enabled on the client device.")
+    firewalled: Optional[StrictBool] = Field(default=None, description="Indicates whether a firewall is enabled on the client device.")
+    os: Optional[OS] = None
+    browser: Optional[Browser] = None
+    __properties: ClassVar[List[str]] = ["uid", "location", "ipAddress", "passwordSet", "encrypted", "firewalled", "os", "browser"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -54,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UnifiedObjectListView from a JSON string"""
+        """Create an instance of ClientDevice from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -75,38 +75,40 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of value
-        if self.value:
-            _dict['value'] = self.value.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of issues
-        if self.issues:
-            _dict['issues'] = self.issues.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of location
+        if self.location:
+            _dict['location'] = self.location.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of os
+        if self.os:
+            _dict['os'] = self.os.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of browser
+        if self.browser:
+            _dict['browser'] = self.browser.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UnifiedObjectListView from a dict"""
+        """Create an instance of ClientDevice from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "uid": obj.get("uid"),
-            "name": obj.get("name"),
-            "description": obj.get("description"),
-            "value": SharedObjectValue.from_dict(obj["value"]) if obj.get("value") is not None else None,
-            "targetIds": obj.get("targetIds"),
-            "overrideIds": obj.get("overrideIds"),
-            "tags": obj.get("tags"),
-            "labels": obj.get("labels"),
-            "issues": IssuesDto.from_dict(obj["issues"]) if obj.get("issues") is not None else None
+            "location": Location.from_dict(obj["location"]) if obj.get("location") is not None else None,
+            "ipAddress": obj.get("ipAddress"),
+            "passwordSet": obj.get("passwordSet"),
+            "encrypted": obj.get("encrypted"),
+            "firewalled": obj.get("firewalled"),
+            "os": OS.from_dict(obj["os"]) if obj.get("os") is not None else None,
+            "browser": Browser.from_dict(obj["browser"]) if obj.get("browser") is not None else None
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/update_request.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/update_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/url_object_content.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/json_web_key.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UrlObjectContent(BaseModel):
+class JsonWebKey(BaseModel):
     """
-    UrlObjectContent
+    The JSON Web Key Set.
     """ # noqa: E501
-    url: StrictStr = Field(description="The URL literal")
-    __properties: ClassVar[List[str]] = ["url"]
+    kty: Optional[StrictStr] = Field(default=None, description="The family of cryptographic algorithms used with the key.")
+    e: Optional[StrictStr] = Field(default=None, description="The exponent for the RSA public key.")
+    use: Optional[StrictStr] = Field(default=None, description="How the key was meant to be used.")
+    kid: Optional[StrictStr] = Field(default=None, description="The unique identifier for the key.")
+    alg: Optional[StrictStr] = Field(default=None, description="The specific cryptographic algorithm used with the key.")
+    n: Optional[StrictStr] = Field(default=None, description="The modulus for the RSA public key.")
+    __properties: ClassVar[List[str]] = ["kty", "e", "use", "kid", "alg", "n"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UrlObjectContent from a JSON string"""
+        """Create an instance of JsonWebKey from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +74,25 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UrlObjectContent from a dict"""
+        """Create an instance of JsonWebKey from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "url": obj.get("url")
+            "kty": obj.get("kty"),
+            "e": obj.get("e"),
+            "use": obj.get("use"),
+            "kid": obj.get("kid"),
+            "alg": obj.get("alg"),
+            "n": obj.get("n")
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/user_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from cdo_sdk_python.models.user_role import UserRole
+from cdo_sdk_python.models.user import User
 from typing import Optional, Set
 from typing_extensions import Self
 
-class User(BaseModel):
+class UserPage(BaseModel):
     """
-    User
+    UserPage
     """ # noqa: E501
-    uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the SDC in CDO.")
-    name: Optional[StrictStr] = Field(default=None, description="The name of the user in CDO.")
-    roles: Optional[List[UserRole]] = Field(default=None, description="Roles associated with this user in CDO.")
-    api_only_user: Optional[StrictBool] = Field(default=None, description="Whether the user is API-only, an API-only user cannot access CDO in the UI.", alias="apiOnlyUser")
-    last_successful_login: Optional[datetime] = Field(default=None, description="The time (UTC; represented using the RFC-3339 standard) that indicate the last time the user successfully login CDO.", alias="lastSuccessfulLogin")
-    __properties: ClassVar[List[str]] = ["uid", "name", "roles", "apiOnlyUser", "lastSuccessfulLogin"]
+    count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
+    limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    items: Optional[List[User]] = Field(default=None, description="The list of items retrieved.")
+    __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -50,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of User from a JSON string"""
+        """Create an instance of UserPage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,28 +69,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in items (list)
+        _items = []
+        if self.items:
+            for _item in self.items:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['items'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of User from a dict"""
+        """Create an instance of UserPage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "uid": obj.get("uid"),
-            "name": obj.get("name"),
-            "roles": obj.get("roles"),
-            "apiOnlyUser": obj.get("apiOnlyUser"),
-            "lastSuccessfulLogin": obj.get("lastSuccessfulLogin")
+            "count": obj.get("count"),
+            "limit": obj.get("limit"),
+            "offset": obj.get("offset"),
+            "items": [User.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_create_or_update_input.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/user_create_or_update_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_page.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/mfa_event_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from cdo_sdk_python.models.user import User
+from cdo_sdk_python.models.mfa_event import MfaEvent
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserPage(BaseModel):
+class MfaEventPage(BaseModel):
     """
-    UserPage
+    MfaEventPage
     """ # noqa: E501
     count: Optional[StrictInt] = Field(default=None, description="The total number of results available.")
     limit: Optional[StrictInt] = Field(default=None, description="The number of results retrieved.")
-    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO Public API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
-    items: Optional[List[User]] = Field(default=None, description="The list of items retrieved.")
+    offset: Optional[StrictInt] = Field(default=None, description="The offset of the results retrieved. The CDO API uses the offset field to determine the index of the first result retrieved, and will retrieve `limit` results from the offset specified.")
+    items: Optional[List[MfaEvent]] = Field(default=None, description="The list of items retrieved.")
     __properties: ClassVar[List[str]] = ["count", "limit", "offset", "items"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserPage from a JSON string"""
+        """Create an instance of MfaEventPage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,23 +80,23 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['items'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserPage from a dict"""
+        """Create an instance of MfaEventPage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "limit": obj.get("limit"),
             "offset": obj.get("offset"),
-            "items": [User.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None
+            "items": [MfaEvent.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None
         })
         return _obj
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/models/user_role.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/models/user_role.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python/rest.py` & `cdo-sdk-python-1.0.90/cdo_sdk_python/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Cisco Defense Orchestrator API
+    CDO API
 
-    Use the interactive documentation to explore the endpoints CDO has to offer
+    Use the documentation to explore the endpoints CDO has to offer
 
-    The version of the OpenAPI document: 0.0.1
+    The version of the OpenAPI document: 0.1.0
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `cdo-sdk-python-1.0.9/cdo_sdk_python.egg-info/SOURCES.txt` & `cdo-sdk-python-1.0.90/cdo_sdk_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 setup.cfg
 setup.py
 cdo_sdk_python/__init__.py
 cdo_sdk_python/api_client.py
 cdo_sdk_python/api_response.py
 cdo_sdk_python/configuration.py
 cdo_sdk_python/exceptions.py
-cdo_sdk_python/py.typed
 cdo_sdk_python/rest.py
 cdo_sdk_python.egg-info/PKG-INFO
 cdo_sdk_python.egg-info/SOURCES.txt
 cdo_sdk_python.egg-info/dependency_links.txt
 cdo_sdk_python.egg-info/requires.txt
 cdo_sdk_python.egg-info/top_level.txt
 cdo_sdk_python/api/__init__.py
 cdo_sdk_python/api/change_requests_api.py
 cdo_sdk_python/api/changelogs_api.py
+cdo_sdk_python/api/cloud_delivered_fmc_api.py
 cdo_sdk_python/api/connectors_api.py
 cdo_sdk_python/api/inventory_api.py
 cdo_sdk_python/api/meta_api.py
 cdo_sdk_python/api/object_management_api.py
 cdo_sdk_python/api/remote_access_monitoring_api.py
 cdo_sdk_python/api/search_api.py
 cdo_sdk_python/api/tenant_management_api.py
@@ -28,28 +28,30 @@
 cdo_sdk_python/api/users_api.py
 cdo_sdk_python/models/__init__.py
 cdo_sdk_python/models/api_token_info.py
 cdo_sdk_python/models/asa_create_or_update_input.py
 cdo_sdk_python/models/asa_failover_mate.py
 cdo_sdk_python/models/asa_failover_mode.py
 cdo_sdk_python/models/authentication_error.py
+cdo_sdk_python/models/browser.py
 cdo_sdk_python/models/cd_fmc_info.py
 cdo_sdk_python/models/cd_fmc_object.py
 cdo_sdk_python/models/cd_fmc_result.py
 cdo_sdk_python/models/cdo_region.py
 cdo_sdk_python/models/cdo_region_list.py
 cdo_sdk_python/models/cdo_token_info.py
 cdo_sdk_python/models/cdo_transaction.py
 cdo_sdk_python/models/cdo_transaction_status.py
 cdo_sdk_python/models/cdo_transaction_type.py
 cdo_sdk_python/models/change_request.py
 cdo_sdk_python/models/change_request_create_input.py
 cdo_sdk_python/models/change_request_page.py
 cdo_sdk_python/models/changelog.py
 cdo_sdk_python/models/changelog_page.py
+cdo_sdk_python/models/client_device.py
 cdo_sdk_python/models/common_api_error.py
 cdo_sdk_python/models/config_state.py
 cdo_sdk_python/models/conflict_detection_interval.py
 cdo_sdk_python/models/conflict_detection_state.py
 cdo_sdk_python/models/connectivity_state.py
 cdo_sdk_python/models/connector_type.py
 cdo_sdk_python/models/create_request.py
@@ -73,38 +75,41 @@
 cdo_sdk_python/models/json_web_key.py
 cdo_sdk_python/models/jwk_set.py
 cdo_sdk_python/models/labels.py
 cdo_sdk_python/models/list_object_response.py
 cdo_sdk_python/models/location.py
 cdo_sdk_python/models/meraki_deployment_mode.py
 cdo_sdk_python/models/meta.py
+cdo_sdk_python/models/mfa_event.py
+cdo_sdk_python/models/mfa_event_page.py
 cdo_sdk_python/models/msp_add_tenant_input.py
 cdo_sdk_python/models/network.py
 cdo_sdk_python/models/network_object_content.py
 cdo_sdk_python/models/object_content.py
 cdo_sdk_python/models/object_response.py
 cdo_sdk_python/models/on_prem_fmc_info.py
 cdo_sdk_python/models/os.py
 cdo_sdk_python/models/override.py
 cdo_sdk_python/models/policy.py
 cdo_sdk_python/models/ports_value.py
+cdo_sdk_python/models/public_key.py
 cdo_sdk_python/models/ra_vpn_session.py
 cdo_sdk_python/models/ra_vpn_session_page.py
 cdo_sdk_python/models/reference_info.py
 cdo_sdk_python/models/sdc.py
 cdo_sdk_python/models/sdc_page.py
 cdo_sdk_python/models/sdc_public_key.py
 cdo_sdk_python/models/sdc_status.py
 cdo_sdk_python/models/service_object_content.py
 cdo_sdk_python/models/service_object_value_content.py
 cdo_sdk_python/models/shared_object_value.py
 cdo_sdk_python/models/single_content.py
-cdo_sdk_python/models/sort_criteria_param.py
 cdo_sdk_python/models/state_machine_details.py
 cdo_sdk_python/models/state_machine_error.py
+cdo_sdk_python/models/status.py
 cdo_sdk_python/models/status_info.py
 cdo_sdk_python/models/target.py
 cdo_sdk_python/models/targets_request.py
 cdo_sdk_python/models/tenant.py
 cdo_sdk_python/models/tenant_page.py
 cdo_sdk_python/models/tenant_pay_type.py
 cdo_sdk_python/models/tenant_settings.py
@@ -116,14 +121,15 @@
 cdo_sdk_python/models/user_page.py
 cdo_sdk_python/models/user_role.py
 test/test_api_token_info.py
 test/test_asa_create_or_update_input.py
 test/test_asa_failover_mate.py
 test/test_asa_failover_mode.py
 test/test_authentication_error.py
+test/test_browser.py
 test/test_cd_fmc_info.py
 test/test_cd_fmc_object.py
 test/test_cd_fmc_result.py
 test/test_cdo_region.py
 test/test_cdo_region_list.py
 test/test_cdo_token_info.py
 test/test_cdo_transaction.py
@@ -132,14 +138,16 @@
 test/test_change_request.py
 test/test_change_request_create_input.py
 test/test_change_request_page.py
 test/test_change_requests_api.py
 test/test_changelog.py
 test/test_changelog_page.py
 test/test_changelogs_api.py
+test/test_client_device.py
+test/test_cloud_delivered_fmc_api.py
 test/test_common_api_error.py
 test/test_config_state.py
 test/test_conflict_detection_interval.py
 test/test_conflict_detection_state.py
 test/test_connectivity_state.py
 test/test_connector_type.py
 test/test_connectors_api.py
@@ -166,41 +174,44 @@
 test/test_jwk_set.py
 test/test_labels.py
 test/test_list_object_response.py
 test/test_location.py
 test/test_meraki_deployment_mode.py
 test/test_meta.py
 test/test_meta_api.py
+test/test_mfa_event.py
+test/test_mfa_event_page.py
 test/test_msp_add_tenant_input.py
 test/test_network.py
 test/test_network_object_content.py
 test/test_object_content.py
 test/test_object_management_api.py
 test/test_object_response.py
 test/test_on_prem_fmc_info.py
 test/test_os.py
 test/test_override.py
 test/test_policy.py
 test/test_ports_value.py
+test/test_public_key.py
 test/test_ra_vpn_session.py
 test/test_ra_vpn_session_page.py
 test/test_reference_info.py
 test/test_remote_access_monitoring_api.py
 test/test_sdc.py
 test/test_sdc_page.py
 test/test_sdc_public_key.py
 test/test_sdc_status.py
 test/test_search_api.py
 test/test_service_object_content.py
 test/test_service_object_value_content.py
 test/test_shared_object_value.py
 test/test_single_content.py
-test/test_sort_criteria_param.py
 test/test_state_machine_details.py
 test/test_state_machine_error.py
+test/test_status.py
 test/test_status_info.py
 test/test_target.py
 test/test_targets_request.py
 test/test_tenant.py
 test/test_tenant_management_api.py
 test/test_tenant_page.py
 test/test_tenant_pay_type.py
```

### Comparing `cdo-sdk-python-1.0.9/pyproject.toml` & `cdo-sdk-python-1.0.90/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "cdo_sdk_python"
-version = "1.0.9"
-description = "Cisco Defense Orchestrator API"
+version = "1.0.90"
+description = "CDO API"
 authors = ["CDO TAC <cdo.tac@cisco.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
-keywords = ["OpenAPI", "OpenAPI-Generator", "Cisco Defense Orchestrator API"]
+keywords = ["OpenAPI", "OpenAPI-Generator", "CDO API"]
 include = ["cdo_sdk_python/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 urllib3 = ">= 1.25.3"
 python-dateutil = ">=2.8.2"
```

### Comparing `cdo-sdk-python-1.0.9/test/test_api_token_info.py` & `cdo-sdk-python-1.0.90/test/test_api_token_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_asa_create_or_update_input.py` & `cdo-sdk-python-1.0.90/test/test_asa_create_or_update_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_asa_failover_mate.py` & `cdo-sdk-python-1.0.90/test/test_asa_failover_mate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_asa_failover_mode.py` & `cdo-sdk-python-1.0.90/test/test_asa_failover_mode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_authentication_error.py` & `cdo-sdk-python-1.0.90/test/test_authentication_error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cd_fmc_info.py` & `cdo-sdk-python-1.0.90/test/test_cd_fmc_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cd_fmc_object.py` & `cdo-sdk-python-1.0.90/test/test_cd_fmc_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cd_fmc_result.py` & `cdo-sdk-python-1.0.90/test/test_cd_fmc_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cdo_region.py` & `cdo-sdk-python-1.0.90/test/test_cdo_region.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cdo_region_list.py` & `cdo-sdk-python-1.0.90/test/test_cdo_region_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cdo_token_info.py` & `cdo-sdk-python-1.0.90/test/test_cdo_token_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cdo_transaction.py` & `cdo-sdk-python-1.0.90/test/test_cdo_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cdo_transaction_status.py` & `cdo-sdk-python-1.0.90/test/test_cdo_transaction_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_cdo_transaction_type.py` & `cdo-sdk-python-1.0.90/test/test_cdo_transaction_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_change_request.py` & `cdo-sdk-python-1.0.90/test/test_change_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_change_request_create_input.py` & `cdo-sdk-python-1.0.90/test/test_change_request_create_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_change_request_page.py` & `cdo-sdk-python-1.0.90/test/test_change_request_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_change_requests_api.py` & `cdo-sdk-python-1.0.90/test/test_object_management_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,88 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.api.change_requests_api import ChangeRequestsApi
+from cdo_sdk_python.api.object_management_api import ObjectManagementApi
 
 
-class TestChangeRequestsApi(unittest.TestCase):
-    """ChangeRequestsApi unit test stubs"""
+class TestObjectManagementApi(unittest.TestCase):
+    """ObjectManagementApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = ChangeRequestsApi()
+        self.api = ObjectManagementApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_create_change_request(self) -> None:
-        """Test case for create_change_request
+    def test_create_object(self) -> None:
+        """Test case for create_object
 
-        Create Change Requests.
+        Create Object
         """
         pass
 
-    def test_delete_change_request(self) -> None:
-        """Test case for delete_change_request
+    def test_create_targets(self) -> None:
+        """Test case for create_targets
 
-        Delete a Change Request by UID in the CDO tenant
+        Create Targets
         """
         pass
 
-    def test_get_change_request(self) -> None:
-        """Test case for get_change_request
+    def test_delete_object(self) -> None:
+        """Test case for delete_object
 
-        Fetch a Change Request by UID in the CDO tenant.
+        Delete Object
         """
         pass
 
-    def test_list_change_requests(self) -> None:
-        """Test case for list_change_requests
+    def test_delete_targets(self) -> None:
+        """Test case for delete_targets
 
-        Fetch a list of Change Requests.
+        Delete Targets
+        """
+        pass
+
+    def test_get_object(self) -> None:
+        """Test case for get_object
+
+        Get Object
+        """
+        pass
+
+    def test_get_object_usages(self) -> None:
+        """Test case for get_object_usages
+
+        Get Object Usages
+        """
+        pass
+
+    def test_get_objects(self) -> None:
+        """Test case for get_objects
+
+        Get Objects
+        """
+        pass
+
+    def test_modify_object(self) -> None:
+        """Test case for modify_object
+
+        Modify Object
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_changelog.py` & `cdo-sdk-python-1.0.90/test/test_changelog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_changelog_page.py` & `cdo-sdk-python-1.0.90/test/test_changelog_page.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_changelogs_api.py` & `cdo-sdk-python-1.0.90/test/test_changelogs_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
@@ -26,21 +26,21 @@
 
     def tearDown(self) -> None:
         pass
 
     def test_get_changelog(self) -> None:
         """Test case for get_changelog
 
-        Fetch a Change Log by UID in the CDO tenant.
+        Get Change Log
         """
         pass
 
-    def test_list_changelogs(self) -> None:
-        """Test case for list_changelogs
+    def test_get_changelogs(self) -> None:
+        """Test case for get_changelogs
 
-        Fetch a list of Change Logs.
+        List Change Logs
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_common_api_error.py` & `cdo-sdk-python-1.0.90/test/test_common_api_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
@@ -34,17 +34,15 @@
         # uncomment below to create an instance of `CommonApiError`
         """
         model = CommonApiError()
         if include_optional:
             return CommonApiError(
                 error_code = 'INVALID_INPUT',
                 error_msg = 'sample error',
-                details = {
-                    'key' : None
-                    }
+                details = {}
             )
         else:
             return CommonApiError(
         )
         """
 
     def testCommonApiError(self):
```

### Comparing `cdo-sdk-python-1.0.9/test/test_config_state.py` & `cdo-sdk-python-1.0.90/test/test_config_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_conflict_detection_interval.py` & `cdo-sdk-python-1.0.90/test/test_conflict_detection_interval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_conflict_detection_state.py` & `cdo-sdk-python-1.0.90/test/test_conflict_detection_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_connectivity_state.py` & `cdo-sdk-python-1.0.90/test/test_connectivity_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_connector_type.py` & `cdo-sdk-python-1.0.90/test/test_connector_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_create_request.py` & `cdo-sdk-python-1.0.90/test/test_create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_device.py` & `cdo-sdk-python-1.0.90/test/test_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_device_page.py` & `cdo-sdk-python-1.0.90/test/test_device_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_device_patch_input.py` & `cdo-sdk-python-1.0.90/test/test_device_patch_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_device_role.py` & `cdo-sdk-python-1.0.90/test/test_device_role.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_duo_admin_panel_create_or_update_input.py` & `cdo-sdk-python-1.0.90/test/test_duo_admin_panel_create_or_update_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_entity.py` & `cdo-sdk-python-1.0.90/test/test_entity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_entity_type.py` & `cdo-sdk-python-1.0.90/test/test_tenant_pay_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.entity_type import EntityType
+from cdo_sdk_python.models.tenant_pay_type import TenantPayType
 
-class TestEntityType(unittest.TestCase):
-    """EntityType unit test stubs"""
+class TestTenantPayType(unittest.TestCase):
+    """TenantPayType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEntityType(self):
-        """Test EntityType"""
-        # inst = EntityType()
+    def testTenantPayType(self):
+        """Test TenantPayType"""
+        # inst = TenantPayType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_event.py` & `cdo-sdk-python-1.0.90/test/test_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_ftd_create_or_update_input.py` & `cdo-sdk-python-1.0.90/test/test_ftd_create_or_update_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_ftd_registration_input.py` & `cdo-sdk-python-1.0.90/test/test_override.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.ftd_registration_input import FtdRegistrationInput
+from cdo_sdk_python.models.override import Override
 
-class TestFtdRegistrationInput(unittest.TestCase):
-    """FtdRegistrationInput unit test stubs"""
+class TestOverride(unittest.TestCase):
+    """Override unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> FtdRegistrationInput:
-        """Test FtdRegistrationInput
+    def make_instance(self, include_optional) -> Override:
+        """Test Override
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `FtdRegistrationInput`
+        # uncomment below to create an instance of `Override`
         """
-        model = FtdRegistrationInput()
+        model = Override()
         if include_optional:
-            return FtdRegistrationInput(
-                ftd_uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb'
+            return Override(
+                target_id = 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx',
+                content = {"literal":"a:b:c::1"}
             )
         else:
-            return FtdRegistrationInput(
-                ftd_uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb',
+            return Override(
+                content = {"literal":"a:b:c::1"},
         )
         """
 
-    def testFtdRegistrationInput(self):
-        """Test FtdRegistrationInput"""
+    def testOverride(self):
+        """Test Override"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_global_search_result.py` & `cdo-sdk-python-1.0.90/test/test_global_search_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_group_content.py` & `cdo-sdk-python-1.0.90/test/test_group_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_icmp4_value.py` & `cdo-sdk-python-1.0.90/test/test_icmp6_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.icmp4_value import Icmp4Value
+from cdo_sdk_python.models.icmp6_value import Icmp6Value
 
-class TestIcmp4Value(unittest.TestCase):
-    """Icmp4Value unit test stubs"""
+class TestIcmp6Value(unittest.TestCase):
+    """Icmp6Value unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Icmp4Value:
-        """Test Icmp4Value
+    def make_instance(self, include_optional) -> Icmp6Value:
+        """Test Icmp6Value
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Icmp4Value`
+        # uncomment below to create an instance of `Icmp6Value`
         """
-        model = Icmp4Value()
+        model = Icmp6Value()
         if include_optional:
-            return Icmp4Value(
-                icmp4_type = 'DESTINATION_UNREACHABLE',
-                icmp4_code = 'NET_UNREACHABLE'
+            return Icmp6Value(
+                icmp6_type = 'DESTINATION_UNREACHABLE',
+                icmp6_code = 'ADDRESS_UNREACHABLE'
             )
         else:
-            return Icmp4Value(
+            return Icmp6Value(
         )
         """
 
-    def testIcmp4Value(self):
-        """Test Icmp4Value"""
+    def testIcmp6Value(self):
+        """Test Icmp6Value"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_icmp6_value.py` & `cdo-sdk-python-1.0.90/test/test_labels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.icmp6_value import Icmp6Value
+from cdo_sdk_python.models.labels import Labels
 
-class TestIcmp6Value(unittest.TestCase):
-    """Icmp6Value unit test stubs"""
+class TestLabels(unittest.TestCase):
+    """Labels unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Icmp6Value:
-        """Test Icmp6Value
+    def make_instance(self, include_optional) -> Labels:
+        """Test Labels
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Icmp6Value`
+        # uncomment below to create an instance of `Labels`
         """
-        model = Icmp6Value()
+        model = Labels()
         if include_optional:
-            return Icmp6Value(
-                icmp6_type = 'DESTINATION_UNREACHABLE',
-                icmp6_code = 'ADDRESS_UNREACHABLE'
+            return Labels(
+                grouped_labels = {"group1":["label-1","label-2"],"group2":["label-1","label-2"]},
+                ungrouped_labels = ["label-a","label-b","label-c"]
             )
         else:
-            return Icmp6Value(
+            return Labels(
         )
         """
 
-    def testIcmp6Value(self):
-        """Test Icmp6Value"""
+    def testLabels(self):
+        """Test Labels"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_inventory.py` & `cdo-sdk-python-1.0.90/test/test_inventory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_ios_create_or_update_input.py` & `cdo-sdk-python-1.0.90/test/test_ios_create_or_update_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_issues_dto.py` & `cdo-sdk-python-1.0.90/test/test_issues_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_json_web_key.py` & `cdo-sdk-python-1.0.90/test/test_json_web_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_jwk_set.py` & `cdo-sdk-python-1.0.90/test/test_jwk_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_labels.py` & `cdo-sdk-python-1.0.90/test/test_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.labels import Labels
+from cdo_sdk_python.models.user import User
 
-class TestLabels(unittest.TestCase):
-    """Labels unit test stubs"""
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Labels:
-        """Test Labels
+    def make_instance(self, include_optional) -> User:
+        """Test User
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Labels`
+        # uncomment below to create an instance of `User`
         """
-        model = Labels()
+        model = User()
         if include_optional:
-            return Labels(
-                grouped_labels = {"group1":["label-1","label-2"],"group2":["label-1","label-2"]},
-                ungrouped_labels = ["label-a","label-b","label-c"]
+            return User(
+                uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb',
+                name = 'myusername@cisco.com',
+                roles = [ROLE_ADMIN],
+                api_only_user = False,
+                last_successful_login = '2023-12-13T05:15:44Z'
             )
         else:
-            return Labels(
+            return User(
         )
         """
 
-    def testLabels(self):
-        """Test Labels"""
+    def testUser(self):
+        """Test User"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_list_object_response.py` & `cdo-sdk-python-1.0.90/test/test_list_object_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_location.py` & `cdo-sdk-python-1.0.90/test/test_location.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_meraki_deployment_mode.py` & `cdo-sdk-python-1.0.90/test/test_meraki_deployment_mode.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_meta.py` & `cdo-sdk-python-1.0.90/test/test_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_meta_api.py` & `cdo-sdk-python-1.0.90/test/test_meta_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
@@ -26,27 +26,27 @@
 
     def tearDown(self) -> None:
         pass
 
     def test_get_jwks(self) -> None:
         """Test case for get_jwks
 
-        Fetch The JSON Web Key Set
+        Fetch JSON Web Key Set
         """
         pass
 
     def test_get_meta(self) -> None:
         """Test case for get_meta
 
-        Get Meta information about CDO, including the IP addresses of CDO services
+        Get Meta information
         """
         pass
 
-    def test_list_regions(self) -> None:
-        """Test case for list_regions
+    def test_get_regions(self) -> None:
+        """Test case for get_regions
 
         Fetch a list of CDO regions.
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `cdo-sdk-python-1.0.9/test/test_msp_add_tenant_input.py` & `cdo-sdk-python-1.0.90/test/test_msp_add_tenant_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_network.py` & `cdo-sdk-python-1.0.90/test/test_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_network_object_content.py` & `cdo-sdk-python-1.0.90/test/test_network_object_content.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_object_content.py` & `cdo-sdk-python-1.0.90/test/test_object_content.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_object_management_api.py` & `cdo-sdk-python-1.0.90/test/test_users_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,88 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.api.object_management_api import ObjectManagementApi
+from cdo_sdk_python.api.users_api import UsersApi
 
 
-class TestObjectManagementApi(unittest.TestCase):
-    """ObjectManagementApi unit test stubs"""
+class TestUsersApi(unittest.TestCase):
+    """UsersApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = ObjectManagementApi()
+        self.api = UsersApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_create_object(self) -> None:
-        """Test case for create_object
+    def test_create_user(self) -> None:
+        """Test case for create_user
 
-        Creates an object in the CDO tenant
+        Create User in CDO Tenant
         """
         pass
 
-    def test_create_targets(self) -> None:
-        """Test case for create_targets
+    def test_delete_user(self) -> None:
+        """Test case for delete_user
 
-        Create targets for an object in the CDO tenant
+        Remove User from CDO Tenant
         """
         pass
 
-    def test_delete_object(self) -> None:
-        """Test case for delete_object
+    def test_generate_api_token(self) -> None:
+        """Test case for generate_api_token
 
-        Deletes an object in the CDO tenant
+        Generate Token for API-only user
         """
         pass
 
-    def test_get_object(self) -> None:
-        """Test case for get_object
+    def test_get_token(self) -> None:
+        """Test case for get_token
 
-        Retrieves an object in the CDO tenant
+        Get Token Info
         """
         pass
 
-    def test_get_object_usage(self) -> None:
-        """Test case for get_object_usage
+    def test_get_user(self) -> None:
+        """Test case for get_user
 
-        Retrieves usages of an object in the CDO tenant
+        Get Tenant User
         """
         pass
 
-    def test_list_objects(self) -> None:
-        """Test case for list_objects
+    def test_get_users(self) -> None:
+        """Test case for get_users
 
-        Retrieves objects in the CDO tenant
+        Get Tenant Users
         """
         pass
 
-    def test_remove_targets(self) -> None:
-        """Test case for remove_targets
+    def test_revoke_api_token(self) -> None:
+        """Test case for revoke_api_token
 
-        Removes targets from an object in the CDO tenant
+        Revoke API-only User's Token
         """
         pass
 
-    def test_update_object(self) -> None:
-        """Test case for update_object
+    def test_revoke_token(self) -> None:
+        """Test case for revoke_token
 
-        Updates an object in the CDO tenant
+        Revoke Token
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_object_response.py` & `cdo-sdk-python-1.0.90/test/test_object_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_on_prem_fmc_info.py` & `cdo-sdk-python-1.0.90/test/test_on_prem_fmc_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_os.py` & `cdo-sdk-python-1.0.90/test/test_os.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_override.py` & `cdo-sdk-python-1.0.90/test/test_status_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.override import Override
+from cdo_sdk_python.models.status_info import StatusInfo
 
-class TestOverride(unittest.TestCase):
-    """Override unit test stubs"""
+class TestStatusInfo(unittest.TestCase):
+    """StatusInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Override:
-        """Test Override
+    def make_instance(self, include_optional) -> StatusInfo:
+        """Test StatusInfo
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Override`
+        # uncomment below to create an instance of `StatusInfo`
         """
-        model = Override()
+        model = StatusInfo()
         if include_optional:
-            return Override(
-                target_id = 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx',
-                content = {"literal":"a:b:c::1"}
+            return StatusInfo(
+                status = 'OK'
             )
         else:
-            return Override(
-                content = {"literal":"a:b:c::1"},
+            return StatusInfo(
         )
         """
 
-    def testOverride(self):
-        """Test Override"""
+    def testStatusInfo(self):
+        """Test StatusInfo"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_policy.py` & `cdo-sdk-python-1.0.90/test/test_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_ports_value.py` & `cdo-sdk-python-1.0.90/test/test_ports_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_ra_vpn_session.py` & `cdo-sdk-python-1.0.90/test/test_ra_vpn_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_ra_vpn_session_page.py` & `cdo-sdk-python-1.0.90/test/test_ra_vpn_session_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_reference_info.py` & `cdo-sdk-python-1.0.90/test/test_reference_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_remote_access_monitoring_api.py` & `cdo-sdk-python-1.0.90/test/test_remote_access_monitoring_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
@@ -26,21 +26,35 @@
 
     def tearDown(self) -> None:
         pass
 
     def test_get_ra_vpn_session(self) -> None:
         """Test case for get_ra_vpn_session
 
-        Fetch a RA VPN session by UID in the CDO tenant.
+        Get RA VPN Session
         """
         pass
 
-    def test_list_ra_vpn_sessions(self) -> None:
-        """Test case for list_ra_vpn_sessions
+    def test_get_ra_vpn_sessions(self) -> None:
+        """Test case for get_ra_vpn_sessions
 
-        Fetch a list of RA VPN sessions.
+        Get RA VPN Sessions
+        """
+        pass
+
+    def test_terminate_ra_vpn_sessions_by_device(self) -> None:
+        """Test case for terminate_ra_vpn_sessions_by_device
+
+        Terminate RA VPN Sessions.
+        """
+        pass
+
+    def test_terminate_ra_vpn_sessions_by_device_and_user_name(self) -> None:
+        """Test case for terminate_ra_vpn_sessions_by_device_and_user_name
+
+        Terminate User's RA VPN Sessions
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_sdc.py` & `cdo-sdk-python-1.0.90/test/test_sdc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_sdc_page.py` & `cdo-sdk-python-1.0.90/test/test_sdc_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_sdc_public_key.py` & `cdo-sdk-python-1.0.90/test/test_sdc_public_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_sdc_status.py` & `cdo-sdk-python-1.0.90/test/test_sdc_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_service_object_content.py` & `cdo-sdk-python-1.0.90/test/test_service_object_content.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_service_object_value_content.py` & `cdo-sdk-python-1.0.90/test/test_service_object_value_content.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_shared_object_value.py` & `cdo-sdk-python-1.0.90/test/test_shared_object_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_single_content.py` & `cdo-sdk-python-1.0.90/test/test_single_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_state_machine_details.py` & `cdo-sdk-python-1.0.90/test/test_state_machine_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_state_machine_error.py` & `cdo-sdk-python-1.0.90/test/test_state_machine_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_status_info.py` & `cdo-sdk-python-1.0.90/test/test_tenant.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.status_info import StatusInfo
+from cdo_sdk_python.models.tenant import Tenant
 
-class TestStatusInfo(unittest.TestCase):
-    """StatusInfo unit test stubs"""
+class TestTenant(unittest.TestCase):
+    """Tenant unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> StatusInfo:
-        """Test StatusInfo
+    def make_instance(self, include_optional) -> Tenant:
+        """Test Tenant
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `StatusInfo`
+        # uncomment below to create an instance of `Tenant`
         """
-        model = StatusInfo()
+        model = Tenant()
         if include_optional:
-            return StatusInfo(
-                status = 'OK'
+            return Tenant(
+                uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb',
+                name = 'mytenantname@cisco.com',
+                security_cloud_control_enterprise_id = 'dda3ce52-312c-477a-aa86-1fd1866ddab7',
+                display_name = 'mytenantname',
+                pay_type = 'TRIAL'
             )
         else:
-            return StatusInfo(
+            return Tenant(
         )
         """
 
-    def testStatusInfo(self):
-        """Test StatusInfo"""
+    def testTenant(self):
+        """Test Tenant"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_target.py` & `cdo-sdk-python-1.0.90/test/test_target.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_targets_request.py` & `cdo-sdk-python-1.0.90/test/test_targets_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_tenant.py` & `cdo-sdk-python-1.0.90/test/test_tenant_page.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.tenant import Tenant
+from cdo_sdk_python.models.tenant_page import TenantPage
 
-class TestTenant(unittest.TestCase):
-    """Tenant unit test stubs"""
+class TestTenantPage(unittest.TestCase):
+    """TenantPage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Tenant:
-        """Test Tenant
+    def make_instance(self, include_optional) -> TenantPage:
+        """Test TenantPage
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Tenant`
+        # uncomment below to create an instance of `TenantPage`
         """
-        model = Tenant()
+        model = TenantPage()
         if include_optional:
-            return Tenant(
-                uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb',
-                name = 'mytenantname@cisco.com',
-                security_cloud_control_enterprise_id = 'dda3ce52-312c-477a-aa86-1fd1866ddab7',
-                display_name = 'mytenantname',
-                pay_type = 'TRIAL'
+            return TenantPage(
+                count = 100,
+                limit = 50,
+                offset = 0,
+                items = [
+                    cdo_sdk_python.models.tenant.Tenant(
+                        uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb', 
+                        name = 'mytenantname@cisco.com', 
+                        security_cloud_control_enterprise_id = 'dda3ce52-312c-477a-aa86-1fd1866ddab7', 
+                        display_name = 'mytenantname', 
+                        pay_type = 'TRIAL', )
+                    ]
             )
         else:
-            return Tenant(
+            return TenantPage(
         )
         """
 
-    def testTenant(self):
-        """Test Tenant"""
+    def testTenantPage(self):
+        """Test TenantPage"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_tenant_management_api.py` & `cdo-sdk-python-1.0.90/test/test_tenant_management_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
@@ -26,49 +26,49 @@
 
     def tearDown(self) -> None:
         pass
 
     def test_add_msp_tenant(self) -> None:
         """Test case for add_msp_tenant
 
-        Add a tenant to the MSP Portal
+        Add Tenant to MSP Portal
         """
         pass
 
-    def test_get_tenant(self) -> None:
-        """Test case for get_tenant
+    def test_get_feature_flags(self) -> None:
+        """Test case for get_feature_flags
 
-        Fetch a tenant by UID in CDO
+        Get Feature Flags
         """
         pass
 
-    def test_get_tenant_settings(self) -> None:
-        """Test case for get_tenant_settings
+    def test_get_tenant(self) -> None:
+        """Test case for get_tenant
 
-        Fetch the tenant settings in CDO
+        Get Tenant
         """
         pass
 
-    def test_list_feature_flags(self) -> None:
-        """Test case for list_feature_flags
+    def test_get_tenant_settings(self) -> None:
+        """Test case for get_tenant_settings
 
-        Fetch the feature flags enabled for this tenant
+        Get Tenant Settings
         """
         pass
 
-    def test_list_tenants(self) -> None:
-        """Test case for list_tenants
+    def test_get_tenants(self) -> None:
+        """Test case for get_tenants
 
-        Fetch a list of tenants associated with the CDO user.
+        Get Tenants
         """
         pass
 
-    def test_update_tenant_settings(self) -> None:
-        """Test case for update_tenant_settings
+    def test_modify_tenant_settings(self) -> None:
+        """Test case for modify_tenant_settings
 
-        Update the tenant settings in CDO
+        Modify Tenant Settings
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_tenant_page.py` & `cdo-sdk-python-1.0.90/test/test_update_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.tenant_page import TenantPage
+from cdo_sdk_python.models.update_request import UpdateRequest
 
-class TestTenantPage(unittest.TestCase):
-    """TenantPage unit test stubs"""
+class TestUpdateRequest(unittest.TestCase):
+    """UpdateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> TenantPage:
-        """Test TenantPage
+    def make_instance(self, include_optional) -> UpdateRequest:
+        """Test UpdateRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `TenantPage`
+        # uncomment below to create an instance of `UpdateRequest`
         """
-        model = TenantPage()
+        model = UpdateRequest()
         if include_optional:
-            return TenantPage(
-                count = 100,
-                limit = 50,
-                offset = 0,
-                items = [
-                    cdo_sdk_python.models.tenant.Tenant(
-                        uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb', 
-                        name = 'mytenantname@cisco.com', 
-                        security_cloud_control_enterprise_id = 'dda3ce52-312c-477a-aa86-1fd1866ddab7', 
-                        display_name = 'mytenantname', 
-                        pay_type = 'TRIAL', )
-                    ]
+            return UpdateRequest(
+                name = 'my-object',
+                description = 'My object description',
+                value = cdo_sdk_python.models.shared_object_value.SharedObjectValue(
+                    object_type = 'NETWORK_OBJECT', 
+                    default_content = {"literal":"a:b:c::1"}, 
+                    overrides = [
+                        {"targetId":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx","content":"a:b:c::2"}
+                        ], ),
+                tags = {"location":["London","Head-office"]},
+                labels = ["migration"]
             )
         else:
-            return TenantPage(
+            return UpdateRequest(
         )
         """
 
-    def testTenantPage(self):
-        """Test TenantPage"""
+    def testUpdateRequest(self):
+        """Test UpdateRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_tenant_settings.py` & `cdo-sdk-python-1.0.90/test/test_tenant_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_transactions_api.py` & `cdo-sdk-python-1.0.90/test/test_transactions_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
@@ -26,14 +26,14 @@
 
     def tearDown(self) -> None:
         pass
 
     def test_get_transaction(self) -> None:
         """Test case for get_transaction
 
-        Get information of an in-progress CDO transaction
+        Get Transaction
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_unified_object_list_view.py` & `cdo-sdk-python-1.0.90/test/test_unified_object_list_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_update_request.py` & `cdo-sdk-python-1.0.90/test/test_user_create_or_update_input.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,55 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.update_request import UpdateRequest
+from cdo_sdk_python.models.user_create_or_update_input import UserCreateOrUpdateInput
 
-class TestUpdateRequest(unittest.TestCase):
-    """UpdateRequest unit test stubs"""
+class TestUserCreateOrUpdateInput(unittest.TestCase):
+    """UserCreateOrUpdateInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> UpdateRequest:
-        """Test UpdateRequest
+    def make_instance(self, include_optional) -> UserCreateOrUpdateInput:
+        """Test UserCreateOrUpdateInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UpdateRequest`
+        # uncomment below to create an instance of `UserCreateOrUpdateInput`
         """
-        model = UpdateRequest()
+        model = UserCreateOrUpdateInput()
         if include_optional:
-            return UpdateRequest(
-                name = 'my-object',
-                description = 'My object description',
-                value = cdo_sdk_python.models.shared_object_value.SharedObjectValue(
-                    object_type = 'NETWORK_OBJECT', 
-                    default_content = {"literal":"a:b:c::1"}, 
-                    overrides = [
-                        {"targetId":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx","content":"a:b:c::2"}
-                        ], ),
-                tags = {"location":["London","Head-office"]},
-                labels = ["migration"]
+            return UserCreateOrUpdateInput(
+                name = 'myusername@cisco.com',
+                role = 'ROLE_ADMIN',
+                api_only_user = False
             )
         else:
-            return UpdateRequest(
+            return UserCreateOrUpdateInput(
+                name = 'myusername@cisco.com',
         )
         """
 
-    def testUpdateRequest(self):
-        """Test UpdateRequest"""
+    def testUserCreateOrUpdateInput(self):
+        """Test UserCreateOrUpdateInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_url_object_content.py` & `cdo-sdk-python-1.0.90/test/test_url_object_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

### Comparing `cdo-sdk-python-1.0.9/test/test_user.py` & `cdo-sdk-python-1.0.90/test/test_user_page.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.user import User
+from cdo_sdk_python.models.user_page import UserPage
 
-class TestUser(unittest.TestCase):
-    """User unit test stubs"""
+class TestUserPage(unittest.TestCase):
+    """UserPage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> User:
-        """Test User
+    def make_instance(self, include_optional) -> UserPage:
+        """Test UserPage
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `User`
+        # uncomment below to create an instance of `UserPage`
         """
-        model = User()
+        model = UserPage()
         if include_optional:
-            return User(
-                uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb',
-                name = 'myusername@cisco.com',
-                roles = [ROLE_ADMIN],
-                api_only_user = False,
-                last_successful_login = '2023-12-13T05:15:44Z'
+            return UserPage(
+                count = 100,
+                limit = 50,
+                offset = 0,
+                items = [
+                    cdo_sdk_python.models.user.User(
+                        uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb', 
+                        name = 'myusername@cisco.com', 
+                        roles = [ROLE_ADMIN], 
+                        api_only_user = False, 
+                        last_successful_login = '2023-12-13T05:15:44Z', )
+                    ]
             )
         else:
-            return User(
+            return UserPage(
         )
         """
 
-    def testUser(self):
-        """Test User"""
+    def testUserPage(self):
+        """Test UserPage"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_user_create_or_update_input.py` & `cdo-sdk-python-1.0.90/test/test_icmp4_value.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.user_create_or_update_input import UserCreateOrUpdateInput
+from cdo_sdk_python.models.icmp4_value import Icmp4Value
 
-class TestUserCreateOrUpdateInput(unittest.TestCase):
-    """UserCreateOrUpdateInput unit test stubs"""
+class TestIcmp4Value(unittest.TestCase):
+    """Icmp4Value unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> UserCreateOrUpdateInput:
-        """Test UserCreateOrUpdateInput
+    def make_instance(self, include_optional) -> Icmp4Value:
+        """Test Icmp4Value
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UserCreateOrUpdateInput`
+        # uncomment below to create an instance of `Icmp4Value`
         """
-        model = UserCreateOrUpdateInput()
+        model = Icmp4Value()
         if include_optional:
-            return UserCreateOrUpdateInput(
-                name = 'myusername@cisco.com',
-                role = 'ROLE_ADMIN',
-                api_only_user = False
+            return Icmp4Value(
+                icmp4_type = 'DESTINATION_UNREACHABLE',
+                icmp4_code = 'NET_UNREACHABLE'
             )
         else:
-            return UserCreateOrUpdateInput(
-                name = 'myusername@cisco.com',
+            return Icmp4Value(
         )
         """
 
-    def testUserCreateOrUpdateInput(self):
-        """Test UserCreateOrUpdateInput"""
+    def testIcmp4Value(self):
+        """Test Icmp4Value"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_user_page.py` & `cdo-sdk-python-1.0.90/test/test_client_device.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from cdo_sdk_python.models.user_page import UserPage
+from cdo_sdk_python.models.client_device import ClientDevice
 
-class TestUserPage(unittest.TestCase):
-    """UserPage unit test stubs"""
+class TestClientDevice(unittest.TestCase):
+    """ClientDevice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> UserPage:
-        """Test UserPage
+    def make_instance(self, include_optional) -> ClientDevice:
+        """Test ClientDevice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UserPage`
+        # uncomment below to create an instance of `ClientDevice`
         """
-        model = UserPage()
+        model = ClientDevice()
         if include_optional:
-            return UserPage(
-                count = 100,
-                limit = 50,
-                offset = 0,
-                items = [
-                    cdo_sdk_python.models.user.User(
-                        uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb', 
-                        name = 'myusername@cisco.com', 
-                        roles = [ROLE_ADMIN], 
-                        api_only_user = False, 
-                        last_successful_login = '2023-12-13T05:15:44Z', )
-                    ]
+            return ClientDevice(
+                uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb',
+                location = cdo_sdk_python.models.location.Location(
+                    city = 'San Jose', 
+                    subdivision = 'California', 
+                    country = 'United States', ),
+                ip_address = '106.51.163.157',
+                password_set = False,
+                encrypted = True,
+                firewalled = True,
+                os = cdo_sdk_python.models.os.OS(
+                    type = 'mac-intel', 
+                    version = '14.2.1', ),
+                browser = cdo_sdk_python.models.browser.Browser(
+                    name = 'Chrome', 
+                    version = '121.0.6167.160', )
             )
         else:
-            return UserPage(
+            return ClientDevice(
+                uid = '7131daad-e813-4b8f-8f42-be1e241e8cdb',
         )
         """
 
-    def testUserPage(self):
-        """Test UserPage"""
+    def testClientDevice(self):
+        """Test ClientDevice"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cdo-sdk-python-1.0.9/test/test_user_role.py` & `cdo-sdk-python-1.0.90/test/test_user_role.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    API Docs
+    Cisco Defense Orchestrator API
 
     Use the interactive documentation to explore the endpoints CDO has to offer
 
     The version of the OpenAPI document: 0.0.1
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
```

