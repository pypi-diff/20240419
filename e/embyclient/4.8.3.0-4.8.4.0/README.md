# Comparing `tmp/embyclient-4.8.3.0.tar.gz` & `tmp/embyclient-4.8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embyclient-4.8.3.0.tar", last modified: Fri Mar 15 07:48:22 2024, max compression
+gzip compressed data, was "embyclient-4.8.4.0.tar", last modified: Fri Apr 19 00:16:42 2024, max compression
```

## Comparing `embyclient-4.8.3.0.tar` & `embyclient-4.8.4.0.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:48:22.695880 embyclient-4.8.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-15 07:48:22.695880 embyclient-4.8.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:48:22.635880 embyclient-4.8.3.0/embyclient/
--rw-r--r--   0 runner    (1001) docker     (127)    28759 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:48:22.695880 embyclient-4.8.3.0/embyclient/models/
--rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/access_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/actions_postback_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/activity_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/album_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/all_theme_media_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_available_recording_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_base_items_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_configuration_page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_epg_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_listing_provider_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_name_id_description_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_on_playback_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_set_channel_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_set_channel_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_set_channel_sort_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/api_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/artist_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/attributes_simple_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/attributes_value_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/authenticate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/authenticate_user_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/authentication_authentication_result.py
--rw-r--r--   0 runner    (1001) docker     (127)   126488 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/base_item_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/base_item_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/book_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/branding_branding_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/channel_management_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/chapter_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/codec_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/codec_directions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/codec_kinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/codec_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/codec_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/collections_collection_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/color_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/common_editor_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/common_interfaces_i_codec_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/common_plugins_i_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/conditions_property_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/conditions_property_condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/connect_connect_authentication_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/connect_user_link_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/connect_user_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/container_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/create_user_by_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/default_directory_browser_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/device_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/devices_content_upload_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/devices_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/devices_device_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/devices_local_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/direct_play_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/display_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dlna_profile_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dlna_profiles_device_identification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dlna_profiles_device_profile_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    37624 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dlna_profiles_dlna_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dlna_profiles_header_match_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dlna_profiles_http_header_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dlna_profiles_protocol_info_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/drawing_image_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/dynamic_day_of_week.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/edit_object_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/editors_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/editors_editor_button_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/editors_editor_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/encoding_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/enums_ui_command_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/enums_ui_view_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/extended_video_sub_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/extended_video_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/external_id_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/external_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/feature_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/feature_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/forgot_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/forgot_password_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/forgot_password_pin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/forgot_password_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/game_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/general_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/generic_edit_i_edit_object_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/get_directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/globalization_country_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/globalization_culture_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/globalization_localizaton_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/image_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/image_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/image_saving_convention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/installation_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/io_file_system_entry_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/io_file_system_entry_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/item_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/item_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/item_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/item_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/level_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_add_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_add_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_delete_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_item_link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_library_option_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_library_options_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_library_type_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_media_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_media_update_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    60338 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_post_updated_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_remove_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_remove_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_rename_virtual_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_sub_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_update_library_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_update_media_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/library_user_copy_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_stream_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_channel_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_guide_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_keep_until.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_keyword_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_keyword_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_listings_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_live_tv_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_recording_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    24601 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_series_timer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    36209 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_series_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_timer_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/live_tv_tuner_host_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/location_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/logging_log_severity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/marker_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/mb_backup_api_all_backups_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/mb_backup_api_data_restore_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/mb_backup_api_restore_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/mb_backup_api_user_restore_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/mb_backup_backup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_encoding_codec_parameter_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_path_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    39926 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_source_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    58923 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_stream_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/media_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/metadata_editor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/metadata_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/metadata_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/metadata_refresh_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/movie_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/music_video_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/name_id_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/name_long_id_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/name_value_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/net_end_point_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/net_sockets_address_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/notification_category_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/notification_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/package_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/package_target_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/package_version_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/package_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/parental_rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/path_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/persistence_intro_debug_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/person_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/person_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/pin_redeem_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/play_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/play_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/play_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playback_error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    19970 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playback_info_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playback_info_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    25054 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playback_progress_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playback_start_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playback_stop_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/player_state_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playlists_add_to_playlist_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playlists_playlist_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playstate_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/playstate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/plugins_configuration_page_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/plugins_plugin_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/process_run_metrics_process_metric_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/process_run_metrics_process_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/profile_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/profile_condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/profile_condition_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/profile_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/profile_level_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/progress_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/provider_id_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/proxy_header_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/public_system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_activity_log_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_api_epg_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_base_item_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_channel_management_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_devices_device_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_live_tv_timer_info_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_log_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_sync_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_sync_job_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_user_library_official_rating_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_user_library_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/query_result_virtual_folder_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/queue_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/rating_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/recommendation_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/recommendation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_image_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_album_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_artist_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_book_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_game_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_item_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_movie_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_music_video_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_person_lookup_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_series_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_query_trailer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_search_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/remote_subtitle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/repeat_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/resolution_with_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/response_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/roku_metadata_api_thumbnail_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/run_ui_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/secondary_frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/segment_skip_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/series_display_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/series_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    66420 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/server_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/session_session_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/session_user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/song_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sort_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/subtitle_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/subtitle_location_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/subtitle_playback_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/subtitle_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/subtitles_subtitle_download_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_data_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_data_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_dialog_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_job_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_job_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_job_item_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_job_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_profile_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_quality_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/sync_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/synced_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/synced_item_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/system_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/system_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/task_completion_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/task_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/task_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/task_trigger_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/theme_media_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/trailer_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/transcode_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/transcode_seek_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    29815 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/transcoding_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/transcoding_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/transcoding_vp_step_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/transcoding_vp_step_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/transport_stream_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/tuple_double_double.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/type_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/ui_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/ui_tab_page_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/ui_view_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/unrated_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/update_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_action_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_item_data_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_item_share_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_library_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_library_leave_shared_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_library_official_rating_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_library_remove_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_library_tag_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_library_update_user_item_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    13082 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_notification_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    45913 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/user_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/video3_d_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    22765 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/video_codec_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/video_media_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/virtual_folder_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/models/wake_on_lan_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/embyclient/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 07:48:22.695880 embyclient-4.8.3.0/embyclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-15 07:48:22.000000 embyclient-4.8.3.0/embyclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-03-15 07:48:22.000000 embyclient-4.8.3.0/embyclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 07:48:22.000000 embyclient-4.8.3.0/embyclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-15 07:48:22.000000 embyclient-4.8.3.0/embyclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 07:48:22.000000 embyclient-4.8.3.0/embyclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 07:48:22.695880 embyclient-4.8.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-15 07:48:16.000000 embyclient-4.8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:16:42.255389 embyclient-4.8.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-19 00:16:42.255389 embyclient-4.8.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:16:42.195389 embyclient-4.8.4.0/embyclient/
+-rw-r--r--   0 runner    (1001) docker     (127)    28759 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24584 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:16:42.255389 embyclient-4.8.4.0/embyclient/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    22941 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/access_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/actions_postback_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/activity_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/album_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/all_theme_media_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_available_recording_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_base_items_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_configuration_page_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_epg_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_listing_provider_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_name_id_description_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_on_playback_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_set_channel_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_set_channel_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_set_channel_sort_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/api_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/artist_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/attributes_simple_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/attributes_value_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/authenticate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/authenticate_user_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/authentication_authentication_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126488 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/base_item_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/base_item_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/book_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/branding_branding_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/channel_management_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/chapter_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/codec_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/codec_directions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/codec_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/codec_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/codec_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/collections_collection_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/color_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/common_editor_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/common_interfaces_i_codec_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/common_plugins_i_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/conditions_property_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/conditions_property_condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/connect_connect_authentication_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/connect_user_link_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/connect_user_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/container_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/create_user_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/default_directory_browser_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13068 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/device_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/devices_content_upload_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/devices_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/devices_device_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/devices_local_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/direct_play_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/display_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dlna_profile_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dlna_profiles_device_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dlna_profiles_device_profile_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37624 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dlna_profiles_dlna_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dlna_profiles_header_match_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dlna_profiles_http_header_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dlna_profiles_protocol_info_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/drawing_image_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/dynamic_day_of_week.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/edit_object_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/editors_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/editors_editor_button_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/editors_editor_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/encoding_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/enums_ui_command_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/enums_ui_view_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/extended_video_sub_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/extended_video_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/external_id_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/external_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/feature_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/forgot_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/forgot_password_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/forgot_password_pin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/forgot_password_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/game_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/general_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/generic_edit_i_edit_object_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/get_directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/globalization_country_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/globalization_culture_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/globalization_localizaton_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/image_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/image_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/image_saving_convention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/installation_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/io_file_system_entry_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/io_file_system_entry_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13371 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/item_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/item_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/item_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/item_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/level_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_add_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_add_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_delete_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_item_link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_library_option_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_library_options_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_library_type_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_media_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_media_update_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60338 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_post_updated_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_remove_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_remove_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_rename_virtual_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_sub_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_update_library_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_update_media_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/library_user_copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_stream_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_channel_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_guide_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_keep_until.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_keyword_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_keyword_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18555 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_listings_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_live_tv_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_recording_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_series_timer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_series_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24849 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_timer_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/live_tv_tuner_host_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/location_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/logging_log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/marker_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/mb_backup_api_all_backups_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/mb_backup_api_data_restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/mb_backup_api_restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/mb_backup_api_user_restore_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/mb_backup_backup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_encoding_codec_parameter_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39926 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_source_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58923 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_stream_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/media_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/metadata_editor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/metadata_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/metadata_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/metadata_refresh_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/music_video_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/name_id_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/name_long_id_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/name_value_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/net_end_point_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/net_sockets_address_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/notification_category_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/notification_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/package_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/package_target_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/package_version_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/package_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/parental_rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/path_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/persistence_intro_debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/person_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/person_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/pin_redeem_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/play_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/play_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/play_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playback_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19970 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playback_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playback_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25054 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playback_progress_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playback_start_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playback_stop_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/player_state_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playlists_add_to_playlist_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playlists_playlist_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playstate_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/playstate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/plugins_configuration_page_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/plugins_plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/process_run_metrics_process_metric_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/process_run_metrics_process_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/profile_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/profile_condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/profile_condition_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/profile_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/profile_level_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/progress_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/provider_id_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/proxy_header_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/public_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_activity_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_api_epg_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_base_item_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_channel_management_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_devices_device_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_live_tv_timer_info_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_log_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_sync_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_sync_job_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_user_library_official_rating_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_user_library_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/query_result_virtual_folder_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/queue_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/rating_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/recommendation_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/recommendation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10630 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_image_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_album_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_artist_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_book_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_game_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_item_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_music_video_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_person_lookup_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_series_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_query_trailer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/remote_subtitle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/repeat_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/resolution_with_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/response_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/roku_metadata_api_thumbnail_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/run_ui_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/secondary_frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/segment_skip_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/series_display_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/series_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66420 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/server_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23279 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/session_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/session_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13666 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/song_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sort_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/subtitle_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/subtitle_location_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/subtitle_playback_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/subtitle_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/subtitles_subtitle_download_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_dialog_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_job_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_job_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_job_item_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_job_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_profile_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_quality_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/sync_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/synced_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/synced_item_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/system_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34832 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/task_completion_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/task_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/task_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/task_trigger_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/theme_media_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/trailer_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/transcode_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/transcode_seek_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29815 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/transcoding_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19145 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/transcoding_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/transcoding_vp_step_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/transcoding_vp_step_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/transport_stream_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/tuple_double_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/type_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/ui_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/ui_tab_page_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/ui_view_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/unrated_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/update_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19873 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18187 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_item_data_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_item_share_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_library_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_library_leave_shared_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_library_official_rating_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_library_remove_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_library_tag_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_library_update_user_item_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_notification_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45913 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/user_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/video3_d_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22765 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/video_codec_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/video_media_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/virtual_folder_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/models/wake_on_lan_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/embyclient/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:16:42.255389 embyclient-4.8.4.0/embyclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-19 00:16:42.000000 embyclient-4.8.4.0/embyclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-04-19 00:16:42.000000 embyclient-4.8.4.0/embyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:16:42.000000 embyclient-4.8.4.0/embyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 00:16:42.000000 embyclient-4.8.4.0/embyclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 00:16:42.000000 embyclient-4.8.4.0/embyclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:16:42.255389 embyclient-4.8.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-19 00:16:35.000000 embyclient-4.8.4.0/setup.py
```

### Comparing `embyclient-4.8.3.0/README.md` & `embyclient-4.8.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,60 @@
-# Python Client
+# Emby Python Client
 
