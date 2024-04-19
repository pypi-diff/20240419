# Comparing `tmp/iparapheur-internal-1.11.2.tar.gz` & `tmp/iparapheur-internal-1.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-internal-1.11.2.tar", last modified: Thu Mar 28 15:45:33 2024, max compression
+gzip compressed data, was "iparapheur-internal-1.12.3.tar", last modified: Fri Apr 19 14:46:45 2024, max compression
```

## Comparing `iparapheur-internal-1.11.2.tar` & `iparapheur-internal-1.12.3.tar`

### file list

```diff
@@ -1,193 +1,197 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:45:33.374596 iparapheur-internal-1.11.2/
--rw-r--r--   0 root         (0) root         (0)      532 2024-03-28 15:45:33.374596 iparapheur-internal-1.11.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12154 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:45:33.318596 iparapheur-internal-1.11.2/iparapheur_internal/
--rw-r--r--   0 root         (0) root         (0)     7338 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:45:33.322596 iparapheur-internal-1.11.2/iparapheur_internal/api/
--rw-r--r--   0 root         (0) root         (0)      994 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32735 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/admin_advanced_config_api.py
--rw-r--r--   0 root         (0) root         (0)    18231 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)    93433 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/admin_layer_api.py
--rw-r--r--   0 root         (0) root         (0)    26447 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/admin_seal_certificate_api.py
--rw-r--r--   0 root         (0) root         (0)    35616 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/admin_template_api.py
--rw-r--r--   0 root         (0) root         (0)    14505 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/admin_trash_bin_api.py
--rw-r--r--   0 root         (0) root         (0)    18687 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    11818 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/current_user_api.py
--rw-r--r--   0 root         (0) root         (0)    15950 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/desk_api.py
--rw-r--r--   0 root         (0) root         (0)    27573 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/folder_api.py
--rw-r--r--   0 root         (0) root         (0)    20001 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/server_info_api.py
--rw-r--r--   0 root         (0) root         (0)    13684 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/template_api.py
--rw-r--r--   0 root         (0) root         (0)    22740 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/typology_api.py
--rw-r--r--   0 root         (0) root         (0)    12942 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api/workflow_api.py
--rw-r--r--   0 root         (0) root         (0)    25875 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/api_response.py
--rw-r--r--   0 root         (0) root         (0)    14816 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6025 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:45:33.354596 iparapheur-internal-1.11.2/iparapheur_internal/models/
--rw-r--r--   0 root         (0) root         (0)     5802 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1340 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/action.py
--rw-r--r--   0 root         (0) root         (0)     2960 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/create_file_stamp_request.py
--rw-r--r--   0 root         (0) root         (0)     3294 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     3562 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/detached_signature.py
--rw-r--r--   0 root         (0) root         (0)     8680 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/document_dto.py
--rw-r--r--   0 root         (0) root         (0)     2918 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/error_response.py
--rw-r--r--   0 root         (0) root         (0)     3295 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      909 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/external_state.py
--rw-r--r--   0 root         (0) root         (0)     8322 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     4854 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/folder_filter_dto.py
--rw-r--r--   0 root         (0) root         (0)     6481 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)     1174 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     6040 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_application.py
--rw-r--r--   0 root         (0) root         (0)     2737 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_cookie.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_data_element.py
--rw-r--r--   0 root         (0) root         (0)     2895 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_data_set.py
--rw-r--r--   0 root         (0) root         (0)     4361 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_declaring_entity.py
--rw-r--r--   0 root         (0) root         (0)     2799 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_declaring_entity_dpo.py
--rw-r--r--   0 root         (0) root         (0)     2835 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_declaring_entity_responsible.py
--rw-r--r--   0 root         (0) root         (0)     2904 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_entity.py
--rw-r--r--   0 root         (0) root         (0)     4705 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_information_details_dto.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     3642 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     3091 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     2654 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/mail_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     3623 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/media_type.py
--rw-r--r--   0 root         (0) root         (0)     4064 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4853 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     4918 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)     5022 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     2767 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_info.py
--rw-r--r--   0 root         (0) root         (0)     4933 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     4949 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     4957 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/page_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3804 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/password_policies.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     2755 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/pdf_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     3633 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     3059 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/signature_info.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/signature_placement.py
--rw-r--r--   0 root         (0) root         (0)      833 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3095 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/sort_object.py
--rw-r--r--   0 root         (0) root         (0)     3652 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/stamp_dto.py
--rw-r--r--   0 root         (0) root         (0)      800 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/stamp_text_color.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/stamp_type.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/state.py
--rw-r--r--   0 root         (0) root         (0)     6951 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/step_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/step_definition_parallel_type.py
--rw-r--r--   0 root         (0) root         (0)      960 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/step_definition_type.py
--rw-r--r--   0 root         (0) root         (0)    13624 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     3619 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3099 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     7888 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/task.py
--rw-r--r--   0 root         (0) root         (0)     1302 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/template_type.py
--rw-r--r--   0 root         (0) root         (0)     3095 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     2722 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/test_signature_template_request.py
--rw-r--r--   0 root         (0) root         (0)     5238 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     3558 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/typology_representation.py
--rw-r--r--   0 root         (0) root         (0)    12060 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/user_dto.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     2766 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/validation_service_configuration_dto.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/iparapheur_internal/models/workflow_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/py.typed
--rw-r--r--   0 root         (0) root         (0)     9290 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/iparapheur_internal/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:45:33.374596 iparapheur-internal-1.11.2/iparapheur_internal.egg-info/
--rw-r--r--   0 root         (0) root         (0)      532 2024-03-28 15:45:33.000000 iparapheur-internal-1.11.2/iparapheur_internal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7364 2024-03-28 15:45:33.000000 iparapheur-internal-1.11.2/iparapheur_internal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 15:45:33.000000 iparapheur-internal-1.11.2/iparapheur_internal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-03-28 15:45:33.000000 iparapheur-internal-1.11.2/iparapheur_internal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-28 15:45:33.000000 iparapheur-internal-1.11.2/iparapheur_internal.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1952 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       69 2024-03-28 15:45:33.374596 iparapheur-internal-1.11.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1420 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:45:33.374596 iparapheur-internal-1.11.2/test/
--rw-r--r--   0 root         (0) root         (0)      712 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_action.py
--rw-r--r--   0 root         (0) root         (0)     1273 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_admin_advanced_config_api.py
--rw-r--r--   0 root         (0) root         (0)      838 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_admin_layer_api.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_admin_seal_certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1229 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_admin_template_api.py
--rw-r--r--   0 root         (0) root         (0)      898 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_admin_trash_bin_api.py
--rw-r--r--   0 root         (0) root         (0)      889 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)     2454 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_create_file_stamp_request.py
--rw-r--r--   0 root         (0) root         (0)      872 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_current_user_api.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     2106 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_detached_signature.py
--rw-r--r--   0 root         (0) root         (0)     5048 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_document_dto.py
--rw-r--r--   0 root         (0) root         (0)     1544 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      847 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      762 2024-03-28 15:45:02.000000 iparapheur-internal-1.11.2/test/test_external_state.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_folder_api.py
--rw-r--r--   0 root         (0) root         (0)    13245 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     2504 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_folder_filter_dto.py
--rw-r--r--   0 root         (0) root         (0)     6949 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2952 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_application.py
--rw-r--r--   0 root         (0) root         (0)     1498 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_cookie.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_data_element.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_data_set.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_declaring_entity.py
--rw-r--r--   0 root         (0) root         (0)     1562 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_declaring_entity_dpo.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_declaring_entity_responsible.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_entity.py
--rw-r--r--   0 root         (0) root         (0)     4344 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_gdpr_information_details_dto.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     1597 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_mail_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_media_type.py
--rw-r--r--   0 root         (0) root         (0)     1712 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      755 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)    14443 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     8167 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     1432 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     3010 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3111 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_page_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     1901 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     1752 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_password_policies.py
--rw-r--r--   0 root         (0) root         (0)     1624 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_pdf_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     1854 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_server_info_api.py
--rw-r--r--   0 root         (0) root         (0)      776 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1544 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_signature_info.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_signature_placement.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)     1649 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_stamp_dto.py
--rw-r--r--   0 root         (0) root         (0)      770 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_stamp_text_color.py
--rw-r--r--   0 root         (0) root         (0)      734 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_stamp_type.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_state.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_step_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_step_definition_parallel_type.py
--rw-r--r--   0 root         (0) root         (0)      798 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_step_definition_type.py
--rw-r--r--   0 root         (0) root         (0)     4811 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      833 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     1969 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3578 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_task.py
--rw-r--r--   0 root         (0) root         (0)      860 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_template_api.py
--rw-r--r--   0 root         (0) root         (0)      755 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_template_type.py
--rw-r--r--   0 root         (0) root         (0)     1589 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1630 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_test_signature_template_request.py
--rw-r--r--   0 root         (0) root         (0)     1967 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      960 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_typology_api.py
--rw-r--r--   0 root         (0) root         (0)     1702 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     3993 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      762 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1776 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_validation_service_configuration_dto.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-03-28 15:45:04.000000 iparapheur-internal-1.11.2/test/test_workflow_api.py
--rw-r--r--   0 root         (0) root         (0)     3965 2024-03-28 15:45:03.000000 iparapheur-internal-1.11.2/test/test_workflow_definition_dto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/
+-rw-r--r--   0 root         (0) root         (0)      532 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12584 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.782265 iparapheur-internal-1.12.3/iparapheur_internal/
+-rw-r--r--   0 root         (0) root         (0)     7493 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.786265 iparapheur-internal-1.12.3/iparapheur_internal/api/
+-rw-r--r--   0 root         (0) root         (0)      994 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32735 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_advanced_config_api.py
+-rw-r--r--   0 root         (0) root         (0)    18231 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)    93433 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_layer_api.py
+-rw-r--r--   0 root         (0) root         (0)    26447 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)    35616 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_template_api.py
+-rw-r--r--   0 root         (0) root         (0)    14505 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_trash_bin_api.py
+-rw-r--r--   0 root         (0) root         (0)    18687 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    11818 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/current_user_api.py
+-rw-r--r--   0 root         (0) root         (0)    15950 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/desk_api.py
+-rw-r--r--   0 root         (0) root         (0)    27573 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    20001 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/server_info_api.py
+-rw-r--r--   0 root         (0) root         (0)    13684 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/template_api.py
+-rw-r--r--   0 root         (0) root         (0)    22740 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    25503 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/workflow_api.py
+-rw-r--r--   0 root         (0) root         (0)    25875 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    14816 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.802265 iparapheur-internal-1.12.3/iparapheur_internal/models/
+-rw-r--r--   0 root         (0) root         (0)     5957 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/action.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/create_file_stamp_request.py
+-rw-r--r--   0 root         (0) root         (0)     8955 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/create_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3562 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/detached_signature.py
+-rw-r--r--   0 root         (0) root         (0)     8680 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/document_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      909 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/external_state.py
+-rw-r--r--   0 root         (0) root         (0)     8322 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4854 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_filter_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6481 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      826 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_visibility.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_application.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_cookie.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_element.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_set.py
+-rw-r--r--   0 root         (0) root         (0)     4361 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_dpo.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_responsible.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_information_details_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/mail_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/media_type.py
+-rw-r--r--   0 root         (0) root         (0)     4064 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     4768 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4686 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4751 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4855 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_info.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4782 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/password_policies.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_info.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_placement.py
+-rw-r--r--   0 root         (0) root         (0)      833 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_dto.py
+-rw-r--r--   0 root         (0) root         (0)      800 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_text_color.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_type.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/state.py
+-rw-r--r--   0 root         (0) root         (0)     6951 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_parallel_type.py
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_type.py
+-rw-r--r--   0 root         (0) root         (0)    13624 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3619 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     7888 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/task.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/template_type.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/test_signature_template_request.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)    12060 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/validation_service_configuration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/workflow_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9290 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      532 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7530 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/test/
+-rw-r--r--   0 root         (0) root         (0)      712 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_action.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_advanced_config_api.py
+-rw-r--r--   0 root         (0) root         (0)      838 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_layer_api.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_template_api.py
+-rw-r--r--   0 root         (0) root         (0)      898 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_trash_bin_api.py
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_create_file_stamp_request.py
+-rw-r--r--   0 root         (0) root         (0)    13658 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_create_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)      872 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_current_user_api.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_detached_signature.py
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_document_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      847 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      762 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_external_state.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    13245 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_filter_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      783 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_visibility.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_application.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_cookie.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_data_element.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_data_set.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_dpo.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_responsible.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_information_details_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_mail_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      755 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)    14129 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7853 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_info.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2696 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_password_policies.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_pdf_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_server_info_api.py
+-rw-r--r--   0 root         (0) root         (0)      776 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_info.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_placement.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_stamp_dto.py
+-rw-r--r--   0 root         (0) root         (0)      770 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_stamp_text_color.py
+-rw-r--r--   0 root         (0) root         (0)      734 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_stamp_type.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_state.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_step_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_step_definition_parallel_type.py
+-rw-r--r--   0 root         (0) root         (0)      798 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_step_definition_type.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      833 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_task.py
+-rw-r--r--   0 root         (0) root         (0)      860 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_template_api.py
+-rw-r--r--   0 root         (0) root         (0)      755 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_template_type.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_test_signature_template_request.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      762 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_validation_service_configuration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_workflow_api.py
+-rw-r--r--   0 root         (0) root         (0)     3965 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_workflow_definition_dto.py
```

### Comparing `iparapheur-internal-1.11.2/PKG-INFO` & `iparapheur-internal-1.12.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iparapheur-internal
-Version: 1.11.2
+Version: 1.12.3
 Summary: iparapheur
 Home-page: 
 Author: Libriciel SCOP
 Author-email: iparapheur@libriciel.coop
 License: Affero GPL 3.0
 Keywords: OpenAPI,OpenAPI-Generator,iparapheur
 Description-Content-Type: text/markdown
```

### Comparing `iparapheur-internal-1.11.2/README.md` & `iparapheur-internal-1.12.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.11.2
+- Package version: 1.12.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -117,32 +117,35 @@
 *FolderApi* | [**generate_document_signature_verification**](docs/FolderApi.md#generate_document_signature_verification) | **POST** /api/internal/tenant/{tenantId}/folder/{folderId}/signature-report | Get the document(s) signature validation report
 *FolderApi* | [**list_folders**](docs/FolderApi.md#list_folders) | **POST** /api/internal/tenant/{tenantId}/desk/{deskId}/search/{state} | Query folders
 *ServerInfoApi* | [**get_gdpr_information_details**](docs/ServerInfoApi.md#get_gdpr_information_details) | **GET** /api/internal/serverInfo/gdpr | Get the GDPR definition
 *ServerInfoApi* | [**get_password_policies**](docs/ServerInfoApi.md#get_password_policies) | **GET** /api/internal/serverInfo/passwordPolicies | Get Password rules for the server
 *TemplateApi* | [**test_signature_template**](docs/TemplateApi.md#test_signature_template) | **POST** /api/internal/tenant/{tenantId}/templates/{templateType}/example | Test the tenant signature template
 *TypologyApi* | [**get_subtype**](docs/TypologyApi.md#get_subtype) | **GET** /api/internal/tenant/{tenantId}/typology/type/{typeId}/subtype/{subtypeId} | Get a subtype
 *TypologyApi* | [**get_type**](docs/TypologyApi.md#get_type) | **GET** /api/internal/tenant/{tenantId}/typology/type/{typeId} | Get a type with every informations set
+*WorkflowApi* | [**evaluate_workflow_selection_script**](docs/WorkflowApi.md#evaluate_workflow_selection_script) | **POST** /api/internal/tenant/{tenantId}/desk/{deskId}/evaluate-workflow-selection-script | Returns the evaluated workflow definition, using current parent desks, and given metadata on a possible selection script
 *WorkflowApi* | [**get_workflow_definition**](docs/WorkflowApi.md#get_workflow_definition) | **GET** /api/internal/tenant/{tenantId}/desk/{deskId}/workflow-definition/{workflowDefinitionKey} | Get a workflow definition with every information set
 
 
 ## Documentation For Models
 
  - [Action](docs/Action.md)
  - [CreateFileStampRequest](docs/CreateFileStampRequest.md)
+ - [CreateFolderRequest](docs/CreateFolderRequest.md)
  - [DeskRepresentation](docs/DeskRepresentation.md)
  - [DetachedSignature](docs/DetachedSignature.md)
  - [DocumentDto](docs/DocumentDto.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [ExternalSignatureConfigRepresentation](docs/ExternalSignatureConfigRepresentation.md)
  - [ExternalSignatureProvider](docs/ExternalSignatureProvider.md)
  - [ExternalState](docs/ExternalState.md)
  - [FolderDto](docs/FolderDto.md)
  - [FolderFilterDto](docs/FolderFilterDto.md)
  - [FolderListableDto](docs/FolderListableDto.md)
  - [FolderSortBy](docs/FolderSortBy.md)
+ - [FolderVisibility](docs/FolderVisibility.md)
  - [GdprApplication](docs/GdprApplication.md)
  - [GdprCookie](docs/GdprCookie.md)
  - [GdprDataElement](docs/GdprDataElement.md)
  - [GdprDataSet](docs/GdprDataSet.md)
  - [GdprDeclaringEntity](docs/GdprDeclaringEntity.md)
  - [GdprDeclaringEntityDpo](docs/GdprDeclaringEntityDpo.md)
  - [GdprDeclaringEntityResponsible](docs/GdprDeclaringEntityResponsible.md)
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/__init__.py` & `iparapheur-internal-1.12.3/iparapheur_internal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.11.2"
+__version__ = "1.12.3"
 
 # import apis into sdk package
 from iparapheur_internal.api.admin_advanced_config_api import AdminAdvancedConfigApi
 from iparapheur_internal.api.admin_desk_api import AdminDeskApi
 from iparapheur_internal.api.admin_layer_api import AdminLayerApi
 from iparapheur_internal.api.admin_seal_certificate_api import AdminSealCertificateApi
 from iparapheur_internal.api.admin_template_api import AdminTemplateApi
@@ -43,25 +43,27 @@
 from iparapheur_internal.exceptions import ApiKeyError
 from iparapheur_internal.exceptions import ApiAttributeError
 from iparapheur_internal.exceptions import ApiException
 
 # import models into sdk package
 from iparapheur_internal.models.action import Action
 from iparapheur_internal.models.create_file_stamp_request import CreateFileStampRequest
+from iparapheur_internal.models.create_folder_request import CreateFolderRequest
 from iparapheur_internal.models.desk_representation import DeskRepresentation
 from iparapheur_internal.models.detached_signature import DetachedSignature
 from iparapheur_internal.models.document_dto import DocumentDto
 from iparapheur_internal.models.error_response import ErrorResponse
 from iparapheur_internal.models.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_internal.models.external_signature_provider import ExternalSignatureProvider
 from iparapheur_internal.models.external_state import ExternalState
 from iparapheur_internal.models.folder_dto import FolderDto
 from iparapheur_internal.models.folder_filter_dto import FolderFilterDto
 from iparapheur_internal.models.folder_listable_dto import FolderListableDto
 from iparapheur_internal.models.folder_sort_by import FolderSortBy
+from iparapheur_internal.models.folder_visibility import FolderVisibility
 from iparapheur_internal.models.gdpr_application import GdprApplication
 from iparapheur_internal.models.gdpr_cookie import GdprCookie
 from iparapheur_internal.models.gdpr_data_element import GdprDataElement
 from iparapheur_internal.models.gdpr_data_set import GdprDataSet
 from iparapheur_internal.models.gdpr_declaring_entity import GdprDeclaringEntity
 from iparapheur_internal.models.gdpr_declaring_entity_dpo import GdprDeclaringEntityDpo
 from iparapheur_internal.models.gdpr_declaring_entity_responsible import GdprDeclaringEntityResponsible
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/__init__.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/admin_advanced_config_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_advanced_config_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ValidationServiceConfigurationDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "ValidationServiceConfigurationDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -148,17 +148,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ValidationServiceConfigurationDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "ValidationServiceConfigurationDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -213,17 +213,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ValidationServiceConfigurationDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "ValidationServiceConfigurationDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -336,18 +336,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -405,18 +405,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -474,18 +474,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -613,18 +613,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -682,18 +682,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -751,18 +751,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/admin_desk_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_desk_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -113,18 +113,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageHierarchisedDeskRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageHierarchisedDeskRepresentation",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -206,18 +206,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageHierarchisedDeskRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageHierarchisedDeskRepresentation",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -299,18 +299,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageHierarchisedDeskRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageHierarchisedDeskRepresentation",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/admin_layer_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_layer_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,19 +103,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '507': "ErrorResponse",
+            '201': "StampDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '201': "StampDto",
             '404': "ErrorResponse",
-            '507': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -185,19 +185,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '507': "ErrorResponse",
+            '201': "StampDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '201': "StampDto",
             '404': "ErrorResponse",
-            '507': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -267,19 +267,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '507': "ErrorResponse",
+            '201': "StampDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '201': "StampDto",
             '404': "ErrorResponse",
-            '507': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -420,20 +420,20 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '507': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
-            '507': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -495,20 +495,20 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '507': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
-            '507': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -570,20 +570,20 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '507': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
-            '507': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -722,16 +722,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '204': None,
+            '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -799,16 +799,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '204': None,
+            '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -876,16 +876,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '204': None,
+            '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1012,16 +1012,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '204': None,
+            '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1085,16 +1085,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '204': None,
+            '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1158,16 +1158,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '204': None,
+            '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -1291,17 +1291,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "LayerDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1364,17 +1364,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "LayerDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1437,17 +1437,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "LayerDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1570,18 +1570,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -1643,18 +1643,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -1716,18 +1716,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -1764,16 +1764,16 @@
         if layer_dto is not None:
             _body_params = layer_dto
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/pdf'
+                'application/pdf', 
+                'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
@@ -1872,18 +1872,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageLayerRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageLayerRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1955,18 +1955,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageLayerRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageLayerRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -2038,18 +2038,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageLayerRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageLayerRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -2189,18 +2189,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '201': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
             '200': "LayerDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -2268,18 +2268,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '201': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
             '200': "LayerDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -2347,18 +2347,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '201': "LayerDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
             '200': "LayerDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/admin_seal_certificate_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_seal_certificate_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -166,18 +166,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -239,18 +239,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -287,16 +287,16 @@
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/octet-stream'
+                'application/octet-stream', 
+                'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'spring_oauth'
@@ -385,17 +385,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageSubtypeRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageSubtypeRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -470,17 +470,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageSubtypeRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageSubtypeRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -555,17 +555,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageSubtypeRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageSubtypeRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/admin_template_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_template_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -166,18 +166,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -239,18 +239,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -287,16 +287,16 @@
         if mail_template_test_request is not None:
             _body_params = mail_template_test_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/pdf'
+                'application/pdf', 
+                'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
@@ -386,17 +386,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -458,17 +458,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -530,17 +530,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -675,18 +675,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -748,18 +748,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -821,18 +821,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -869,16 +869,16 @@
         if pdf_template_test_request is not None:
             _body_params = pdf_template_test_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/pdf'
+                'application/pdf', 
+                'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/admin_trash_bin_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_trash_bin_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageFolderListableDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageFolderListableDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -182,17 +182,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageFolderListableDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageFolderListableDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -263,17 +263,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageFolderListableDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageFolderListableDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/admin_typology_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_typology_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -114,19 +114,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageTypologyRepresentation",
             '401': "ErrorResponse",
             '406': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageTypologyRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -210,19 +210,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageTypologyRepresentation",
             '401': "ErrorResponse",
             '406': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageTypologyRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -306,19 +306,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageTypologyRepresentation",
             '401': "ErrorResponse",
             '406': "ErrorResponse",
             '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageTypologyRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/current_user_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/current_user_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -157,17 +157,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -227,17 +227,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/desk_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/desk_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageDeskRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageDeskRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -198,17 +198,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageDeskRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageDeskRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -287,17 +287,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageDeskRepresentation",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageDeskRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/folder_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/folder_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -96,18 +96,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '201': "ErrorResponse",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '201': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -169,18 +169,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '201': "ErrorResponse",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '201': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -242,18 +242,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '201': "ErrorResponse",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
             '404': "ErrorResponse",
-            '201': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -395,17 +395,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageFolderDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageFolderDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -488,17 +488,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageFolderDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageFolderDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -581,17 +581,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PageFolderDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PageFolderDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/server_info_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/server_info_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "GdprInformationDetailsDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "GdprInformationDetailsDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -147,17 +147,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "GdprInformationDetailsDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "GdprInformationDetailsDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -211,17 +211,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "GdprInformationDetailsDto",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "GdprInformationDetailsDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -329,17 +329,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PasswordPolicies",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PasswordPolicies",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -393,17 +393,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PasswordPolicies",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PasswordPolicies",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -457,17 +457,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PasswordPolicies",
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': "PasswordPolicies",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/template_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/template_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -181,17 +181,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -261,17 +261,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
+            '200': None,
             '401': "ErrorResponse",
             '403': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -316,16 +316,16 @@
             _files['signatureImage'] = signature_image
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/pdf'
+                'application/pdf', 
+                'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api/typology_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/typology_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "SubtypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -173,16 +173,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "SubtypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -249,16 +249,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "SubtypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -384,16 +384,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "TypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -456,16 +456,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "TypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -528,16 +528,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "TypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api_client.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.11.2/python'
+        self.user_agent = 'OpenAPI-Generator/1.12.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/api_response.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/configuration.py` & `iparapheur-internal-1.12.3/iparapheur_internal/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.11.2".\
+               "SDK Package Version: 1.12.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/exceptions.py` & `iparapheur-internal-1.12.3/iparapheur_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/__init__.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,27 @@
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from iparapheur_internal.models.action import Action
 from iparapheur_internal.models.create_file_stamp_request import CreateFileStampRequest
+from iparapheur_internal.models.create_folder_request import CreateFolderRequest
 from iparapheur_internal.models.desk_representation import DeskRepresentation
 from iparapheur_internal.models.detached_signature import DetachedSignature
 from iparapheur_internal.models.document_dto import DocumentDto
 from iparapheur_internal.models.error_response import ErrorResponse
 from iparapheur_internal.models.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_internal.models.external_signature_provider import ExternalSignatureProvider
 from iparapheur_internal.models.external_state import ExternalState
 from iparapheur_internal.models.folder_dto import FolderDto
 from iparapheur_internal.models.folder_filter_dto import FolderFilterDto
 from iparapheur_internal.models.folder_listable_dto import FolderListableDto
 from iparapheur_internal.models.folder_sort_by import FolderSortBy
+from iparapheur_internal.models.folder_visibility import FolderVisibility
 from iparapheur_internal.models.gdpr_application import GdprApplication
 from iparapheur_internal.models.gdpr_cookie import GdprCookie
 from iparapheur_internal.models.gdpr_data_element import GdprDataElement
 from iparapheur_internal.models.gdpr_data_set import GdprDataSet
 from iparapheur_internal.models.gdpr_declaring_entity import GdprDeclaringEntity
 from iparapheur_internal.models.gdpr_declaring_entity_dpo import GdprDeclaringEntityDpo
 from iparapheur_internal.models.gdpr_declaring_entity_responsible import GdprDeclaringEntityResponsible
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/action.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/action.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/create_file_stamp_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/create_file_stamp_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/detached_signature.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/detached_signature.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/document_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/document_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/error_response.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/external_signature_config_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/external_signature_provider.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/external_state.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/external_state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/folder_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/folder_filter_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_filter_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/folder_listable_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_listable_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/folder_sort_by.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_application.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_application.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_cookie.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_cookie.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_data_element.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_element.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_data_set.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_set.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_declaring_entity.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_declaring_entity_dpo.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_dpo.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_declaring_entity_responsible.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_responsible.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_entity.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_entity.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/gdpr_information_details_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_information_details_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/hierarchised_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/layer_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/layer_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/mail_template_test_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/mail_template_test_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/media_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/media_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/metadata_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/metadata_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_desk_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     PageDeskRepresentation
     """ # noqa: E501
     total_elements: Optional[StrictInt] = Field(default=None, alias="totalElements")
     total_pages: Optional[StrictInt] = Field(default=None, alias="totalPages")
     size: Optional[StrictInt] = None
     content: Optional[List[Optional[DeskRepresentation]]] = None
     number: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
-    pageable: Optional[PageableObject] = None
+    sort: Optional[SortObject] = None
     first: Optional[StrictBool] = None
     last: Optional[StrictBool] = None
+    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
+    pageable: Optional[PageableObject] = None
     empty: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty"]
+    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,21 +85,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
         if self.content:
             for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['content'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pageable
         if self.pageable:
             _dict['pageable'] = self.pageable.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
@@ -112,17 +108,17 @@
 
         _obj = cls.model_validate({
             "totalElements": obj.get("totalElements"),
             "totalPages": obj.get("totalPages"),
             "size": obj.get("size"),
             "content": [DeskRepresentation.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None,
             "number": obj.get("number"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "numberOfElements": obj.get("numberOfElements"),
-            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "first": obj.get("first"),
             "last": obj.get("last"),
+            "numberOfElements": obj.get("numberOfElements"),
+            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
             "empty": obj.get("empty")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_folder_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     PageFolderDto
     """ # noqa: E501
     total_elements: Optional[StrictInt] = Field(default=None, alias="totalElements")
     total_pages: Optional[StrictInt] = Field(default=None, alias="totalPages")
     size: Optional[StrictInt] = None
     content: Optional[List[FolderDto]] = None
     number: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
-    pageable: Optional[PageableObject] = None
+    sort: Optional[SortObject] = None
     first: Optional[StrictBool] = None
     last: Optional[StrictBool] = None
+    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
+    pageable: Optional[PageableObject] = None
     empty: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty"]
+    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,21 +85,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
         if self.content:
             for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['content'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pageable
         if self.pageable:
             _dict['pageable'] = self.pageable.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
@@ -112,17 +108,17 @@
 
         _obj = cls.model_validate({
             "totalElements": obj.get("totalElements"),
             "totalPages": obj.get("totalPages"),
             "size": obj.get("size"),
             "content": [FolderDto.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None,
             "number": obj.get("number"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "numberOfElements": obj.get("numberOfElements"),
-            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "first": obj.get("first"),
             "last": obj.get("last"),
+            "numberOfElements": obj.get("numberOfElements"),
+            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
             "empty": obj.get("empty")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_folder_listable_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_listable_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     PageFolderListableDto
     """ # noqa: E501
     total_elements: Optional[StrictInt] = Field(default=None, alias="totalElements")
     total_pages: Optional[StrictInt] = Field(default=None, alias="totalPages")
     size: Optional[StrictInt] = None
     content: Optional[List[FolderListableDto]] = None
     number: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
-    pageable: Optional[PageableObject] = None
+    sort: Optional[SortObject] = None
     first: Optional[StrictBool] = None
     last: Optional[StrictBool] = None
+    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
+    pageable: Optional[PageableObject] = None
     empty: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty"]
+    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,21 +85,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
         if self.content:
             for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['content'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pageable
         if self.pageable:
             _dict['pageable'] = self.pageable.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
@@ -112,17 +108,17 @@
 
         _obj = cls.model_validate({
             "totalElements": obj.get("totalElements"),
             "totalPages": obj.get("totalPages"),
             "size": obj.get("size"),
             "content": [FolderListableDto.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None,
             "number": obj.get("number"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "numberOfElements": obj.get("numberOfElements"),
-            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "first": obj.get("first"),
             "last": obj.get("last"),
+            "numberOfElements": obj.get("numberOfElements"),
+            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
             "empty": obj.get("empty")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_hierarchised_desk_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     PageHierarchisedDeskRepresentation
     """ # noqa: E501
     total_elements: Optional[StrictInt] = Field(default=None, alias="totalElements")
     total_pages: Optional[StrictInt] = Field(default=None, alias="totalPages")
     size: Optional[StrictInt] = None
     content: Optional[List[HierarchisedDeskRepresentation]] = None
     number: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
-    pageable: Optional[PageableObject] = None
+    sort: Optional[SortObject] = None
     first: Optional[StrictBool] = None
     last: Optional[StrictBool] = None
+    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
+    pageable: Optional[PageableObject] = None
     empty: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty"]
+    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,21 +85,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
         if self.content:
             for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['content'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pageable
         if self.pageable:
             _dict['pageable'] = self.pageable.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
@@ -112,17 +108,17 @@
 
         _obj = cls.model_validate({
             "totalElements": obj.get("totalElements"),
             "totalPages": obj.get("totalPages"),
             "size": obj.get("size"),
             "content": [HierarchisedDeskRepresentation.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None,
             "number": obj.get("number"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "numberOfElements": obj.get("numberOfElements"),
-            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "first": obj.get("first"),
             "last": obj.get("last"),
+            "numberOfElements": obj.get("numberOfElements"),
+            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
             "empty": obj.get("empty")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_info.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_info.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_layer_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_layer_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     PageLayerRepresentation
     """ # noqa: E501
     total_elements: Optional[StrictInt] = Field(default=None, alias="totalElements")
     total_pages: Optional[StrictInt] = Field(default=None, alias="totalPages")
     size: Optional[StrictInt] = None
     content: Optional[List[LayerRepresentation]] = None
     number: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
-    pageable: Optional[PageableObject] = None
+    sort: Optional[SortObject] = None
     first: Optional[StrictBool] = None
     last: Optional[StrictBool] = None
+    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
+    pageable: Optional[PageableObject] = None
     empty: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty"]
+    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,21 +85,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
         if self.content:
             for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['content'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pageable
         if self.pageable:
             _dict['pageable'] = self.pageable.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
@@ -112,17 +108,17 @@
 
         _obj = cls.model_validate({
             "totalElements": obj.get("totalElements"),
             "totalPages": obj.get("totalPages"),
             "size": obj.get("size"),
             "content": [LayerRepresentation.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None,
             "number": obj.get("number"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "numberOfElements": obj.get("numberOfElements"),
-            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "first": obj.get("first"),
             "last": obj.get("last"),
+            "numberOfElements": obj.get("numberOfElements"),
+            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
             "empty": obj.get("empty")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_subtype_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_subtype_representation.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     PageSubtypeRepresentation
     """ # noqa: E501
     total_elements: Optional[StrictInt] = Field(default=None, alias="totalElements")
     total_pages: Optional[StrictInt] = Field(default=None, alias="totalPages")
     size: Optional[StrictInt] = None
     content: Optional[List[SubtypeRepresentation]] = None
     number: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
-    pageable: Optional[PageableObject] = None
+    sort: Optional[SortObject] = None
     first: Optional[StrictBool] = None
     last: Optional[StrictBool] = None
+    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
+    pageable: Optional[PageableObject] = None
     empty: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty"]
+    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,21 +85,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
         if self.content:
             for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['content'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pageable
         if self.pageable:
             _dict['pageable'] = self.pageable.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
@@ -112,17 +108,17 @@
 
         _obj = cls.model_validate({
             "totalElements": obj.get("totalElements"),
             "totalPages": obj.get("totalPages"),
             "size": obj.get("size"),
             "content": [SubtypeRepresentation.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None,
             "number": obj.get("number"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "numberOfElements": obj.get("numberOfElements"),
-            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "first": obj.get("first"),
             "last": obj.get("last"),
+            "numberOfElements": obj.get("numberOfElements"),
+            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
             "empty": obj.get("empty")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/page_typology_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_typology_representation.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     PageTypologyRepresentation
     """ # noqa: E501
     total_elements: Optional[StrictInt] = Field(default=None, alias="totalElements")
     total_pages: Optional[StrictInt] = Field(default=None, alias="totalPages")
     size: Optional[StrictInt] = None
     content: Optional[List[TypologyRepresentation]] = None
     number: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
-    pageable: Optional[PageableObject] = None
+    sort: Optional[SortObject] = None
     first: Optional[StrictBool] = None
     last: Optional[StrictBool] = None
+    number_of_elements: Optional[StrictInt] = Field(default=None, alias="numberOfElements")
+    pageable: Optional[PageableObject] = None
     empty: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty"]
+    __properties: ClassVar[List[str]] = ["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,21 +85,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
         if self.content:
             for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['content'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pageable
         if self.pageable:
             _dict['pageable'] = self.pageable.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
@@ -112,17 +108,17 @@
 
         _obj = cls.model_validate({
             "totalElements": obj.get("totalElements"),
             "totalPages": obj.get("totalPages"),
             "size": obj.get("size"),
             "content": [TypologyRepresentation.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None,
             "number": obj.get("number"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "numberOfElements": obj.get("numberOfElements"),
-            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "first": obj.get("first"),
             "last": obj.get("last"),
+            "numberOfElements": obj.get("numberOfElements"),
+            "pageable": PageableObject.from_dict(obj["pageable"]) if obj.get("pageable") is not None else None,
             "empty": obj.get("empty")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/pageable_object.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/pageable_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 from typing_extensions import Self
 
 class PageableObject(BaseModel):
     """
     PageableObject
     """ # noqa: E501
     offset: Optional[StrictInt] = None
-    sort: Optional[List[SortObject]] = None
-    unpaged: Optional[StrictBool] = None
+    sort: Optional[SortObject] = None
     page_size: Optional[StrictInt] = Field(default=None, alias="pageSize")
     paged: Optional[StrictBool] = None
     page_number: Optional[StrictInt] = Field(default=None, alias="pageNumber")
-    __properties: ClassVar[List[str]] = ["offset", "sort", "unpaged", "pageSize", "paged", "pageNumber"]
+    unpaged: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["offset", "sort", "pageSize", "paged", "pageNumber", "unpaged"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -71,36 +71,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in sort (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of sort
         if self.sort:
-            for _item in self.sort:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sort'] = _items
+            _dict['sort'] = self.sort.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of PageableObject from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "offset": obj.get("offset"),
-            "sort": [SortObject.from_dict(_item) for _item in obj["sort"]] if obj.get("sort") is not None else None,
-            "unpaged": obj.get("unpaged"),
+            "sort": SortObject.from_dict(obj["sort"]) if obj.get("sort") is not None else None,
             "pageSize": obj.get("pageSize"),
             "paged": obj.get("paged"),
-            "pageNumber": obj.get("pageNumber")
+            "pageNumber": obj.get("pageNumber"),
+            "unpaged": obj.get("unpaged")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/password_policies.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/password_policies.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/pdf_signature_position.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/pdf_template_test_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_template_test_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/seal_certificate_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/signature_format.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/signature_info.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_info.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/signature_placement.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_placement.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/signature_protocol.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/sort_object.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/sort_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class SortObject(BaseModel):
     """
     SortObject
     """ # noqa: E501
-    direction: Optional[StrictStr] = None
-    null_handling: Optional[StrictStr] = Field(default=None, alias="nullHandling")
-    ascending: Optional[StrictBool] = None
-    var_property: Optional[StrictStr] = Field(default=None, alias="property")
-    ignore_case: Optional[StrictBool] = Field(default=None, alias="ignoreCase")
-    __properties: ClassVar[List[str]] = ["direction", "nullHandling", "ascending", "property", "ignoreCase"]
+    empty: Optional[StrictBool] = None
+    sorted: Optional[StrictBool] = None
+    unsorted: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["empty", "sorted", "unsorted"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -81,16 +79,14 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "direction": obj.get("direction"),
-            "nullHandling": obj.get("nullHandling"),
-            "ascending": obj.get("ascending"),
-            "property": obj.get("property"),
-            "ignoreCase": obj.get("ignoreCase")
+            "empty": obj.get("empty"),
+            "sorted": obj.get("sorted"),
+            "unsorted": obj.get("unsorted")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/stamp_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/stamp_text_color.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_text_color.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/stamp_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/state.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/step_definition_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/step_definition_parallel_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_parallel_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/step_definition_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_layer_association.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_layer_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_metadata_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/subtype_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/task.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/task.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/template_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/tenant_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/test_signature_template_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/test_signature_template_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/type_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/typology_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/typology_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/user_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/user_privilege.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/user_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/validation_service_configuration_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/validation_service_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/models/workflow_definition_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/workflow_definition_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal/rest.py` & `iparapheur-internal-1.12.3/iparapheur_internal/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal.egg-info/PKG-INFO` & `iparapheur-internal-1.12.3/iparapheur_internal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iparapheur-internal
-Version: 1.11.2
+Version: 1.12.3
 Summary: iparapheur
 Home-page: 
 Author: Libriciel SCOP
 Author-email: iparapheur@libriciel.coop
 License: Affero GPL 3.0
 Keywords: OpenAPI,OpenAPI-Generator,iparapheur
 Description-Content-Type: text/markdown
```

### Comparing `iparapheur-internal-1.11.2/iparapheur_internal.egg-info/SOURCES.txt` & `iparapheur-internal-1.12.3/iparapheur_internal.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 iparapheur_internal/api/server_info_api.py
 iparapheur_internal/api/template_api.py
 iparapheur_internal/api/typology_api.py
 iparapheur_internal/api/workflow_api.py
 iparapheur_internal/models/__init__.py
 iparapheur_internal/models/action.py
 iparapheur_internal/models/create_file_stamp_request.py
+iparapheur_internal/models/create_folder_request.py
 iparapheur_internal/models/desk_representation.py
 iparapheur_internal/models/detached_signature.py
 iparapheur_internal/models/document_dto.py
 iparapheur_internal/models/error_response.py
 iparapheur_internal/models/external_signature_config_representation.py
 iparapheur_internal/models/external_signature_provider.py
 iparapheur_internal/models/external_state.py
 iparapheur_internal/models/folder_dto.py
 iparapheur_internal/models/folder_filter_dto.py
 iparapheur_internal/models/folder_listable_dto.py
 iparapheur_internal/models/folder_sort_by.py
+iparapheur_internal/models/folder_visibility.py
 iparapheur_internal/models/gdpr_application.py
 iparapheur_internal/models/gdpr_cookie.py
 iparapheur_internal/models/gdpr_data_element.py
 iparapheur_internal/models/gdpr_data_set.py
 iparapheur_internal/models/gdpr_declaring_entity.py
 iparapheur_internal/models/gdpr_declaring_entity_dpo.py
 iparapheur_internal/models/gdpr_declaring_entity_responsible.py
@@ -105,28 +107,30 @@
 test/test_admin_desk_api.py
 test/test_admin_layer_api.py
 test/test_admin_seal_certificate_api.py
 test/test_admin_template_api.py
 test/test_admin_trash_bin_api.py
 test/test_admin_typology_api.py
 test/test_create_file_stamp_request.py
+test/test_create_folder_request.py
 test/test_current_user_api.py
 test/test_desk_api.py
 test/test_desk_representation.py
 test/test_detached_signature.py
 test/test_document_dto.py
 test/test_error_response.py
 test/test_external_signature_config_representation.py
 test/test_external_signature_provider.py
 test/test_external_state.py
 test/test_folder_api.py
 test/test_folder_dto.py
 test/test_folder_filter_dto.py
 test/test_folder_listable_dto.py
 test/test_folder_sort_by.py
+test/test_folder_visibility.py
 test/test_gdpr_application.py
 test/test_gdpr_cookie.py
 test/test_gdpr_data_element.py
 test/test_gdpr_data_set.py
 test/test_gdpr_declaring_entity.py
 test/test_gdpr_declaring_entity_dpo.py
 test/test_gdpr_declaring_entity_responsible.py
```

### Comparing `iparapheur-internal-1.11.2/pyproject.toml` & `iparapheur-internal-1.12.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iparapheur_internal"
-version = "1.11.2"
+version = "1.12.3"
 description = "iparapheur"
 authors = ["Libriciel SCOP <iparapheur@libriciel.coop>"]
 license = "Affero GPL 3.0"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "iparapheur"]
 include = ["iparapheur_internal/py.typed"]
```

### Comparing `iparapheur-internal-1.11.2/setup.py` & `iparapheur-internal-1.12.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "iparapheur-internal"
-VERSION = "1.11.2"
+VERSION = "1.12.3"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `iparapheur-internal-1.11.2/test/test_action.py` & `iparapheur-internal-1.12.3/test/test_action.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_admin_advanced_config_api.py` & `iparapheur-internal-1.12.3/test/test_admin_advanced_config_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_admin_desk_api.py` & `iparapheur-internal-1.12.3/test/test_admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_admin_layer_api.py` & `iparapheur-internal-1.12.3/test/test_admin_layer_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_admin_seal_certificate_api.py` & `iparapheur-internal-1.12.3/test/test_admin_seal_certificate_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_admin_template_api.py` & `iparapheur-internal-1.12.3/test/test_admin_template_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_admin_trash_bin_api.py` & `iparapheur-internal-1.12.3/test/test_admin_trash_bin_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_admin_typology_api.py` & `iparapheur-internal-1.12.3/test/test_admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_create_file_stamp_request.py` & `iparapheur-internal-1.12.3/test/test_create_file_stamp_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_current_user_api.py` & `iparapheur-internal-1.12.3/test/test_current_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_desk_api.py` & `iparapheur-internal-1.12.3/test/test_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_detached_signature.py` & `iparapheur-internal-1.12.3/test/test_detached_signature.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_document_dto.py` & `iparapheur-internal-1.12.3/test/test_document_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_error_response.py` & `iparapheur-internal-1.12.3/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_external_signature_config_representation.py` & `iparapheur-internal-1.12.3/test/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_external_signature_provider.py` & `iparapheur-internal-1.12.3/test/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_external_state.py` & `iparapheur-internal-1.12.3/test/test_external_state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_folder_api.py` & `iparapheur-internal-1.12.3/test/test_folder_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_folder_dto.py` & `iparapheur-internal-1.12.3/test/test_folder_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_folder_filter_dto.py` & `iparapheur-internal-1.12.3/test/test_folder_filter_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_folder_listable_dto.py` & `iparapheur-internal-1.12.3/test/test_folder_listable_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_folder_sort_by.py` & `iparapheur-internal-1.12.3/test/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_application.py` & `iparapheur-internal-1.12.3/test/test_gdpr_application.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_cookie.py` & `iparapheur-internal-1.12.3/test/test_gdpr_cookie.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_data_element.py` & `iparapheur-internal-1.12.3/test/test_gdpr_data_element.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_data_set.py` & `iparapheur-internal-1.12.3/test/test_gdpr_data_set.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_declaring_entity.py` & `iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_declaring_entity_dpo.py` & `iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_dpo.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_declaring_entity_responsible.py` & `iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_responsible.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_entity.py` & `iparapheur-internal-1.12.3/test/test_gdpr_entity.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_gdpr_information_details_dto.py` & `iparapheur-internal-1.12.3/test/test_gdpr_information_details_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_hierarchised_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_layer_dto.py` & `iparapheur-internal-1.12.3/test/test_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_layer_representation.py` & `iparapheur-internal-1.12.3/test/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_mail_template_test_request.py` & `iparapheur-internal-1.12.3/test/test_mail_template_test_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_media_type.py` & `iparapheur-internal-1.12.3/test/test_media_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_metadata_dto.py` & `iparapheur-internal-1.12.3/test/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_metadata_type.py` & `iparapheur-internal-1.12.3/test/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_page_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_page_layer_representation.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,77 +11,68 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.page_desk_representation import PageDeskRepresentation
+from iparapheur_internal.models.page_layer_representation import PageLayerRepresentation
 
-class TestPageDeskRepresentation(unittest.TestCase):
-    """PageDeskRepresentation unit test stubs"""
+class TestPageLayerRepresentation(unittest.TestCase):
+    """PageLayerRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageDeskRepresentation:
-        """Test PageDeskRepresentation
+    def make_instance(self, include_optional) -> PageLayerRepresentation:
+        """Test PageLayerRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageDeskRepresentation`
+        # uncomment below to create an instance of `PageLayerRepresentation`
         """
-        model = PageDeskRepresentation()
+        model = PageLayerRepresentation()
         if include_optional:
-            return PageDeskRepresentation(
+            return PageLayerRepresentation(
                 total_elements = 56,
                 total_pages = 56,
                 size = 56,
                 content = [
-                    iparapheur_internal.models.desk_representation.DeskRepresentation(
+                    iparapheur_internal.models.layer_representation.LayerRepresentation(
                         id = '', 
-                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                        tenant_id = '', )
+                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', )
                     ],
                 number = 56,
-                sort = [
-                    iparapheur_internal.models.sort_object.SortObject(
-                        direction = '', 
-                        null_handling = '', 
-                        ascending = True, 
-                        property = '', 
-                        ignore_case = True, )
-                    ],
+                sort = iparapheur_internal.models.sort_object.SortObject(
+                    empty = True, 
+                    sorted = True, 
+                    unsorted = True, ),
+                first = True,
+                last = True,
                 number_of_elements = 56,
                 pageable = iparapheur_internal.models.pageable_object.PageableObject(
                     offset = 56, 
-                    sort = [
-                        iparapheur_internal.models.sort_object.SortObject(
-                            direction = '', 
-                            null_handling = '', 
-                            ascending = True, 
-                            property = '', 
-                            ignore_case = True, )
-                        ], 
-                    unpaged = True, 
+                    sort = iparapheur_internal.models.sort_object.SortObject(
+                        empty = True, 
+                        sorted = True, 
+                        unsorted = True, ), 
                     page_size = 56, 
                     paged = True, 
-                    page_number = 56, ),
-                first = True,
-                last = True,
+                    page_number = 56, 
+                    unpaged = True, ),
                 empty = True
             )
         else:
-            return PageDeskRepresentation(
+            return PageLayerRepresentation(
         )
         """
 
-    def testPageDeskRepresentation(self):
-        """Test PageDeskRepresentation"""
+    def testPageLayerRepresentation(self):
+        """Test PageLayerRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.2/test/test_page_folder_dto.py` & `iparapheur-internal-1.12.3/test/test_create_folder_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,275 +11,282 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.page_folder_dto import PageFolderDto
+from iparapheur_internal.models.create_folder_request import CreateFolderRequest
 
-class TestPageFolderDto(unittest.TestCase):
-    """PageFolderDto unit test stubs"""
+class TestCreateFolderRequest(unittest.TestCase):
+    """CreateFolderRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageFolderDto:
-        """Test PageFolderDto
+    def make_instance(self, include_optional) -> CreateFolderRequest:
+        """Test CreateFolderRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageFolderDto`
+        # uncomment below to create an instance of `CreateFolderRequest`
         """
-        model = PageFolderDto()
+        model = CreateFolderRequest()
         if include_optional:
-            return PageFolderDto(
-                total_elements = 56,
-                total_pages = 56,
-                size = 56,
-                content = [
-                    iparapheur_internal.models.folder_dto.FolderDto(
+            return CreateFolderRequest(
+                id = '',
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
+                due_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                metadata = {
+                    'key' : ''
+                    },
+                draft_creation_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                type = iparapheur_internal.models.type_dto.TypeDto(
+                    id = '', 
+                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                    description = '012', 
+                    signature_format = 'PKCS7', 
+                    protocol = 'HELIOS', 
+                    signature_visible = True, 
+                    signature_position = iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
+                        x = 1.337, 
+                        y = 1.337, 
+                        page = 56, 
+                        template_type = 'MAIL_NOTIFICATION_SINGLE', ), 
+                    signature_location = '', 
+                    signature_zip_code = '', ),
+                subtype = iparapheur_internal.models.subtype_dto.SubtypeDto(
+                    id = '', 
+                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                    description = '012', 
+                    creation_workflow_id = '', 
+                    validation_workflow_id = '', 
+                    workflow_selection_script = '', 
+                    annotations_allowed = True, 
+                    external_signature_automatic = True, 
+                    secure_mail_server_id = 56, 
+                    seal_certificate_id = '', 
+                    seal_certificate = iparapheur_internal.models.seal_certificate_representation.SealCertificateRepresentation(
+                        id = '', 
+                        name = 'Example certificate', 
+                        expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        usage_count = 56, ), 
+                    subtype_metadata_list = [
+                        iparapheur_internal.models.subtype_metadata_dto.SubtypeMetadataDto(
+                            metadata_id = '', 
+                            metadata = iparapheur_internal.models.metadata_dto.MetadataDto(
+                                id = '', 
+                                name = 'Example metadata', 
+                                key = 'example_metadata', 
+                                index = 56, 
+                                type = 'TEXT', 
+                                restricted_values = [
+                                    ''
+                                    ], ), 
+                            default_value = '', 
+                            mandatory = True, 
+                            editable = True, )
+                        ], 
+                    subtype_layers = [
+                        iparapheur_internal.models.subtype_layer_dto.SubtypeLayerDto(
+                            layer_id = '', 
+                            layer = iparapheur_internal.models.layer_representation.LayerRepresentation(
+                                id = '', 
+                                name = 'jXAuKb%@;_5)#fEb-bx%oZ01', ), 
+                            association = 'ALL', )
+                        ], 
+                    external_signature_config_id = '', 
+                    external_signature_config = iparapheur_internal.models.external_signature_config_representation.ExternalSignatureConfigRepresentation(
+                        id = '', 
+                        name = '01', 
+                        service_name = 'YOUSIGN_V2', 
+                        url = '', 
+                        login = '', ), 
+                    creation_permitted_desk_ids = [
+                        ''
+                        ], 
+                    creation_permitted_desks = [
+                        iparapheur_internal.models.desk_representation.DeskRepresentation(
+                            id = '', 
+                            name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                            tenant_id = '', )
+                        ], 
+                    filterable_by_desk_ids = [
+                        ''
+                        ], 
+                    filterable_by_desks = [
+                        iparapheur_internal.models.desk_representation.DeskRepresentation(
+                            id = '', 
+                            name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                            tenant_id = '', )
+                        ], 
+                    max_main_documents = 56, 
+                    multi_documents = True, 
+                    annexe_included = True, 
+                    digital_signature_mandatory = True, 
+                    reading_mandatory = True, 
+                    seal_automatic = True, ),
+                origin_desk = iparapheur_internal.models.desk_representation.DeskRepresentation(
+                    id = '', 
+                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                    tenant_id = '', ),
+                final_desk = iparapheur_internal.models.desk_representation.DeskRepresentation(
+                    id = '', 
+                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                    tenant_id = '', ),
+                is_read_by_current_user = True,
+                legacy_id = '',
+                type_id = '',
+                subtype_id = '',
+                step_list = [
+                    iparapheur_internal.models.task.Task(
                         id = '', 
-                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                        due_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         metadata = {
                             'key' : ''
                             }, 
-                        draft_creation_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        type = iparapheur_internal.models.type_dto.TypeDto(
+                        action = 'VISA', 
+                        performed_action = 'VISA', 
+                        external_state = 'FORM', 
+                        state = 'DRAFT', 
+                        desks = [
+                            iparapheur_internal.models.desk_representation.DeskRepresentation(
+                                id = '', 
+                                name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                                tenant_id = '', )
+                            ], 
+                        delegated_by_desk = iparapheur_internal.models.desk_representation.DeskRepresentation(
                             id = '', 
                             name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                            description = '012', 
-                            signature_format = 'PKCS7', 
-                            protocol = 'HELIOS', 
-                            signature_visible = True, 
-                            signature_position = iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
-                                x = 1.337, 
-                                y = 1.337, 
-                                page = 56, 
-                                template_type = 'MAIL_NOTIFICATION_SINGLE', ), 
-                            signature_location = '', 
-                            signature_zip_code = '', ), 
-                        subtype = iparapheur_internal.models.subtype_dto.SubtypeDto(
+                            tenant_id = '', ), 
+                        user = iparapheur_internal.models.user_representation.UserRepresentation(
                             id = '', 
-                            name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                            description = '012', 
-                            creation_workflow_id = '', 
-                            validation_workflow_id = '', 
-                            workflow_selection_script = '', 
-                            annotations_allowed = True, 
-                            external_signature_automatic = True, 
-                            secure_mail_server_id = 56, 
-                            seal_certificate_id = '', 
-                            seal_certificate = iparapheur_internal.models.seal_certificate_representation.SealCertificateRepresentation(
-                                id = '', 
-                                name = 'Example certificate', 
-                                expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                                usage_count = 56, ), 
-                            subtype_metadata_list = [
-                                iparapheur_internal.models.subtype_metadata_dto.SubtypeMetadataDto(
-                                    metadata_id = '', 
-                                    default_value = '', 
-                                    mandatory = True, 
-                                    editable = True, )
-                                ], 
-                            subtype_layers = [
-                                iparapheur_internal.models.subtype_layer_dto.SubtypeLayerDto(
-                                    layer_id = '', 
-                                    layer = iparapheur_internal.models.layer_representation.LayerRepresentation(
-                                        id = '', 
-                                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', ), 
-                                    association = 'ALL', )
-                                ], 
-                            external_signature_config_id = '', 
-                            external_signature_config = iparapheur_internal.models.external_signature_config_representation.ExternalSignatureConfigRepresentation(
-                                id = '', 
-                                name = '01', 
-                                service_name = 'YOUSIGN_V2', 
-                                url = '', 
-                                login = '', ), 
-                            creation_permitted_desk_ids = [
-                                ''
-                                ], 
-                            creation_permitted_desks = [
-                                iparapheur_internal.models.desk_representation.DeskRepresentation(
-                                    id = '', 
-                                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                                    tenant_id = '', )
-                                ], 
-                            filterable_by_desk_ids = [
-                                ''
-                                ], 
-                            filterable_by_desks = [
-                                iparapheur_internal.models.desk_representation.DeskRepresentation(
-                                    id = '', 
-                                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                                    tenant_id = '', )
-                                ], 
-                            max_main_documents = 56, 
-                            multi_documents = True, 
-                            annexe_included = True, 
-                            digital_signature_mandatory = True, 
-                            reading_mandatory = True, 
-                            seal_automatic = True, ), 
-                        origin_desk = , 
-                        final_desk = , 
-                        is_read_by_current_user = True, 
-                        legacy_id = '', 
-                        type_id = '', 
-                        subtype_id = '', 
-                        step_list = [
-                            iparapheur_internal.models.task.Task(
+                            user_name = '0', 
+                            first_name = '', 
+                            last_name = '', 
+                            email = '', 
+                            privilege = 'NONE', 
+                            is_ldap_synchronized = True, ), 
+                        read_by_user_ids = [
+                            ''
+                            ], 
+                        public_certificate_base64 = '', 
+                        external_signature_procedure_id = '', 
+                        begin_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        draft_creation_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        public_annotation = '', 
+                        private_annotation = '', 
+                        notified_desks = [
+                            
+                            ], 
+                        workflow_index = 56, 
+                        step_index = 56, 
+                        mandatory_validation_metadata = [
+                            ''
+                            ], 
+                        mandatory_rejection_metadata = [
+                            ''
+                            ], 
+                        instance_name = '', )
+                    ],
+                document_list = [
+                    iparapheur_internal.models.document_dto.DocumentDto(
+                        id = '', 
+                        name = '', 
+                        index = 56, 
+                        page_count = 56, 
+                        content_length = 56, 
+                        media_type = iparapheur_internal.models.media_type.MediaType(
+                            type = '', 
+                            subtype = '', 
+                            parameters = {
+                                'key' : ''
+                                }, 
+                            quality_value = 1.337, 
+                            wildcard_type = True, 
+                            wildcard_subtype = True, 
+                            subtype_suffix = '', 
+                            charset = '', 
+                            concrete = True, ), 
+                        pages_properties = {
+                            'key' : iparapheur_internal.models.page_info.PageInfo(
+                                width = 1.337, 
+                                height = 1.337, 
+                                rotation = 56, )
+                            }, 
+                        pdf_visual_id = '', 
+                        signature_placement_annotations = [
+                            iparapheur_internal.models.signature_placement.SignaturePlacement(
                                 id = '', 
-                                action = 'VISA', 
-                                performed_action = 'VISA', 
-                                external_state = 'FORM', 
-                                state = 'DRAFT', 
-                                desks = [
-                                    
-                                    ], 
-                                delegated_by_desk = , 
-                                user = iparapheur_internal.models.user_representation.UserRepresentation(
-                                    id = '', 
-                                    user_name = '0', 
-                                    first_name = '', 
-                                    last_name = '', 
-                                    email = '', 
-                                    privilege = 'NONE', 
-                                    is_ldap_synchronized = True, ), 
-                                read_by_user_ids = [
-                                    ''
-                                    ], 
-                                public_certificate_base64 = '', 
-                                external_signature_procedure_id = '', 
-                                begin_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                                date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                                draft_creation_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                                public_annotation = '', 
-                                private_annotation = '', 
-                                notified_desks = [
-                                    
-                                    ], 
-                                workflow_index = 56, 
-                                step_index = 56, 
-                                mandatory_validation_metadata = [
-                                    ''
-                                    ], 
-                                mandatory_rejection_metadata = [
-                                    ''
-                                    ], 
-                                instance_name = '', )
+                                page = 1, 
+                                width = 15, 
+                                height = 15, 
+                                x = 56, 
+                                y = 56, 
+                                page_rotation = 0, 
+                                page_width = 276, 
+                                page_height = 308, 
+                                rectangle_origin = 'TOP_RIGHT', 
+                                signature_number = 0, 
+                                template_type = 'MAIL_NOTIFICATION_SINGLE', )
                             ], 
-                        document_list = [
-                            iparapheur_internal.models.document_dto.DocumentDto(
+                        signature_tags = {
+                            'key' : iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
+                                x = 1.337, 
+                                y = 1.337, 
+                                page = 56, )
+                            }, 
+                        seal_tags = {
+                            'key' : iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
+                                x = 1.337, 
+                                y = 1.337, 
+                                page = 56, )
+                            }, 
+                        detached_signatures = [
+                            iparapheur_internal.models.detached_signature.DetachedSignature(
                                 id = '', 
                                 name = '', 
-                                index = 56, 
-                                page_count = 56, 
                                 content_length = 56, 
-                                media_type = iparapheur_internal.models.media_type.MediaType(
-                                    parameters = {
-                                        'key' : ''
-                                        }, 
-                                    quality_value = 1.337, 
-                                    wildcard_type = True, 
-                                    wildcard_subtype = True, 
-                                    subtype_suffix = '', 
-                                    charset = '', 
-                                    concrete = True, ), 
-                                pages_properties = {
-                                    'key' : iparapheur_internal.models.page_info.PageInfo(
-                                        width = 1.337, 
-                                        height = 1.337, 
-                                        rotation = 56, )
-                                    }, 
-                                pdf_visual_id = '', 
-                                signature_placement_annotations = [
-                                    iparapheur_internal.models.signature_placement.SignaturePlacement(
-                                        id = '', 
-                                        page = 1, 
-                                        width = 15, 
-                                        height = 15, 
-                                        x = 56, 
-                                        y = 56, 
-                                        page_rotation = 0, 
-                                        page_width = 276, 
-                                        page_height = 308, 
-                                        rectangle_origin = 'TOP_RIGHT', 
-                                        signature_number = 0, )
-                                    ], 
-                                signature_tags = {
-                                    'key' : iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
-                                        x = 1.337, 
-                                        y = 1.337, 
-                                        page = 56, )
-                                    }, 
-                                seal_tags = {
-                                    'key' : 
-                                    }, 
-                                detached_signatures = [
-                                    iparapheur_internal.models.detached_signature.DetachedSignature(
-                                        id = '', 
-                                        name = '', 
-                                        content_length = 56, 
-                                        target_document_id = '', 
-                                        target_task_id = '', )
-                                    ], 
-                                embedded_signature_infos = [
-                                    iparapheur_internal.models.signature_info.SignatureInfo(
-                                        signature_date_time = 56, 
-                                        is_signature_valid = True, 
-                                        name = '', 
-                                        issuer_name = '', )
-                                    ], 
-                                signature_proof = True, 
-                                deletable = True, 
-                                is_main_document = True, )
+                                target_document_id = '', 
+                                target_task_id = '', )
                             ], 
-                        read_by_user_ids = [
-                            ''
+                        embedded_signature_infos = [
+                            iparapheur_internal.models.signature_info.SignatureInfo(
+                                signature_date_time = 56, 
+                                is_signature_valid = True, 
+                                name = '', 
+                                issuer_name = '', )
                             ], 
-                        read_by_current_user = True, )
+                        signature_proof = True, 
+                        deletable = True, 
+                        is_main_document = True, )
                     ],
-                number = 56,
-                sort = [
-                    iparapheur_internal.models.sort_object.SortObject(
-                        direction = '', 
-                        null_handling = '', 
-                        ascending = True, 
-                        property = '', 
-                        ignore_case = True, )
+                read_by_user_ids = [
+                    ''
                     ],
-                number_of_elements = 56,
-                pageable = iparapheur_internal.models.pageable_object.PageableObject(
-                    offset = 56, 
-                    sort = [
-                        iparapheur_internal.models.sort_object.SortObject(
-                            direction = '', 
-                            null_handling = '', 
-                            ascending = True, 
-                            property = '', 
-                            ignore_case = True, )
-                        ], 
-                    unpaged = True, 
-                    page_size = 56, 
-                    paged = True, 
-                    page_number = 56, ),
-                first = True,
-                last = True,
-                empty = True
+                variable_desks_ids = {
+                    'key' : ''
+                    },
+                detached_signatures_mapping = {
+                    'key' : [
+                        ''
+                        ]
+                    },
+                visibility = 'CONFIDENTIAL',
+                read_by_current_user = True
             )
         else:
-            return PageFolderDto(
+            return CreateFolderRequest(
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
         )
         """
 
-    def testPageFolderDto(self):
-        """Test PageFolderDto"""
+    def testCreateFolderRequest(self):
+        """Test CreateFolderRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.2/test/test_page_folder_listable_dto.py` & `iparapheur-internal-1.12.3/test/test_page_folder_listable_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,39 +127,31 @@
                         origin_desk = , 
                         final_desk = , 
                         is_read_by_current_user = True, 
                         legacy_id = '', 
                         read_by_current_user = True, )
                     ],
                 number = 56,
-                sort = [
-                    iparapheur_internal.models.sort_object.SortObject(
-                        direction = '', 
-                        null_handling = '', 
-                        ascending = True, 
-                        property = '', 
-                        ignore_case = True, )
-                    ],
+                sort = iparapheur_internal.models.sort_object.SortObject(
+                    empty = True, 
+                    sorted = True, 
+                    unsorted = True, ),
+                first = True,
+                last = True,
                 number_of_elements = 56,
                 pageable = iparapheur_internal.models.pageable_object.PageableObject(
                     offset = 56, 
-                    sort = [
-                        iparapheur_internal.models.sort_object.SortObject(
-                            direction = '', 
-                            null_handling = '', 
-                            ascending = True, 
-                            property = '', 
-                            ignore_case = True, )
-                        ], 
-                    unpaged = True, 
+                    sort = iparapheur_internal.models.sort_object.SortObject(
+                        empty = True, 
+                        sorted = True, 
+                        unsorted = True, ), 
                     page_size = 56, 
                     paged = True, 
-                    page_number = 56, ),
-                first = True,
-                last = True,
+                    page_number = 56, 
+                    unpaged = True, ),
                 empty = True
             )
         else:
             return PageFolderListableDto(
         )
         """
```

### Comparing `iparapheur-internal-1.11.2/test/test_page_hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_page_hierarchised_desk_representation.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,39 +44,31 @@
                         id = '', 
                         name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
                         tenant_id = '', 
                         direct_children_count = 56, 
                         level = 56, )
                     ],
                 number = 56,
-                sort = [
-                    iparapheur_internal.models.sort_object.SortObject(
-                        direction = '', 
-                        null_handling = '', 
-                        ascending = True, 
-                        property = '', 
-                        ignore_case = True, )
-                    ],
+                sort = iparapheur_internal.models.sort_object.SortObject(
+                    empty = True, 
+                    sorted = True, 
+                    unsorted = True, ),
+                first = True,
+                last = True,
                 number_of_elements = 56,
                 pageable = iparapheur_internal.models.pageable_object.PageableObject(
                     offset = 56, 
-                    sort = [
-                        iparapheur_internal.models.sort_object.SortObject(
-                            direction = '', 
-                            null_handling = '', 
-                            ascending = True, 
-                            property = '', 
-                            ignore_case = True, )
-                        ], 
-                    unpaged = True, 
+                    sort = iparapheur_internal.models.sort_object.SortObject(
+                        empty = True, 
+                        sorted = True, 
+                        unsorted = True, ), 
                     page_size = 56, 
                     paged = True, 
-                    page_number = 56, ),
-                first = True,
-                last = True,
+                    page_number = 56, 
+                    unpaged = True, ),
                 empty = True
             )
         else:
             return PageHierarchisedDeskRepresentation(
         )
         """
```

### Comparing `iparapheur-internal-1.11.2/test/test_page_info.py` & `iparapheur-internal-1.12.3/test/test_page_info.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_page_subtype_representation.py` & `iparapheur-internal-1.12.3/test/test_page_desk_representation.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,76 +11,69 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.page_subtype_representation import PageSubtypeRepresentation
+from iparapheur_internal.models.page_desk_representation import PageDeskRepresentation
 
-class TestPageSubtypeRepresentation(unittest.TestCase):
-    """PageSubtypeRepresentation unit test stubs"""
+class TestPageDeskRepresentation(unittest.TestCase):
+    """PageDeskRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageSubtypeRepresentation:
-        """Test PageSubtypeRepresentation
+    def make_instance(self, include_optional) -> PageDeskRepresentation:
+        """Test PageDeskRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageSubtypeRepresentation`
+        # uncomment below to create an instance of `PageDeskRepresentation`
         """
-        model = PageSubtypeRepresentation()
+        model = PageDeskRepresentation()
         if include_optional:
-            return PageSubtypeRepresentation(
+            return PageDeskRepresentation(
                 total_elements = 56,
                 total_pages = 56,
                 size = 56,
                 content = [
-                    iparapheur_internal.models.subtype_representation.SubtypeRepresentation(
+                    iparapheur_internal.models.desk_representation.DeskRepresentation(
                         id = '', 
-                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', )
+                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                        tenant_id = '', )
                     ],
                 number = 56,
-                sort = [
-                    iparapheur_internal.models.sort_object.SortObject(
-                        direction = '', 
-                        null_handling = '', 
-                        ascending = True, 
-                        property = '', 
-                        ignore_case = True, )
-                    ],
+                sort = iparapheur_internal.models.sort_object.SortObject(
+                    empty = True, 
+                    sorted = True, 
+                    unsorted = True, ),
+                first = True,
+                last = True,
                 number_of_elements = 56,
                 pageable = iparapheur_internal.models.pageable_object.PageableObject(
                     offset = 56, 
-                    sort = [
-                        iparapheur_internal.models.sort_object.SortObject(
-                            direction = '', 
-                            null_handling = '', 
-                            ascending = True, 
-                            property = '', 
-                            ignore_case = True, )
-                        ], 
-                    unpaged = True, 
+                    sort = iparapheur_internal.models.sort_object.SortObject(
+                        empty = True, 
+                        sorted = True, 
+                        unsorted = True, ), 
                     page_size = 56, 
                     paged = True, 
-                    page_number = 56, ),
-                first = True,
-                last = True,
+                    page_number = 56, 
+                    unpaged = True, ),
                 empty = True
             )
         else:
-            return PageSubtypeRepresentation(
+            return PageDeskRepresentation(
         )
         """
 
-    def testPageSubtypeRepresentation(self):
-        """Test PageSubtypeRepresentation"""
+    def testPageDeskRepresentation(self):
+        """Test PageDeskRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.2/test/test_page_typology_representation.py` & `iparapheur-internal-1.12.3/test/test_typology_representation.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,78 +11,46 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.page_typology_representation import PageTypologyRepresentation
+from iparapheur_internal.models.typology_representation import TypologyRepresentation
 
-class TestPageTypologyRepresentation(unittest.TestCase):
-    """PageTypologyRepresentation unit test stubs"""
+class TestTypologyRepresentation(unittest.TestCase):
+    """TypologyRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageTypologyRepresentation:
-        """Test PageTypologyRepresentation
+    def make_instance(self, include_optional) -> TypologyRepresentation:
+        """Test TypologyRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageTypologyRepresentation`
+        # uncomment below to create an instance of `TypologyRepresentation`
         """
-        model = PageTypologyRepresentation()
+        model = TypologyRepresentation()
         if include_optional:
-            return PageTypologyRepresentation(
-                total_elements = 56,
-                total_pages = 56,
-                size = 56,
-                content = [
-                    iparapheur_internal.models.typology_representation.TypologyRepresentation(
-                        id = '', 
-                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                        parent_id = '', 
-                        children_count = 56, )
-                    ],
-                number = 56,
-                sort = [
-                    iparapheur_internal.models.sort_object.SortObject(
-                        direction = '', 
-                        null_handling = '', 
-                        ascending = True, 
-                        property = '', 
-                        ignore_case = True, )
-                    ],
-                number_of_elements = 56,
-                pageable = iparapheur_internal.models.pageable_object.PageableObject(
-                    offset = 56, 
-                    sort = [
-                        iparapheur_internal.models.sort_object.SortObject(
-                            direction = '', 
-                            null_handling = '', 
-                            ascending = True, 
-                            property = '', 
-                            ignore_case = True, )
-                        ], 
-                    unpaged = True, 
-                    page_size = 56, 
-                    paged = True, 
-                    page_number = 56, ),
-                first = True,
-                last = True,
-                empty = True
+            return TypologyRepresentation(
+                id = '',
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
+                parent_id = '',
+                children_count = 56
             )
         else:
-            return PageTypologyRepresentation(
+            return TypologyRepresentation(
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
         )
         """
 
-    def testPageTypologyRepresentation(self):
-        """Test PageTypologyRepresentation"""
+    def testTypologyRepresentation(self):
+        """Test TypologyRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.2/test/test_pageable_object.py` & `iparapheur-internal-1.12.3/test/test_pageable_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,26 +33,22 @@
             optional params are included """
         # uncomment below to create an instance of `PageableObject`
         """
         model = PageableObject()
         if include_optional:
             return PageableObject(
                 offset = 56,
-                sort = [
-                    iparapheur_internal.models.sort_object.SortObject(
-                        direction = '', 
-                        null_handling = '', 
-                        ascending = True, 
-                        property = '', 
-                        ignore_case = True, )
-                    ],
-                unpaged = True,
+                sort = iparapheur_internal.models.sort_object.SortObject(
+                    empty = True, 
+                    sorted = True, 
+                    unsorted = True, ),
                 page_size = 56,
                 paged = True,
-                page_number = 56
+                page_number = 56,
+                unpaged = True
             )
         else:
             return PageableObject(
         )
         """
 
     def testPageableObject(self):
```

### Comparing `iparapheur-internal-1.11.2/test/test_password_policies.py` & `iparapheur-internal-1.12.3/test/test_password_policies.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_pdf_signature_position.py` & `iparapheur-internal-1.12.3/test/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_pdf_template_test_request.py` & `iparapheur-internal-1.12.3/test/test_pdf_template_test_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_seal_certificate_representation.py` & `iparapheur-internal-1.12.3/test/test_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_server_info_api.py` & `iparapheur-internal-1.12.3/test/test_server_info_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_signature_format.py` & `iparapheur-internal-1.12.3/test/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_signature_info.py` & `iparapheur-internal-1.12.3/test/test_signature_info.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_signature_placement.py` & `iparapheur-internal-1.12.3/test/test_signature_placement.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_signature_protocol.py` & `iparapheur-internal-1.12.3/test/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_sort_object.py` & `iparapheur-internal-1.12.3/test/test_sort_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,19 +32,17 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `SortObject`
         """
         model = SortObject()
         if include_optional:
             return SortObject(
-                direction = '',
-                null_handling = '',
-                ascending = True,
-                var_property = '',
-                ignore_case = True
+                empty = True,
+                sorted = True,
+                unsorted = True
             )
         else:
             return SortObject(
         )
         """
 
     def testSortObject(self):
```

### Comparing `iparapheur-internal-1.11.2/test/test_stamp_dto.py` & `iparapheur-internal-1.12.3/test/test_stamp_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_stamp_text_color.py` & `iparapheur-internal-1.12.3/test/test_stamp_text_color.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_stamp_type.py` & `iparapheur-internal-1.12.3/test/test_stamp_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_state.py` & `iparapheur-internal-1.12.3/test/test_state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_step_definition_dto.py` & `iparapheur-internal-1.12.3/test/test_step_definition_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_step_definition_parallel_type.py` & `iparapheur-internal-1.12.3/test/test_step_definition_parallel_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_step_definition_type.py` & `iparapheur-internal-1.12.3/test/test_step_definition_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_subtype_dto.py` & `iparapheur-internal-1.12.3/test/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_subtype_layer_association.py` & `iparapheur-internal-1.12.3/test/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_subtype_layer_dto.py` & `iparapheur-internal-1.12.3/test/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_subtype_metadata_dto.py` & `iparapheur-internal-1.12.3/test/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_subtype_representation.py` & `iparapheur-internal-1.12.3/test/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_task.py` & `iparapheur-internal-1.12.3/test/test_task.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_template_api.py` & `iparapheur-internal-1.12.3/test/test_template_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_template_type.py` & `iparapheur-internal-1.12.3/test/test_template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_tenant_representation.py` & `iparapheur-internal-1.12.3/test/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_test_signature_template_request.py` & `iparapheur-internal-1.12.3/test/test_test_signature_template_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_type_dto.py` & `iparapheur-internal-1.12.3/test/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_typology_api.py` & `iparapheur-internal-1.12.3/test/test_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_typology_representation.py` & `iparapheur-internal-1.12.3/test/test_user_representation.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,46 +11,53 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.typology_representation import TypologyRepresentation
+from iparapheur_internal.models.user_representation import UserRepresentation
 
-class TestTypologyRepresentation(unittest.TestCase):
-    """TypologyRepresentation unit test stubs"""
+class TestUserRepresentation(unittest.TestCase):
+    """UserRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> TypologyRepresentation:
-        """Test TypologyRepresentation
+    def make_instance(self, include_optional) -> UserRepresentation:
+        """Test UserRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `TypologyRepresentation`
+        # uncomment below to create an instance of `UserRepresentation`
         """
-        model = TypologyRepresentation()
+        model = UserRepresentation()
         if include_optional:
-            return TypologyRepresentation(
+            return UserRepresentation(
                 id = '',
-                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
-                parent_id = '',
-                children_count = 56
+                user_name = '0',
+                first_name = '',
+                last_name = '',
+                email = '',
+                privilege = 'NONE',
+                is_ldap_synchronized = True
             )
         else:
-            return TypologyRepresentation(
-                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
+            return UserRepresentation(
+                user_name = '0',
+                first_name = '',
+                last_name = '',
+                email = '',
+                privilege = 'NONE',
         )
         """
 
-    def testTypologyRepresentation(self):
-        """Test TypologyRepresentation"""
+    def testUserRepresentation(self):
+        """Test UserRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.2/test/test_user_dto.py` & `iparapheur-internal-1.12.3/test/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_user_privilege.py` & `iparapheur-internal-1.12.3/test/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_validation_service_configuration_dto.py` & `iparapheur-internal-1.12.3/test/test_validation_service_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.2/test/test_workflow_api.py` & `iparapheur-internal-1.12.3/test/test_workflow_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 
     def setUp(self) -> None:
         self.api = WorkflowApi()
 
     def tearDown(self) -> None:
         pass
 
+    def test_evaluate_workflow_selection_script(self) -> None:
+        """Test case for evaluate_workflow_selection_script
+
+        Returns the evaluated workflow definition, using current parent desks, and given metadata on a possible selection script
+        """
+        pass
+
     def test_get_workflow_definition(self) -> None:
         """Test case for get_workflow_definition
 
         Get a workflow definition with every information set
         """
         pass
```

### Comparing `iparapheur-internal-1.11.2/test/test_workflow_definition_dto.py` & `iparapheur-internal-1.12.3/test/test_workflow_definition_dto.py`

 * *Files identical despite different names*