-<table><tr />
-    <tr>
-        <th valign="top" align="left">Name</th>
-        <td>embyclient</td>
-    </tr>
-    <tr>
-        <th valign="top" align="left">Language</th>
-        <td>Python</td>
-    </tr>
-    <tr>
-        <th valign="top" align="left">SDK Folder</th>
-        <td>SampleCode/RestApi/Clients/Python</td>
-    </tr>
-</table>
+A Python client for Emby Media Server's API. 
 
-## Requirements.
+**NOTE**: The [original source code](https://github.com/MediaBrowser/Emby.SDK/tree/master/SampleCode/RestApi/Clients/Python) for this client is auto-generated by Emby's OpenAPI spec.
+This specific client is an automated release of the source code with some minor modifications.
+Any bugs or issues with the client should be reported to the [Emby SDK repository](https://github.com/MediaBrowser/Emby.SDK)
 
-Python 2.7 and 3.4+
+## Python Version Support
 
-## Installation & Usage
-### Setuptools
+Python 2.7 (deprecated) or 3.4+
 
-Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
+## Installation
+
+Install via [pip](https://pypi.org/project/embyclient/):
 
 ```sh
-python setup.py install --user
+pip install embyclient
 ```
-(or `sudo python setup.py install` to install the package for all users)
 
-Then import the package:
+## Usage
+
+Import the package:
+
 ```python
 import embyclient
 ```
 
-## Getting Started
-
-Please follow the [installation procedure](#installation--usage) and then run the following:
+Configure a client instance:
 
 ```python
-from __future__ import print_function
-import time
 import embyclient
 from embyclient.rest import ApiException
-from pprint import pprint
 
 # Configure API key authorization: apikeyauth
 configuration = embyclient.Configuration()
 configuration.api_key['api_key'] = 'YOUR_API_KEY'
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['api_key'] = 'Bearer'
 
 # create an instance of the API class
-api_instance = embyclient.ActivityLogServiceApi(embyclient.ApiClient(configuration))
-start_index = 56 # int | Optional. The record index to start at. All items with a lower index will be dropped from the results. (optional)
-limit = 56 # int | Optional. The maximum number of records to return (optional)
-min_date = 'min_date_example' # str | Optional. The minimum date. Format = ISO (optional)
+client = embyclient.ApiClient(configuration)
+```
+
+Then use the client to interact via specific API services:
+
+```python
+activity_log_service = embyclient.ActivityLogServiceApi(client)
 
 try:
     # Gets activity log entries
-    api_response = api_instance.get_system_activitylog_entries(start_index=start_index, limit=limit, min_date=min_date)
-    pprint(api_response)
+    api_response = activity_log_service.get_activity_log_entries(start_index=56, limit=56, min_date='min_date_example')
+    print(api_response)
 except ApiException as e:
-    print("Exception when calling ActivityLogServiceApi->get_system_activitylog_entries: %s\n" % e)
+    print("Exception when calling ActivityLogServiceApi->get_activity_log_entries: %s\n" % e)
 ```
+
+## Documentation
+
+For more information, please visit [Emby's API documentation](https://swagger.emby.media/?staticview=true).
```

### Comparing `embyclient-4.8.3.0/embyclient/__init__.py` & `embyclient-4.8.4.0/embyclient/__init__.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/api_client.py` & `embyclient-4.8.4.0/embyclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = '/4.8.3.0/python'
+        self.user_agent = '/4.8.4.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `embyclient-4.8.3.0/embyclient/configuration.py` & `embyclient-4.8.4.0/embyclient/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,10 +234,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.8.3.0\n"\
-               "SDK Package Version: 4.8.3.0".\
+               "Version of the API: 4.8.4.0\n"\
+               "SDK Package Version: 4.8.4.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `embyclient-4.8.3.0/embyclient/models/__init__.py` & `embyclient-4.8.4.0/embyclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/access_schedule.py` & `embyclient-4.8.4.0/embyclient/models/access_schedule.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/actions_postback_action.py` & `embyclient-4.8.4.0/embyclient/models/actions_postback_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/activity_log_entry.py` & `embyclient-4.8.4.0/embyclient/models/activity_log_entry.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/album_info.py` & `embyclient-4.8.4.0/embyclient/models/album_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/all_theme_media_result.py` & `embyclient-4.8.4.0/embyclient/models/all_theme_media_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_available_recording_options.py` & `embyclient-4.8.4.0/embyclient/models/api_available_recording_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_base_items_request.py` & `embyclient-4.8.4.0/embyclient/models/api_base_items_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_configuration_page_info.py` & `embyclient-4.8.4.0/embyclient/models/api_configuration_page_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_epg_row.py` & `embyclient-4.8.4.0/embyclient/models/api_epg_row.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_listing_provider_type_info.py` & `embyclient-4.8.4.0/embyclient/models/api_listing_provider_type_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_name_id_description_pair.py` & `embyclient-4.8.4.0/embyclient/models/api_name_id_description_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_on_playback_progress.py` & `embyclient-4.8.4.0/embyclient/models/api_on_playback_progress.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_set_channel_disabled.py` & `embyclient-4.8.4.0/embyclient/models/api_set_channel_disabled.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_set_channel_mapping.py` & `embyclient-4.8.4.0/embyclient/models/api_set_channel_mapping.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_set_channel_sort_index.py` & `embyclient-4.8.4.0/embyclient/models/api_set_channel_sort_index.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/api_tag_item.py` & `embyclient-4.8.4.0/embyclient/models/api_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/artist_info.py` & `embyclient-4.8.4.0/embyclient/models/artist_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/attributes_simple_condition.py` & `embyclient-4.8.4.0/embyclient/models/attributes_simple_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/attributes_value_condition.py` & `embyclient-4.8.4.0/embyclient/models/attributes_value_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/authenticate_user.py` & `embyclient-4.8.4.0/embyclient/models/authenticate_user.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/authenticate_user_by_name.py` & `embyclient-4.8.4.0/embyclient/models/authenticate_user_by_name.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/authentication_authentication_result.py` & `embyclient-4.8.4.0/embyclient/models/authentication_authentication_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/base_item_dto.py` & `embyclient-4.8.4.0/embyclient/models/base_item_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/base_item_person.py` & `embyclient-4.8.4.0/embyclient/models/base_item_person.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/bit_rate.py` & `embyclient-4.8.4.0/embyclient/models/bit_rate.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/book_info.py` & `embyclient-4.8.4.0/embyclient/models/book_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/branding_branding_options.py` & `embyclient-4.8.4.0/embyclient/models/branding_branding_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/channel_management_info.py` & `embyclient-4.8.4.0/embyclient/models/channel_management_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/chapter_info.py` & `embyclient-4.8.4.0/embyclient/models/chapter_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/client_capabilities.py` & `embyclient-4.8.4.0/embyclient/models/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/codec_configuration.py` & `embyclient-4.8.4.0/embyclient/models/codec_configuration.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/codec_directions.py` & `embyclient-4.8.4.0/embyclient/models/codec_directions.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/codec_kinds.py` & `embyclient-4.8.4.0/embyclient/models/codec_kinds.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/codec_profile.py` & `embyclient-4.8.4.0/embyclient/models/codec_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/codec_type.py` & `embyclient-4.8.4.0/embyclient/models/codec_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/collections_collection_creation_result.py` & `embyclient-4.8.4.0/embyclient/models/collections_collection_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/color_formats.py` & `embyclient-4.8.4.0/embyclient/models/color_formats.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/common_editor_types.py` & `embyclient-4.8.4.0/embyclient/models/common_editor_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py` & `embyclient-4.8.4.0/embyclient/models/common_interfaces_i_codec_device_capabilities.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/common_interfaces_i_codec_device_info.py` & `embyclient-4.8.4.0/embyclient/models/common_interfaces_i_codec_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/common_plugins_i_plugin.py` & `embyclient-4.8.4.0/embyclient/models/common_plugins_i_plugin.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/conditions_property_condition.py` & `embyclient-4.8.4.0/embyclient/models/conditions_property_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/conditions_property_condition_type.py` & `embyclient-4.8.4.0/embyclient/models/conditions_property_condition_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py` & `embyclient-4.8.4.0/embyclient/models/configuration_tone_mapping_tone_map_options_visibility.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/connect_connect_authentication_exchange_result.py` & `embyclient-4.8.4.0/embyclient/models/connect_connect_authentication_exchange_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/connect_user_link_result.py` & `embyclient-4.8.4.0/embyclient/models/connect_user_link_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/connect_user_link_type.py` & `embyclient-4.8.4.0/embyclient/models/connect_user_link_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/container_profile.py` & `embyclient-4.8.4.0/embyclient/models/container_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/create_user_by_name.py` & `embyclient-4.8.4.0/embyclient/models/create_user_by_name.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/day_of_week.py` & `embyclient-4.8.4.0/embyclient/models/day_of_week.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/default_directory_browser_info.py` & `embyclient-4.8.4.0/embyclient/models/default_directory_browser_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/device_profile.py` & `embyclient-4.8.4.0/embyclient/models/device_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/devices_content_upload_history.py` & `embyclient-4.8.4.0/embyclient/models/devices_content_upload_history.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/devices_device_info.py` & `embyclient-4.8.4.0/embyclient/models/devices_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/devices_device_options.py` & `embyclient-4.8.4.0/embyclient/models/devices_device_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/devices_local_file_info.py` & `embyclient-4.8.4.0/embyclient/models/devices_local_file_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/direct_play_profile.py` & `embyclient-4.8.4.0/embyclient/models/direct_play_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/display_preferences.py` & `embyclient-4.8.4.0/embyclient/models/display_preferences.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dlna_profile_type.py` & `embyclient-4.8.4.0/embyclient/models/dlna_profile_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dlna_profiles_device_identification.py` & `embyclient-4.8.4.0/embyclient/models/dlna_profiles_device_identification.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dlna_profiles_device_profile_type.py` & `embyclient-4.8.4.0/embyclient/models/dlna_profiles_device_profile_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dlna_profiles_dlna_profile.py` & `embyclient-4.8.4.0/embyclient/models/dlna_profiles_dlna_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dlna_profiles_header_match_type.py` & `embyclient-4.8.4.0/embyclient/models/dlna_profiles_header_match_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dlna_profiles_http_header_info.py` & `embyclient-4.8.4.0/embyclient/models/dlna_profiles_http_header_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dlna_profiles_protocol_info_detection.py` & `embyclient-4.8.4.0/embyclient/models/dlna_profiles_protocol_info_detection.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/drawing_image_orientation.py` & `embyclient-4.8.4.0/embyclient/models/drawing_image_orientation.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/dynamic_day_of_week.py` & `embyclient-4.8.4.0/embyclient/models/dynamic_day_of_week.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/edit_object_container.py` & `embyclient-4.8.4.0/embyclient/models/edit_object_container.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/editors_editor_base.py` & `embyclient-4.8.4.0/embyclient/models/editors_editor_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,39 +26,42 @@
         'name': 'str',
         'id': 'str',
         'allow_empty': 'bool',
         'is_read_only': 'bool',
         'is_advanced': 'bool',
         'display_name': 'str',
         'description': 'str',
+        'feature_requires_premiere': 'bool',
         'parent_id': 'str'
     }
 
     attribute_map = {
         'editor_type': 'EditorType',
         'name': 'Name',
         'id': 'Id',
         'allow_empty': 'AllowEmpty',
         'is_read_only': 'IsReadOnly',
         'is_advanced': 'IsAdvanced',
         'display_name': 'DisplayName',
         'description': 'Description',
+        'feature_requires_premiere': 'FeatureRequiresPremiere',
         'parent_id': 'ParentId'
     }
 
-    def __init__(self, editor_type=None, name=None, id=None, allow_empty=None, is_read_only=None, is_advanced=None, display_name=None, description=None, parent_id=None):  # noqa: E501
+    def __init__(self, editor_type=None, name=None, id=None, allow_empty=None, is_read_only=None, is_advanced=None, display_name=None, description=None, feature_requires_premiere=None, parent_id=None):  # noqa: E501
         """EditorsEditorBase - a model defined in Swagger"""  # noqa: E501
         self._editor_type = None
         self._name = None
         self._id = None
         self._allow_empty = None
         self._is_read_only = None
         self._is_advanced = None
         self._display_name = None
         self._description = None
+        self._feature_requires_premiere = None
         self._parent_id = None
         self.discriminator = None
         if editor_type is not None:
             self.editor_type = editor_type
         if name is not None:
             self.name = name
         if id is not None:
@@ -69,14 +72,16 @@
             self.is_read_only = is_read_only
         if is_advanced is not None:
             self.is_advanced = is_advanced
         if display_name is not None:
             self.display_name = display_name
         if description is not None:
             self.description = description
+        if feature_requires_premiere is not None:
+            self.feature_requires_premiere = feature_requires_premiere
         if parent_id is not None:
             self.parent_id = parent_id
 
     @property
     def editor_type(self):
         """Gets the editor_type of this EditorsEditorBase.  # noqa: E501
 
@@ -241,14 +246,35 @@
         :param description: The description of this EditorsEditorBase.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
+    def feature_requires_premiere(self):
+        """Gets the feature_requires_premiere of this EditorsEditorBase.  # noqa: E501
+
+
+        :return: The feature_requires_premiere of this EditorsEditorBase.  # noqa: E501
+        :rtype: bool
+        """
+        return self._feature_requires_premiere
+
+    @feature_requires_premiere.setter
+    def feature_requires_premiere(self, feature_requires_premiere):
+        """Sets the feature_requires_premiere of this EditorsEditorBase.
+
+
+        :param feature_requires_premiere: The feature_requires_premiere of this EditorsEditorBase.  # noqa: E501
+        :type: bool
+        """
+
+        self._feature_requires_premiere = feature_requires_premiere
+
+    @property
     def parent_id(self):
         """Gets the parent_id of this EditorsEditorBase.  # noqa: E501
 
 
         :return: The parent_id of this EditorsEditorBase.  # noqa: E501
         :rtype: str
         """
```

### Comparing `embyclient-4.8.3.0/embyclient/models/editors_editor_button_item.py` & `embyclient-4.8.4.0/embyclient/models/editors_editor_button_item.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,39 +26,42 @@
         'name': 'str',
         'id': 'str',
         'allow_empty': 'bool',
         'is_read_only': 'bool',
         'is_advanced': 'bool',
         'display_name': 'str',
         'description': 'str',
+        'feature_requires_premiere': 'bool',
         'parent_id': 'str'
     }
 
     attribute_map = {
         'editor_type': 'EditorType',
         'name': 'Name',
         'id': 'Id',
         'allow_empty': 'AllowEmpty',
         'is_read_only': 'IsReadOnly',
         'is_advanced': 'IsAdvanced',
         'display_name': 'DisplayName',
         'description': 'Description',
+        'feature_requires_premiere': 'FeatureRequiresPremiere',
         'parent_id': 'ParentId'
     }
 
-    def __init__(self, editor_type=None, name=None, id=None, allow_empty=None, is_read_only=None, is_advanced=None, display_name=None, description=None, parent_id=None):  # noqa: E501
+    def __init__(self, editor_type=None, name=None, id=None, allow_empty=None, is_read_only=None, is_advanced=None, display_name=None, description=None, feature_requires_premiere=None, parent_id=None):  # noqa: E501
         """EditorsEditorButtonItem - a model defined in Swagger"""  # noqa: E501
         self._editor_type = None
         self._name = None
         self._id = None
         self._allow_empty = None
         self._is_read_only = None
         self._is_advanced = None
         self._display_name = None
         self._description = None
+        self._feature_requires_premiere = None
         self._parent_id = None
         self.discriminator = None
         if editor_type is not None:
             self.editor_type = editor_type
         if name is not None:
             self.name = name
         if id is not None:
@@ -69,14 +72,16 @@
             self.is_read_only = is_read_only
         if is_advanced is not None:
             self.is_advanced = is_advanced
         if display_name is not None:
             self.display_name = display_name
         if description is not None:
             self.description = description
+        if feature_requires_premiere is not None:
+            self.feature_requires_premiere = feature_requires_premiere
         if parent_id is not None:
             self.parent_id = parent_id
 
     @property
     def editor_type(self):
         """Gets the editor_type of this EditorsEditorButtonItem.  # noqa: E501
 
@@ -241,14 +246,35 @@
         :param description: The description of this EditorsEditorButtonItem.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
+    def feature_requires_premiere(self):
+        """Gets the feature_requires_premiere of this EditorsEditorButtonItem.  # noqa: E501
+
+
+        :return: The feature_requires_premiere of this EditorsEditorButtonItem.  # noqa: E501
+        :rtype: bool
+        """
+        return self._feature_requires_premiere
+
+    @feature_requires_premiere.setter
+    def feature_requires_premiere(self, feature_requires_premiere):
+        """Sets the feature_requires_premiere of this EditorsEditorButtonItem.
+
+
+        :param feature_requires_premiere: The feature_requires_premiere of this EditorsEditorButtonItem.  # noqa: E501
+        :type: bool
+        """
+
+        self._feature_requires_premiere = feature_requires_premiere
+
+    @property
     def parent_id(self):
         """Gets the parent_id of this EditorsEditorButtonItem.  # noqa: E501
 
 
         :return: The parent_id of this EditorsEditorButtonItem.  # noqa: E501
         :rtype: str
         """
```

### Comparing `embyclient-4.8.3.0/embyclient/models/editors_editor_root.py` & `embyclient-4.8.4.0/embyclient/models/editors_editor_root.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         'name': 'str',
         'id': 'str',
         'allow_empty': 'bool',
         'is_read_only': 'bool',
         'is_advanced': 'bool',
         'display_name': 'str',
         'description': 'str',
+        'feature_requires_premiere': 'bool',
         'parent_id': 'str'
     }
 
     attribute_map = {
         'property_conditions': 'PropertyConditions',
         'postback_actions': 'PostbackActions',
         'title_button': 'TitleButton',
@@ -46,31 +47,33 @@
         'name': 'Name',
         'id': 'Id',
         'allow_empty': 'AllowEmpty',
         'is_read_only': 'IsReadOnly',
         'is_advanced': 'IsAdvanced',
         'display_name': 'DisplayName',
         'description': 'Description',
+        'feature_requires_premiere': 'FeatureRequiresPremiere',
         'parent_id': 'ParentId'
     }
 
-    def __init__(self, property_conditions=None, postback_actions=None, title_button=None, editor_items=None, editor_type=None, name=None, id=None, allow_empty=None, is_read_only=None, is_advanced=None, display_name=None, description=None, parent_id=None):  # noqa: E501
+    def __init__(self, property_conditions=None, postback_actions=None, title_button=None, editor_items=None, editor_type=None, name=None, id=None, allow_empty=None, is_read_only=None, is_advanced=None, display_name=None, description=None, feature_requires_premiere=None, parent_id=None):  # noqa: E501
         """EditorsEditorRoot - a model defined in Swagger"""  # noqa: E501
         self._property_conditions = None
         self._postback_actions = None
         self._title_button = None
         self._editor_items = None
         self._editor_type = None
         self._name = None
         self._id = None
         self._allow_empty = None
         self._is_read_only = None
         self._is_advanced = None
         self._display_name = None
         self._description = None
+        self._feature_requires_premiere = None
         self._parent_id = None
         self.discriminator = None
         if property_conditions is not None:
             self.property_conditions = property_conditions
         if postback_actions is not None:
             self.postback_actions = postback_actions
         if title_button is not None:
@@ -89,14 +92,16 @@
             self.is_read_only = is_read_only
         if is_advanced is not None:
             self.is_advanced = is_advanced
         if display_name is not None:
             self.display_name = display_name
         if description is not None:
             self.description = description
+        if feature_requires_premiere is not None:
+            self.feature_requires_premiere = feature_requires_premiere
         if parent_id is not None:
             self.parent_id = parent_id
 
     @property
     def property_conditions(self):
         """Gets the property_conditions of this EditorsEditorRoot.  # noqa: E501
 
@@ -345,14 +350,35 @@
         :param description: The description of this EditorsEditorRoot.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
+    def feature_requires_premiere(self):
+        """Gets the feature_requires_premiere of this EditorsEditorRoot.  # noqa: E501
+
+
+        :return: The feature_requires_premiere of this EditorsEditorRoot.  # noqa: E501
+        :rtype: bool
+        """
+        return self._feature_requires_premiere
+
+    @feature_requires_premiere.setter
+    def feature_requires_premiere(self, feature_requires_premiere):
+        """Sets the feature_requires_premiere of this EditorsEditorRoot.
+
+
+        :param feature_requires_premiere: The feature_requires_premiere of this EditorsEditorRoot.  # noqa: E501
+        :type: bool
+        """
+
+        self._feature_requires_premiere = feature_requires_premiere
+
+    @property
     def parent_id(self):
         """Gets the parent_id of this EditorsEditorRoot.  # noqa: E501
 
 
         :return: The parent_id of this EditorsEditorRoot.  # noqa: E501
         :rtype: str
         """
```

### Comparing `embyclient-4.8.3.0/embyclient/models/encoding_context.py` & `embyclient-4.8.4.0/embyclient/models/encoding_context.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/enums_ui_command_type.py` & `embyclient-4.8.4.0/embyclient/models/enums_ui_command_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/enums_ui_view_type.py` & `embyclient-4.8.4.0/embyclient/models/enums_ui_view_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/extended_video_sub_types.py` & `embyclient-4.8.4.0/embyclient/models/extended_video_sub_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/extended_video_types.py` & `embyclient-4.8.4.0/embyclient/models/extended_video_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/external_id_info.py` & `embyclient-4.8.4.0/embyclient/models/external_id_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/external_url.py` & `embyclient-4.8.4.0/embyclient/models/external_url.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/feature_info.py` & `embyclient-4.8.4.0/embyclient/models/feature_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/feature_type.py` & `embyclient-4.8.4.0/embyclient/models/feature_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/forgot_password.py` & `embyclient-4.8.4.0/embyclient/models/forgot_password.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/forgot_password_action.py` & `embyclient-4.8.4.0/embyclient/models/forgot_password_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/forgot_password_pin.py` & `embyclient-4.8.4.0/embyclient/models/forgot_password_pin.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/forgot_password_result.py` & `embyclient-4.8.4.0/embyclient/models/forgot_password_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/game_info.py` & `embyclient-4.8.4.0/embyclient/models/game_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/general_command.py` & `embyclient-4.8.4.0/embyclient/models/general_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/generic_edit_i_edit_object_container.py` & `embyclient-4.8.4.0/embyclient/models/generic_edit_i_edit_object_container.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/get_directory_contents.py` & `embyclient-4.8.4.0/embyclient/models/get_directory_contents.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/globalization_country_info.py` & `embyclient-4.8.4.0/embyclient/models/globalization_country_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/globalization_culture_dto.py` & `embyclient-4.8.4.0/embyclient/models/globalization_culture_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/globalization_localizaton_option.py` & `embyclient-4.8.4.0/embyclient/models/globalization_localizaton_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/image_info.py` & `embyclient-4.8.4.0/embyclient/models/image_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/image_option.py` & `embyclient-4.8.4.0/embyclient/models/image_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/image_provider_info.py` & `embyclient-4.8.4.0/embyclient/models/image_provider_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/image_saving_convention.py` & `embyclient-4.8.4.0/embyclient/models/image_saving_convention.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/image_type.py` & `embyclient-4.8.4.0/embyclient/models/image_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/installation_info.py` & `embyclient-4.8.4.0/embyclient/models/installation_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/io_file_system_entry_info.py` & `embyclient-4.8.4.0/embyclient/models/io_file_system_entry_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/io_file_system_entry_type.py` & `embyclient-4.8.4.0/embyclient/models/io_file_system_entry_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/item_counts.py` & `embyclient-4.8.4.0/embyclient/models/item_counts.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/item_file_info.py` & `embyclient-4.8.4.0/embyclient/models/item_file_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/item_file_type.py` & `embyclient-4.8.4.0/embyclient/models/item_file_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/item_lookup_info.py` & `embyclient-4.8.4.0/embyclient/models/item_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/level_information.py` & `embyclient-4.8.4.0/embyclient/models/level_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_add_media_path.py` & `embyclient-4.8.4.0/embyclient/models/library_add_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_add_virtual_folder.py` & `embyclient-4.8.4.0/embyclient/models/library_add_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_delete_info.py` & `embyclient-4.8.4.0/embyclient/models/library_delete_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_item_link_type.py` & `embyclient-4.8.4.0/embyclient/models/library_item_link_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_library_option_info.py` & `embyclient-4.8.4.0/embyclient/models/library_library_option_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_library_options_result.py` & `embyclient-4.8.4.0/embyclient/models/library_library_options_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_library_type_options.py` & `embyclient-4.8.4.0/embyclient/models/library_library_type_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_media_folder.py` & `embyclient-4.8.4.0/embyclient/models/library_media_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_media_update_info.py` & `embyclient-4.8.4.0/embyclient/models/library_media_update_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_options.py` & `embyclient-4.8.4.0/embyclient/models/library_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_post_updated_media.py` & `embyclient-4.8.4.0/embyclient/models/library_post_updated_media.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_remove_media_path.py` & `embyclient-4.8.4.0/embyclient/models/library_remove_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_remove_virtual_folder.py` & `embyclient-4.8.4.0/embyclient/models/library_remove_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_rename_virtual_folder.py` & `embyclient-4.8.4.0/embyclient/models/library_rename_virtual_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_sub_folder.py` & `embyclient-4.8.4.0/embyclient/models/library_sub_folder.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_update_library_options.py` & `embyclient-4.8.4.0/embyclient/models/library_update_library_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_update_media_path.py` & `embyclient-4.8.4.0/embyclient/models/library_update_media_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/library_user_copy_options.py` & `embyclient-4.8.4.0/embyclient/models/library_user_copy_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_stream_request.py` & `embyclient-4.8.4.0/embyclient/models/live_stream_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_stream_response.py` & `embyclient-4.8.4.0/embyclient/models/live_stream_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_channel_type.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_channel_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_guide_info.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_guide_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_keep_until.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_keep_until.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_keyword_info.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_keyword_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_keyword_type.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_keyword_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_listings_provider_info.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_listings_provider_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_live_tv_info.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_live_tv_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_recording_status.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_recording_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_series_timer_info.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_series_timer_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         'overview': 'str',
         'start_date': 'datetime',
         'end_date': 'datetime',
         'record_any_time': 'bool',
         'keep_up_to': 'int',
         'keep_until': 'LiveTvKeepUntil',
         'skip_episodes_in_library': 'bool',
+        'match_existing_items_with_any_library': 'bool',
         'record_new_only': 'bool',
         'days': 'list[DayOfWeek]',
         'priority': 'int',
         'pre_padding_seconds': 'int',
         'post_padding_seconds': 'int',
         'is_pre_padding_required': 'bool',
         'is_post_padding_required': 'bool',
@@ -61,29 +62,30 @@
         'overview': 'Overview',
         'start_date': 'StartDate',
         'end_date': 'EndDate',
         'record_any_time': 'RecordAnyTime',
         'keep_up_to': 'KeepUpTo',
         'keep_until': 'KeepUntil',
         'skip_episodes_in_library': 'SkipEpisodesInLibrary',
+        'match_existing_items_with_any_library': 'MatchExistingItemsWithAnyLibrary',
         'record_new_only': 'RecordNewOnly',
         'days': 'Days',
         'priority': 'Priority',
         'pre_padding_seconds': 'PrePaddingSeconds',
         'post_padding_seconds': 'PostPaddingSeconds',
         'is_pre_padding_required': 'IsPrePaddingRequired',
         'is_post_padding_required': 'IsPostPaddingRequired',
         'series_id': 'SeriesId',
         'provider_ids': 'ProviderIds',
         'max_recording_seconds': 'MaxRecordingSeconds',
         'keywords': 'Keywords',
         'timer_type': 'TimerType'
     }
 
-    def __init__(self, id=None, channel_id=None, channel_ids=None, parent_folder_id=None, program_id=None, name=None, service_name=None, overview=None, start_date=None, end_date=None, record_any_time=None, keep_up_to=None, keep_until=None, skip_episodes_in_library=None, record_new_only=None, days=None, priority=None, pre_padding_seconds=None, post_padding_seconds=None, is_pre_padding_required=None, is_post_padding_required=None, series_id=None, provider_ids=None, max_recording_seconds=None, keywords=None, timer_type=None):  # noqa: E501
+    def __init__(self, id=None, channel_id=None, channel_ids=None, parent_folder_id=None, program_id=None, name=None, service_name=None, overview=None, start_date=None, end_date=None, record_any_time=None, keep_up_to=None, keep_until=None, skip_episodes_in_library=None, match_existing_items_with_any_library=None, record_new_only=None, days=None, priority=None, pre_padding_seconds=None, post_padding_seconds=None, is_pre_padding_required=None, is_post_padding_required=None, series_id=None, provider_ids=None, max_recording_seconds=None, keywords=None, timer_type=None):  # noqa: E501
         """LiveTvSeriesTimerInfo - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._channel_id = None
         self._channel_ids = None
         self._parent_folder_id = None
         self._program_id = None
         self._name = None
@@ -91,14 +93,15 @@
         self._overview = None
         self._start_date = None
         self._end_date = None
         self._record_any_time = None
         self._keep_up_to = None
         self._keep_until = None
         self._skip_episodes_in_library = None
+        self._match_existing_items_with_any_library = None
         self._record_new_only = None
         self._days = None
         self._priority = None
         self._pre_padding_seconds = None
         self._post_padding_seconds = None
         self._is_pre_padding_required = None
         self._is_post_padding_required = None
@@ -132,14 +135,16 @@
             self.record_any_time = record_any_time
         if keep_up_to is not None:
             self.keep_up_to = keep_up_to
         if keep_until is not None:
             self.keep_until = keep_until
         if skip_episodes_in_library is not None:
             self.skip_episodes_in_library = skip_episodes_in_library
+        if match_existing_items_with_any_library is not None:
+            self.match_existing_items_with_any_library = match_existing_items_with_any_library
         if record_new_only is not None:
             self.record_new_only = record_new_only
         if days is not None:
             self.days = days
         if priority is not None:
             self.priority = priority
         if pre_padding_seconds is not None:
@@ -468,14 +473,35 @@
         :param skip_episodes_in_library: The skip_episodes_in_library of this LiveTvSeriesTimerInfo.  # noqa: E501
         :type: bool
         """
 
         self._skip_episodes_in_library = skip_episodes_in_library
 
     @property
+    def match_existing_items_with_any_library(self):
+        """Gets the match_existing_items_with_any_library of this LiveTvSeriesTimerInfo.  # noqa: E501
+
+
+        :return: The match_existing_items_with_any_library of this LiveTvSeriesTimerInfo.  # noqa: E501
+        :rtype: bool
+        """
+        return self._match_existing_items_with_any_library
+
+    @match_existing_items_with_any_library.setter
+    def match_existing_items_with_any_library(self, match_existing_items_with_any_library):
+        """Sets the match_existing_items_with_any_library of this LiveTvSeriesTimerInfo.
+
+
+        :param match_existing_items_with_any_library: The match_existing_items_with_any_library of this LiveTvSeriesTimerInfo.  # noqa: E501
+        :type: bool
+        """
+
+        self._match_existing_items_with_any_library = match_existing_items_with_any_library
+
+    @property
     def record_new_only(self):
         """Gets the record_new_only of this LiveTvSeriesTimerInfo.  # noqa: E501
 
         A value indicating whether \\[record new only\\].  # noqa: E501
 
         :return: The record_new_only of this LiveTvSeriesTimerInfo.  # noqa: E501
         :rtype: bool
```

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_series_timer_info_dto.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_series_timer_info_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'record_any_time': 'bool',
         'skip_episodes_in_library': 'bool',
+        'match_existing_items_with_any_library': 'bool',
         'record_any_channel': 'bool',
         'keep_up_to': 'int',
         'max_recording_seconds': 'int',
         'record_new_only': 'bool',
         'channel_ids': 'list[str]',
         'days': 'list[DayOfWeek]',
         'image_tags': 'dict(str, str)',
@@ -60,14 +61,15 @@
         'is_post_padding_required': 'bool',
         'keep_until': 'LiveTvKeepUntil'
     }
 
     attribute_map = {
         'record_any_time': 'RecordAnyTime',
         'skip_episodes_in_library': 'SkipEpisodesInLibrary',
+        'match_existing_items_with_any_library': 'MatchExistingItemsWithAnyLibrary',
         'record_any_channel': 'RecordAnyChannel',
         'keep_up_to': 'KeepUpTo',
         'max_recording_seconds': 'MaxRecordingSeconds',
         'record_new_only': 'RecordNewOnly',
         'channel_ids': 'ChannelIds',
         'days': 'Days',
         'image_tags': 'ImageTags',
@@ -97,18 +99,19 @@
         'is_pre_padding_required': 'IsPrePaddingRequired',
         'parent_backdrop_item_id': 'ParentBackdropItemId',
         'parent_backdrop_image_tags': 'ParentBackdropImageTags',
         'is_post_padding_required': 'IsPostPaddingRequired',
         'keep_until': 'KeepUntil'
     }
 
-    def __init__(self, record_any_time=None, skip_episodes_in_library=None, record_any_channel=None, keep_up_to=None, max_recording_seconds=None, record_new_only=None, channel_ids=None, days=None, image_tags=None, parent_thumb_item_id=None, parent_thumb_image_tag=None, parent_primary_image_item_id=None, parent_primary_image_tag=None, series_id=None, keywords=None, timer_type=None, id=None, type=None, server_id=None, channel_id=None, channel_name=None, channel_number=None, channel_primary_image_tag=None, program_id=None, name=None, overview=None, parent_folder_id=None, start_date=None, end_date=None, priority=None, pre_padding_seconds=None, post_padding_seconds=None, is_pre_padding_required=None, parent_backdrop_item_id=None, parent_backdrop_image_tags=None, is_post_padding_required=None, keep_until=None):  # noqa: E501
+    def __init__(self, record_any_time=None, skip_episodes_in_library=None, match_existing_items_with_any_library=None, record_any_channel=None, keep_up_to=None, max_recording_seconds=None, record_new_only=None, channel_ids=None, days=None, image_tags=None, parent_thumb_item_id=None, parent_thumb_image_tag=None, parent_primary_image_item_id=None, parent_primary_image_tag=None, series_id=None, keywords=None, timer_type=None, id=None, type=None, server_id=None, channel_id=None, channel_name=None, channel_number=None, channel_primary_image_tag=None, program_id=None, name=None, overview=None, parent_folder_id=None, start_date=None, end_date=None, priority=None, pre_padding_seconds=None, post_padding_seconds=None, is_pre_padding_required=None, parent_backdrop_item_id=None, parent_backdrop_image_tags=None, is_post_padding_required=None, keep_until=None):  # noqa: E501
         """LiveTvSeriesTimerInfoDto - a model defined in Swagger"""  # noqa: E501
         self._record_any_time = None
         self._skip_episodes_in_library = None
+        self._match_existing_items_with_any_library = None
         self._record_any_channel = None
         self._keep_up_to = None
         self._max_recording_seconds = None
         self._record_new_only = None
         self._channel_ids = None
         self._days = None
         self._image_tags = None
@@ -141,14 +144,16 @@
         self._is_post_padding_required = None
         self._keep_until = None
         self.discriminator = None
         if record_any_time is not None:
             self.record_any_time = record_any_time
         if skip_episodes_in_library is not None:
             self.skip_episodes_in_library = skip_episodes_in_library
+        if match_existing_items_with_any_library is not None:
+            self.match_existing_items_with_any_library = match_existing_items_with_any_library
         if record_any_channel is not None:
             self.record_any_channel = record_any_channel
         if keep_up_to is not None:
             self.keep_up_to = keep_up_to
         if max_recording_seconds is not None:
             self.max_recording_seconds = max_recording_seconds
         if record_new_only is not None:
@@ -257,14 +262,35 @@
         :param skip_episodes_in_library: The skip_episodes_in_library of this LiveTvSeriesTimerInfoDto.  # noqa: E501
         :type: bool
         """
 
         self._skip_episodes_in_library = skip_episodes_in_library
 
     @property
+    def match_existing_items_with_any_library(self):
+        """Gets the match_existing_items_with_any_library of this LiveTvSeriesTimerInfoDto.  # noqa: E501
+
+
+        :return: The match_existing_items_with_any_library of this LiveTvSeriesTimerInfoDto.  # noqa: E501
+        :rtype: bool
+        """
+        return self._match_existing_items_with_any_library
+
+    @match_existing_items_with_any_library.setter
+    def match_existing_items_with_any_library(self, match_existing_items_with_any_library):
+        """Sets the match_existing_items_with_any_library of this LiveTvSeriesTimerInfoDto.
+
+
+        :param match_existing_items_with_any_library: The match_existing_items_with_any_library of this LiveTvSeriesTimerInfoDto.  # noqa: E501
+        :type: bool
+        """
+
+        self._match_existing_items_with_any_library = match_existing_items_with_any_library
+
+    @property
     def record_any_channel(self):
         """Gets the record_any_channel of this LiveTvSeriesTimerInfoDto.  # noqa: E501
 
         A value indicating whether \\[record any channel\\].  # noqa: E501
 
         :return: The record_any_channel of this LiveTvSeriesTimerInfoDto.  # noqa: E501
         :rtype: bool
```

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_timer_info_dto.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_timer_type.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_timer_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/live_tv_tuner_host_info.py` & `embyclient-4.8.4.0/embyclient/models/live_tv_tuner_host_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/location_type.py` & `embyclient-4.8.4.0/embyclient/models/location_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/log_file.py` & `embyclient-4.8.4.0/embyclient/models/log_file.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/logging_log_severity.py` & `embyclient-4.8.4.0/embyclient/models/logging_log_severity.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/marker_type.py` & `embyclient-4.8.4.0/embyclient/models/marker_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/mb_backup_api_all_backups_info.py` & `embyclient-4.8.4.0/embyclient/models/mb_backup_api_all_backups_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/mb_backup_api_data_restore_options.py` & `embyclient-4.8.4.0/embyclient/models/mb_backup_api_data_restore_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/mb_backup_api_restore_options.py` & `embyclient-4.8.4.0/embyclient/models/mb_backup_api_restore_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/mb_backup_api_user_restore_info.py` & `embyclient-4.8.4.0/embyclient/models/mb_backup_api_user_restore_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/mb_backup_backup_info.py` & `embyclient-4.8.4.0/embyclient/models/mb_backup_backup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_encoding_codec_parameter_context.py` & `embyclient-4.8.4.0/embyclient/models/media_encoding_codec_parameter_context.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_path_info.py` & `embyclient-4.8.4.0/embyclient/models/media_path_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_protocol.py` & `embyclient-4.8.4.0/embyclient/models/media_protocol.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_source_info.py` & `embyclient-4.8.4.0/embyclient/models/media_source_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_source_type.py` & `embyclient-4.8.4.0/embyclient/models/media_source_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_stream.py` & `embyclient-4.8.4.0/embyclient/models/media_stream.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_stream_type.py` & `embyclient-4.8.4.0/embyclient/models/media_stream_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/media_url.py` & `embyclient-4.8.4.0/embyclient/models/media_url.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/metadata_editor_info.py` & `embyclient-4.8.4.0/embyclient/models/metadata_editor_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/metadata_features.py` & `embyclient-4.8.4.0/embyclient/models/metadata_features.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/metadata_fields.py` & `embyclient-4.8.4.0/embyclient/models/metadata_fields.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/metadata_refresh_mode.py` & `embyclient-4.8.4.0/embyclient/models/metadata_refresh_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/movie_info.py` & `embyclient-4.8.4.0/embyclient/models/movie_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/music_video_info.py` & `embyclient-4.8.4.0/embyclient/models/music_video_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/name_id_pair.py` & `embyclient-4.8.4.0/embyclient/models/name_id_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/name_long_id_pair.py` & `embyclient-4.8.4.0/embyclient/models/name_long_id_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/name_value_pair.py` & `embyclient-4.8.4.0/embyclient/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/net_end_point_info.py` & `embyclient-4.8.4.0/embyclient/models/net_end_point_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/net_sockets_address_family.py` & `embyclient-4.8.4.0/embyclient/models/net_sockets_address_family.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/notification_category_info.py` & `embyclient-4.8.4.0/embyclient/models/notification_category_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/notification_type_info.py` & `embyclient-4.8.4.0/embyclient/models/notification_type_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/operating_system.py` & `embyclient-4.8.4.0/embyclient/models/operating_system.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/package_info.py` & `embyclient-4.8.4.0/embyclient/models/package_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/package_target_system.py` & `embyclient-4.8.4.0/embyclient/models/package_target_system.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/package_version_class.py` & `embyclient-4.8.4.0/embyclient/models/package_version_class.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/package_version_info.py` & `embyclient-4.8.4.0/embyclient/models/package_version_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/parental_rating.py` & `embyclient-4.8.4.0/embyclient/models/parental_rating.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/path_substitution.py` & `embyclient-4.8.4.0/embyclient/models/path_substitution.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/persistence_intro_debug_info.py` & `embyclient-4.8.4.0/embyclient/models/persistence_intro_debug_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/person_lookup_info.py` & `embyclient-4.8.4.0/embyclient/models/person_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/person_type.py` & `embyclient-4.8.4.0/embyclient/models/person_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/pin_redeem_result.py` & `embyclient-4.8.4.0/embyclient/models/pin_redeem_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/play_command.py` & `embyclient-4.8.4.0/embyclient/models/play_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/play_method.py` & `embyclient-4.8.4.0/embyclient/models/play_method.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/play_request.py` & `embyclient-4.8.4.0/embyclient/models/play_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playback_error_code.py` & `embyclient-4.8.4.0/embyclient/models/playback_error_code.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playback_info_request.py` & `embyclient-4.8.4.0/embyclient/models/playback_info_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playback_info_response.py` & `embyclient-4.8.4.0/embyclient/models/playback_info_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playback_progress_info.py` & `embyclient-4.8.4.0/embyclient/models/playback_progress_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playback_start_info.py` & `embyclient-4.8.4.0/embyclient/models/playback_start_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playback_stop_info.py` & `embyclient-4.8.4.0/embyclient/models/playback_stop_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/player_state_info.py` & `embyclient-4.8.4.0/embyclient/models/player_state_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playlists_add_to_playlist_result.py` & `embyclient-4.8.4.0/embyclient/models/playlists_add_to_playlist_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playlists_playlist_creation_result.py` & `embyclient-4.8.4.0/embyclient/models/playlists_playlist_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playstate_command.py` & `embyclient-4.8.4.0/embyclient/models/playstate_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/playstate_request.py` & `embyclient-4.8.4.0/embyclient/models/playstate_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/plugins_configuration_page_type.py` & `embyclient-4.8.4.0/embyclient/models/plugins_configuration_page_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/plugins_plugin_info.py` & `embyclient-4.8.4.0/embyclient/models/plugins_plugin_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/process_run_metrics_process_metric_point.py` & `embyclient-4.8.4.0/embyclient/models/process_run_metrics_process_metric_point.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/process_run_metrics_process_statistics.py` & `embyclient-4.8.4.0/embyclient/models/process_run_metrics_process_statistics.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/profile_condition.py` & `embyclient-4.8.4.0/embyclient/models/profile_condition.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/profile_condition_type.py` & `embyclient-4.8.4.0/embyclient/models/profile_condition_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/profile_condition_value.py` & `embyclient-4.8.4.0/embyclient/models/profile_condition_value.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/profile_information.py` & `embyclient-4.8.4.0/embyclient/models/profile_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/profile_level_information.py` & `embyclient-4.8.4.0/embyclient/models/profile_level_information.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/progress_event.py` & `embyclient-4.8.4.0/embyclient/models/progress_event.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/provider_id_dictionary.py` & `embyclient-4.8.4.0/embyclient/models/provider_id_dictionary.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/proxy_header_mode.py` & `embyclient-4.8.4.0/embyclient/models/proxy_header_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/public_system_info.py` & `embyclient-4.8.4.0/embyclient/models/public_system_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_activity_log_entry.py` & `embyclient-4.8.4.0/embyclient/models/query_result_activity_log_entry.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_api_epg_row.py` & `embyclient-4.8.4.0/embyclient/models/query_result_api_epg_row.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_base_item_dto.py` & `embyclient-4.8.4.0/embyclient/models/query_result_base_item_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_channel_management_info.py` & `embyclient-4.8.4.0/embyclient/models/query_result_channel_management_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_devices_device_info.py` & `embyclient-4.8.4.0/embyclient/models/query_result_devices_device_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py` & `embyclient-4.8.4.0/embyclient/models/query_result_live_tv_series_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_live_tv_timer_info_dto.py` & `embyclient-4.8.4.0/embyclient/models/query_result_live_tv_timer_info_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_log_file.py` & `embyclient-4.8.4.0/embyclient/models/query_result_log_file.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_string.py` & `embyclient-4.8.4.0/embyclient/models/query_result_string.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_sync_job.py` & `embyclient-4.8.4.0/embyclient/models/query_result_sync_job.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_sync_job_item.py` & `embyclient-4.8.4.0/embyclient/models/query_result_sync_job_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_user_dto.py` & `embyclient-4.8.4.0/embyclient/models/query_result_user_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_user_library_official_rating_item.py` & `embyclient-4.8.4.0/embyclient/models/query_result_user_library_official_rating_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_user_library_tag_item.py` & `embyclient-4.8.4.0/embyclient/models/query_result_user_library_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/query_result_virtual_folder_info.py` & `embyclient-4.8.4.0/embyclient/models/query_result_virtual_folder_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/queue_item.py` & `embyclient-4.8.4.0/embyclient/models/queue_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/rating_type.py` & `embyclient-4.8.4.0/embyclient/models/rating_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/recommendation_dto.py` & `embyclient-4.8.4.0/embyclient/models/recommendation_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/recommendation_type.py` & `embyclient-4.8.4.0/embyclient/models/recommendation_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_image_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_image_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_image_result.py` & `embyclient-4.8.4.0/embyclient/models/remote_image_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_album_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_album_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_artist_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_artist_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_book_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_book_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_game_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_game_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_item_lookup_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_item_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_movie_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_movie_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_music_video_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_music_video_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_person_lookup_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_person_lookup_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_series_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_series_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_query_trailer_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_query_trailer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_search_result.py` & `embyclient-4.8.4.0/embyclient/models/remote_search_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/remote_subtitle_info.py` & `embyclient-4.8.4.0/embyclient/models/remote_subtitle_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/repeat_mode.py` & `embyclient-4.8.4.0/embyclient/models/repeat_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/resolution.py` & `embyclient-4.8.4.0/embyclient/models/resolution.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/resolution_with_rate.py` & `embyclient-4.8.4.0/embyclient/models/resolution_with_rate.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/response_profile.py` & `embyclient-4.8.4.0/embyclient/models/response_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/roku_metadata_api_thumbnail_info.py` & `embyclient-4.8.4.0/embyclient/models/roku_metadata_api_thumbnail_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py` & `embyclient-4.8.4.0/embyclient/models/roku_metadata_api_thumbnail_set_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/run_ui_command.py` & `embyclient-4.8.4.0/embyclient/models/run_ui_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/secondary_frameworks.py` & `embyclient-4.8.4.0/embyclient/models/secondary_frameworks.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/segment_skip_mode.py` & `embyclient-4.8.4.0/embyclient/models/segment_skip_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/series_display_order.py` & `embyclient-4.8.4.0/embyclient/models/series_display_order.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/series_info.py` & `embyclient-4.8.4.0/embyclient/models/series_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/server_configuration.py` & `embyclient-4.8.4.0/embyclient/models/server_configuration.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/session_session_info.py` & `embyclient-4.8.4.0/embyclient/models/session_session_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/session_user_info.py` & `embyclient-4.8.4.0/embyclient/models/session_user_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/song_info.py` & `embyclient-4.8.4.0/embyclient/models/song_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sort_order.py` & `embyclient-4.8.4.0/embyclient/models/sort_order.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/subtitle_delivery_method.py` & `embyclient-4.8.4.0/embyclient/models/subtitle_delivery_method.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/subtitle_location_type.py` & `embyclient-4.8.4.0/embyclient/models/subtitle_location_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/subtitle_playback_mode.py` & `embyclient-4.8.4.0/embyclient/models/subtitle_playback_mode.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/subtitle_profile.py` & `embyclient-4.8.4.0/embyclient/models/subtitle_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/subtitles_subtitle_download_result.py` & `embyclient-4.8.4.0/embyclient/models/subtitles_subtitle_download_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_category.py` & `embyclient-4.8.4.0/embyclient/models/sync_category.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_data_request.py` & `embyclient-4.8.4.0/embyclient/models/sync_data_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_data_response.py` & `embyclient-4.8.4.0/embyclient/models/sync_data_response.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_dialog_options.py` & `embyclient-4.8.4.0/embyclient/models/sync_dialog_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_job.py` & `embyclient-4.8.4.0/embyclient/models/sync_job.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_job_creation_result.py` & `embyclient-4.8.4.0/embyclient/models/sync_job_creation_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_job_item.py` & `embyclient-4.8.4.0/embyclient/models/sync_job_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_job_item_status.py` & `embyclient-4.8.4.0/embyclient/models/sync_job_item_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_job_option.py` & `embyclient-4.8.4.0/embyclient/models/sync_job_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_job_request.py` & `embyclient-4.8.4.0/embyclient/models/sync_job_request.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_job_status.py` & `embyclient-4.8.4.0/embyclient/models/sync_job_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_profile_option.py` & `embyclient-4.8.4.0/embyclient/models/sync_profile_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_quality_option.py` & `embyclient-4.8.4.0/embyclient/models/sync_quality_option.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/sync_target.py` & `embyclient-4.8.4.0/embyclient/models/sync_target.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/synced_item.py` & `embyclient-4.8.4.0/embyclient/models/synced_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/synced_item_progress.py` & `embyclient-4.8.4.0/embyclient/models/synced_item_progress.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/system_event.py` & `embyclient-4.8.4.0/embyclient/models/system_event.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/system_info.py` & `embyclient-4.8.4.0/embyclient/models/system_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/task_completion_status.py` & `embyclient-4.8.4.0/embyclient/models/task_completion_status.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/task_info.py` & `embyclient-4.8.4.0/embyclient/models/task_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/task_result.py` & `embyclient-4.8.4.0/embyclient/models/task_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/task_state.py` & `embyclient-4.8.4.0/embyclient/models/task_state.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/task_trigger_info.py` & `embyclient-4.8.4.0/embyclient/models/task_trigger_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/theme_media_result.py` & `embyclient-4.8.4.0/embyclient/models/theme_media_result.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/trailer_info.py` & `embyclient-4.8.4.0/embyclient/models/trailer_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/transcode_reason.py` & `embyclient-4.8.4.0/embyclient/models/transcode_reason.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/transcode_seek_info.py` & `embyclient-4.8.4.0/embyclient/models/transcode_seek_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/transcoding_info.py` & `embyclient-4.8.4.0/embyclient/models/transcoding_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/transcoding_profile.py` & `embyclient-4.8.4.0/embyclient/models/transcoding_profile.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/transcoding_vp_step_info.py` & `embyclient-4.8.4.0/embyclient/models/transcoding_vp_step_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/transcoding_vp_step_types.py` & `embyclient-4.8.4.0/embyclient/models/transcoding_vp_step_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/transport_stream_timestamp.py` & `embyclient-4.8.4.0/embyclient/models/transport_stream_timestamp.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/tuple_double_double.py` & `embyclient-4.8.4.0/embyclient/models/tuple_double_double.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/type_options.py` & `embyclient-4.8.4.0/embyclient/models/type_options.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/ui_command.py` & `embyclient-4.8.4.0/embyclient/models/ui_command.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/ui_tab_page_info.py` & `embyclient-4.8.4.0/embyclient/models/ui_tab_page_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/ui_view_info.py` & `embyclient-4.8.4.0/embyclient/models/ui_view_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/unrated_item.py` & `embyclient-4.8.4.0/embyclient/models/unrated_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/update_user_password.py` & `embyclient-4.8.4.0/embyclient/models/update_user_password.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_action.py` & `embyclient-4.8.4.0/embyclient/models/user_action.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_action_type.py` & `embyclient-4.8.4.0/embyclient/models/user_action_type.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_configuration.py` & `embyclient-4.8.4.0/embyclient/models/user_configuration.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_dto.py` & `embyclient-4.8.4.0/embyclient/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_item_data_dto.py` & `embyclient-4.8.4.0/embyclient/models/user_item_data_dto.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_item_share_level.py` & `embyclient-4.8.4.0/embyclient/models/user_item_share_level.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_library_add_tags.py` & `embyclient-4.8.4.0/embyclient/models/user_library_add_tags.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_library_leave_shared_items.py` & `embyclient-4.8.4.0/embyclient/models/user_library_leave_shared_items.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_library_official_rating_item.py` & `embyclient-4.8.4.0/embyclient/models/user_library_official_rating_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_library_remove_tags.py` & `embyclient-4.8.4.0/embyclient/models/user_library_remove_tags.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_library_tag_item.py` & `embyclient-4.8.4.0/embyclient/models/user_library_tag_item.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_library_update_user_item_access.py` & `embyclient-4.8.4.0/embyclient/models/user_library_update_user_item_access.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/user_notification_info.py` & `embyclient-4.8.4.0/embyclient/models/user_notification_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         'enabled': 'bool',
         'user_ids': 'list[str]',
         'device_ids': 'list[str]',
         'library_ids': 'list[str]',
         'event_ids': 'list[str]',
         'user_id': 'str',
         'is_self_notification': 'bool',
+        'group_items': 'bool',
         'options': 'dict(str, str)'
     }
 
     attribute_map = {
         'notifier_key': 'NotifierKey',
         'setup_module_url': 'SetupModuleUrl',
         'service_name': 'ServiceName',
@@ -48,32 +49,34 @@
         'enabled': 'Enabled',
         'user_ids': 'UserIds',
         'device_ids': 'DeviceIds',
         'library_ids': 'LibraryIds',
         'event_ids': 'EventIds',
         'user_id': 'UserId',
         'is_self_notification': 'IsSelfNotification',
+        'group_items': 'GroupItems',
         'options': 'Options'
     }
 
-    def __init__(self, notifier_key=None, setup_module_url=None, service_name=None, plugin_id=None, friendly_name=None, id=None, enabled=None, user_ids=None, device_ids=None, library_ids=None, event_ids=None, user_id=None, is_self_notification=None, options=None):  # noqa: E501
+    def __init__(self, notifier_key=None, setup_module_url=None, service_name=None, plugin_id=None, friendly_name=None, id=None, enabled=None, user_ids=None, device_ids=None, library_ids=None, event_ids=None, user_id=None, is_self_notification=None, group_items=None, options=None):  # noqa: E501
         """UserNotificationInfo - a model defined in Swagger"""  # noqa: E501
         self._notifier_key = None
         self._setup_module_url = None
         self._service_name = None
         self._plugin_id = None
         self._friendly_name = None
         self._id = None
         self._enabled = None
         self._user_ids = None
         self._device_ids = None
         self._library_ids = None
         self._event_ids = None
         self._user_id = None
         self._is_self_notification = None
+        self._group_items = None
         self._options = None
         self.discriminator = None
         if notifier_key is not None:
             self.notifier_key = notifier_key
         if setup_module_url is not None:
             self.setup_module_url = setup_module_url
         if service_name is not None:
@@ -94,14 +97,16 @@
             self.library_ids = library_ids
         if event_ids is not None:
             self.event_ids = event_ids
         if user_id is not None:
             self.user_id = user_id
         if is_self_notification is not None:
             self.is_self_notification = is_self_notification
+        if group_items is not None:
+            self.group_items = group_items
         if options is not None:
             self.options = options
 
     @property
     def notifier_key(self):
         """Gets the notifier_key of this UserNotificationInfo.  # noqa: E501
 
@@ -375,14 +380,35 @@
         :param is_self_notification: The is_self_notification of this UserNotificationInfo.  # noqa: E501
         :type: bool
         """
 
         self._is_self_notification = is_self_notification
 
     @property
+    def group_items(self):
+        """Gets the group_items of this UserNotificationInfo.  # noqa: E501
+
+
+        :return: The group_items of this UserNotificationInfo.  # noqa: E501
+        :rtype: bool
+        """
+        return self._group_items
+
+    @group_items.setter
+    def group_items(self, group_items):
+        """Sets the group_items of this UserNotificationInfo.
+
+
+        :param group_items: The group_items of this UserNotificationInfo.  # noqa: E501
+        :type: bool
+        """
+
+        self._group_items = group_items
+
+    @property
     def options(self):
         """Gets the options of this UserNotificationInfo.  # noqa: E501
 
         This is for webhooks since this will cause xml serialization to fail  # noqa: E501
 
         :return: The options of this UserNotificationInfo.  # noqa: E501
         :rtype: dict(str, str)
```

### Comparing `embyclient-4.8.3.0/embyclient/models/user_policy.py` & `embyclient-4.8.4.0/embyclient/models/user_policy.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/validate_path.py` & `embyclient-4.8.4.0/embyclient/models/validate_path.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/version.py` & `embyclient-4.8.4.0/embyclient/models/version.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/video3_d_format.py` & `embyclient-4.8.4.0/embyclient/models/video3_d_format.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/video_codec_base.py` & `embyclient-4.8.4.0/embyclient/models/video_codec_base.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/video_media_types.py` & `embyclient-4.8.4.0/embyclient/models/video_media_types.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/virtual_folder_info.py` & `embyclient-4.8.4.0/embyclient/models/virtual_folder_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/models/wake_on_lan_info.py` & `embyclient-4.8.4.0/embyclient/models/wake_on_lan_info.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient/rest.py` & `embyclient-4.8.4.0/embyclient/rest.py`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/embyclient.egg-info/SOURCES.txt` & `embyclient-4.8.4.0/embyclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embyclient-4.8.3.0/setup.py` & `embyclient-4.8.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-VERSION = "4.8.3.0"
+VERSION = "4.8.4.0"
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 
 classifiers = [
     'Intended Audience :: Developers',  # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'Topic :: Multimedia :: Video',
```

