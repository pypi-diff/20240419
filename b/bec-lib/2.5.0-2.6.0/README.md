# Comparing `tmp/bec_lib-2.5.0.tar.gz` & `tmp/bec_lib-2.6.0.tar.gz`

## Comparing `bec_lib-2.5.0.tar` & `bec_lib-2.6.0.tar`

### file list

```diff
@@ -1,88 +1,90 @@
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bec_lib-2.5.0/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/__init__.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/alarm_handler.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/async_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bec_errors.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bec_service.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bl_checks.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/bl_conditions.py
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/callback_handler.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/channel_monitor.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/client.py
--rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/config_helper.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/connector.py
--rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/dap_plugin_objects.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/dap_plugins.py
--rw-r--r--   0        0        0    30828 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/device.py
--rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/devicemanager.py
--rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/endpoints.py
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/file_utils.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/lmfit_serializer.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/logbook_connector.py
--rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/logger.py
--rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/messages.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/numpy_encoder.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/observer.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/pdf_writer.py
--rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/queue_items.py
--rw-r--r--   0        0        0    39020 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/redis_connector.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/request_items.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_data.py
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_items.py
--rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_manager.py
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scan_report.py
--rw-r--r--   0        0        0    17027 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scans.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/scibec_validator.py
--rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/serialization.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/service_config.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/signature_serializer.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/user_scripts_mixin.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/configs/__init__.py
--rw-r--r--   0        0        0    38908 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/configs/demo_config.yaml
--rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/configs/openapi_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/__init__.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/fixtures.py
--rw-r--r--   0        0        0    41009 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/test_config.yaml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/test_service_config.yaml
--rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 bec_lib-2.5.0/bec_lib/tests/utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/conftest.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_async_data.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_beamline_checks.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bec_logger.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bec_messages.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bec_service.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_bl_conditions.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_callback_handler.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_channel_monitor.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_config_helper.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_core_utils.py
--rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_dap_plugins.py
--rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_device_manager.py
--rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_devices.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_file_utils.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_lmfit_serializer.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_observer.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_pdf_writer.py
--rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_redis_connector.py
--rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_redis_connector_fakeredis.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_context.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_data.py
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_items.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_manager.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_object.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scan_report.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_scibec_validator.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_serializer.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_signature_serializer.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bec_lib-2.5.0/tests/test_user_scripts_mixin.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/create_plugin_structure.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/init_config.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/post_startup.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/pre_startup.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/scan_plugin_template.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/setup.cfg
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bec_lib-2.5.0/util_scripts/plugin_setup_files/setup.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.5.0/.gitignore
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 bec_lib-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 bec_lib-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 bec_lib-2.6.0/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/__init__.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/alarm_handler.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/async_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/bec_errors.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/bec_service.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/bl_checks.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/bl_conditions.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/callback_handler.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/channel_monitor.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/client.py
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/config_helper.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/connector.py
+-rw-r--r--   0        0        0    12816 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/dap_plugin_objects.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/dap_plugins.py
+-rw-r--r--   0        0        0    30828 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/device.py
+-rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/devicemanager.py
+-rw-r--r--   0        0        0    37595 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/endpoints.py
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/file_utils.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/lmfit_serializer.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/logbook_connector.py
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/logger.py
+-rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/messages.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/numpy_encoder.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/observer.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/pdf_writer.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/plugin_helper.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/queue_items.py
+-rw-r--r--   0        0        0    39020 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/redis_connector.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/request_items.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/scan_data.py
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/scan_items.py
+-rw-r--r--   0        0        0     8573 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/scan_manager.py
+-rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/scan_report.py
+-rw-r--r--   0        0        0    17027 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/scans.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/scibec_validator.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/serialization.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/service_config.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/signature_serializer.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/user_scripts_mixin.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/configs/__init__.py
+-rw-r--r--   0        0        0    41862 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/configs/demo_config.yaml
+-rw-r--r--   0        0        0   289604 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/configs/openapi_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/tests/__init__.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/tests/fixtures.py
+-rw-r--r--   0        0        0    44047 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/tests/test_config.yaml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/tests/test_service_config.yaml
+-rw-r--r--   0        0        0    22469 2020-02-02 00:00:00.000000 bec_lib-2.6.0/bec_lib/tests/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_async_data.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_beamline_checks.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_bec_logger.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_bec_messages.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_bec_service.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_bl_conditions.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_channel_monitor.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_config_helper.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_core_utils.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_dap_plugins.py
+-rw-r--r--   0        0        0    11924 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_device_manager.py
+-rw-r--r--   0        0        0    25797 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_devices.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_file_utils.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_lmfit_serializer.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_observer.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_pdf_writer.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_plugin_helper.py
+-rw-r--r--   0        0        0    15768 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_redis_connector.py
+-rw-r--r--   0        0        0    17701 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_redis_connector_fakeredis.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_scan_context.py
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_scan_data.py
+-rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_scan_items.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_scan_manager.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_scan_object.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_scan_report.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_scibec_validator.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_serializer.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_signature_serializer.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bec_lib-2.6.0/tests/test_user_scripts_mixin.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 bec_lib-2.6.0/util_scripts/create_plugin_structure.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bec_lib-2.6.0/util_scripts/init_config.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 bec_lib-2.6.0/util_scripts/plugin_setup_files/post_startup.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 bec_lib-2.6.0/util_scripts/plugin_setup_files/pre_startup.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 bec_lib-2.6.0/util_scripts/plugin_setup_files/scan_plugin_template.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 bec_lib-2.6.0/util_scripts/plugin_setup_files/setup.cfg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bec_lib-2.6.0/util_scripts/plugin_setup_files/setup.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_lib-2.6.0/.gitignore
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 bec_lib-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 bec_lib-2.6.0/PKG-INFO
```

### Comparing `bec_lib-2.5.0/README.md` & `bec_lib-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/__init__.py` & `bec_lib-2.6.0/bec_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/alarm_handler.py` & `bec_lib-2.6.0/bec_lib/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/async_data.py` & `bec_lib-2.6.0/bec_lib/async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/bec_service.py` & `bec_lib-2.6.0/bec_lib/bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/bl_checks.py` & `bec_lib-2.6.0/bec_lib/bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/bl_conditions.py` & `bec_lib-2.6.0/bec_lib/bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/callback_handler.py` & `bec_lib-2.6.0/bec_lib/callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/channel_monitor.py` & `bec_lib-2.6.0/bec_lib/channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/client.py` & `bec_lib-2.6.0/bec_lib/client.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/config_helper.py` & `bec_lib-2.6.0/bec_lib/config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/connector.py` & `bec_lib-2.6.0/bec_lib/connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/dap_plugin_objects.py` & `bec_lib-2.6.0/bec_lib/dap_plugin_objects.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/dap_plugins.py` & `bec_lib-2.6.0/bec_lib/dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/device.py` & `bec_lib-2.6.0/bec_lib/device.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/devicemanager.py` & `bec_lib-2.6.0/bec_lib/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/endpoints.py` & `bec_lib-2.6.0/bec_lib/endpoints.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/file_utils.py` & `bec_lib-2.6.0/bec_lib/file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/lmfit_serializer.py` & `bec_lib-2.6.0/bec_lib/lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/logbook_connector.py` & `bec_lib-2.6.0/bec_lib/logbook_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/logger.py` & `bec_lib-2.6.0/bec_lib/logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/messages.py` & `bec_lib-2.6.0/bec_lib/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,22 @@
     msg_type: ClassVar[str] = "bundle_message"
     messages: list = Field(default_factory=list[BECMessage])
 
     def append(self, msg: BECMessage):
         """append a new BECMessage to the bundle"""
         if not isinstance(msg, BECMessage):
             raise AttributeError(f"Cannot append message of type {msg.__class__.__name__}")
+        # pylint: disable=no-member
         self.messages.append(msg)
 
     def __len__(self):
         return len(self.messages)
 
     def __iter__(self):
+        # pylint: disable=not-an-iterable
         yield from self.messages
 
 
 class ScanQueueMessage(BECMessage):
     """Message type for sending scan requests to the scan queue
     Sent by the API server / user to the scan_queue topic. It will be consumed by the scan server.
         Args:
```

### Comparing `bec_lib-2.5.0/bec_lib/numpy_encoder.py` & `bec_lib-2.6.0/bec_lib/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/observer.py` & `bec_lib-2.6.0/bec_lib/observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/pdf_writer.py` & `bec_lib-2.6.0/bec_lib/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/queue_items.py` & `bec_lib-2.6.0/bec_lib/queue_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/redis_connector.py` & `bec_lib-2.6.0/bec_lib/redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/request_items.py` & `bec_lib-2.6.0/bec_lib/request_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/scan_data.py` & `bec_lib-2.6.0/bec_lib/scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/scan_items.py` & `bec_lib-2.6.0/bec_lib/scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/scan_manager.py` & `bec_lib-2.6.0/bec_lib/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/scan_report.py` & `bec_lib-2.6.0/bec_lib/scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/scans.py` & `bec_lib-2.6.0/bec_lib/scans.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/scibec_validator.py` & `bec_lib-2.6.0/bec_lib/scibec_validator.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/serialization.py` & `bec_lib-2.6.0/bec_lib/serialization.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/service_config.py` & `bec_lib-2.6.0/bec_lib/service_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/signature_serializer.py` & `bec_lib-2.6.0/bec_lib/signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/user_scripts_mixin.py` & `bec_lib-2.6.0/bec_lib/user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/utils.py` & `bec_lib-2.6.0/bec_lib/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/configs/demo_config.yaml` & `bec_lib-2.6.0/bec_lib/configs/demo_config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 ############################################################
 ################## Cameras and detectors ###################
 ############################################################
 
 eiger:
   readoutPriority: monitored
-  deviceClass: SimCamera
+  deviceClass: ophyd_devices.SimCamera
   deviceConfig:
     device_access: true
   deviceTags:
     - detector
   enabled: true
   readOnly: false
   softwareTrigger: true
 
 ############## Cameras and detectors end here ##############
 
 dyn_signals:
   readoutPriority: baseline
-  deviceClass: sim:sim:SynDynamicComponents
+  deviceClass: ophyd_devices.sim.sim.SynDynamicComponents
   deviceConfig:
   enabled: true
   readOnly: false
 
 pseudo_signal1:
-  deviceClass: ComputedSignal
+  deviceClass: ophyd_devices.ComputedSignal
   deviceConfig:
     compute_method: "def compute_signals(signal1, signal2):\n    return signal1.get()*signal2.get()\n"
     input_signals: 
       - "bpm4i_readback"
       - "bpm5i_readback"
   enabled: true
   readOnly: false
@@ -35,259 +35,259 @@
 
 ############################################################
 ####################### User motors ########################
 ############################################################
 
 hexapod:
   readoutPriority: baseline
-  deviceClass: SynDeviceOPAAS
+  deviceClass: ophyd_devices.SynDeviceOPAAS
   deviceConfig:
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 
 eyefoc:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyex:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyey:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 flyer_sim:
   readoutPriority: on_request
-  deviceClass: SynFlyer
+  deviceClass: ophyd_devices.SynFlyer
   deviceConfig:
     delay: 1    
     device_access: true
     update_frequency: 400
   deviceTags:
     - flyer
   enabled: true
   readOnly: false
 hrox:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 piny:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
@@ -300,1800 +300,1800 @@
 
 ############################################################
 #################### Beamline monitors #####################
 ############################################################
 
 bpm3a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4s:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4xf:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4xm:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4yf:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4ym:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 curr:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 diode:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmdx:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmdy:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmux:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmuy:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ftp:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 temp:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 transd:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 
 ################ Beamline monitors end here ################
 
 ############################################################
 ##################### Beamline motors ######################
 ############################################################
 
 aptrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 aptry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2y:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4r:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5r:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1y:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2y:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstn:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstr:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1a:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1b:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1c:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1d:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1f:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1g:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1h:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dettrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtpush:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtth:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi3:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi4:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi1try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi2try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi3try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh1x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh2x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ftrans:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 idgap:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 miroll:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mith:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry3:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobd:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdai:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdbo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdco:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobddi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mokev:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrx2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moyaw2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 strox:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
@@ -2102,15 +2102,15 @@
 
 ############################################################
 #################### Read-only signals #####################
 ############################################################
 
 ring_current_sim:
   readoutPriority: monitored
-  deviceClass: ReadOnlySignal
+  deviceClass: ophyd_devices.ReadOnlySignal
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ################ Read-only signals end here ################
```

### Comparing `bec_lib-2.5.0/bec_lib/configs/openapi_schema.json` & `bec_lib-2.6.0/bec_lib/configs/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/tests/fixtures.py` & `bec_lib-2.6.0/bec_lib/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/bec_lib/tests/test_config.yaml` & `bec_lib-2.6.0/bec_lib/tests/test_config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,293 +1,293 @@
 ############################################################
 ################## Cameras and detectors ###################
 ############################################################
 
 eiger:
   readoutPriority: monitored
-  deviceClass: SimCamera
+  deviceClass: ophyd_devices.SimCamera
   deviceConfig:
     device_access: true
   deviceTags:
     - detector
   enabled: true
   readOnly: false
   softwareTrigger: true
 
 ############## Cameras and detectors end here ##############
 
 dyn_signals:
   readoutPriority: baseline
-  deviceClass: sim:sim:SynDynamicComponents
+  deviceClass: ophyd_devices.sim.sim.SynDynamicComponents
   deviceConfig:
   enabled: true
   readOnly: false
 
 pseudo_signal1:
-  deviceClass: ComputedSignal
+  deviceClass: ophyd_devices.ComputedSignal
   deviceConfig:
     compute_method: "def compute_signals(signal1, signal2):\n    return signal1.get()*signal2.get()\n"
     input_signals: 
       - "bpm4i_readback"
       - "bpm5i_readback"
   enabled: true
   readOnly: false
   readoutPriority: baseline
 
 failure_device:
-  deviceClass: sim:sim:SimPositionerWithCommFailure
+  deviceClass: ophyd_devices.sim.sim.SimPositionerWithCommFailure
   deviceConfig:
     delay: 1
     update_frequency: 400
   enabled: true
   readOnly: false
   readoutPriority: baseline
 
 ############################################################
 ####################### User motors ########################
 ############################################################
 
 eyefoc:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyex:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 eyey:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 flyer_sim:
   readoutPriority: on_request
-  deviceClass: SynFlyer
+  deviceClass: ophyd_devices.SynFlyer
   deviceConfig:
     delay: 1    
     device_access: true
     update_frequency: 400
   deviceTags:
     - flyer
   enabled: true
   readOnly: false
 hrox:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hroz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 hz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 mbsy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 piny:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 pinz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
   deviceTags:
     - user motors
   enabled: true
   readOnly: false
 samz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1    
     limits:
       - -50
       - 50
     tolerance: 0.01
     update_frequency: 400
@@ -300,1800 +300,1800 @@
 
 ############################################################
 #################### Beamline monitors #####################
 ############################################################
 
 bpm3a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm3z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4s:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4xf:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4xm:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4yf:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4ym:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6a:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6b:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6c:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6d:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6i:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6x:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6y:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm6z:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 curr:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 diode:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmdx:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmdy:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmux:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebpmuy:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ftp:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 temp:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 transd:
   readoutPriority: monitored
-  deviceClass: SimMonitor
+  deviceClass: ophyd_devices.SimMonitor
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 
 ################ Beamline monitors end here ################
 
 ############################################################
 ##################### Beamline motors ######################
 ############################################################
 
 aptrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 aptry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bim2y:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm1try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm2try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm3try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm4try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm5try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bm6try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm4r:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bpm5r:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs1y:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 bs2y:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstn:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 burstr:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1a:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1b:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1c:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1d:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1f:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1g:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ddg1h:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dettrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2trx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 di2try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtpush:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dtth:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 dttrz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebcsy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi3:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfi4:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebfzpy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ebtrz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi1try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi2try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fi3try:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh1x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fsh2x:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ftrans:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrx2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttry2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 fttrz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 idgap:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mibd2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 miroll:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mith:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mitry3:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobd:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdai:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdbo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobdco:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mobddi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mokev:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 mopush2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moroll2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth1e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moth2e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrx2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motry2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 motrz1e:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 moyaw2:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl0wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl1wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl2wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl3wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl4wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5ch:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5cv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxi:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5trxo:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryb:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5tryt:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wh:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sl5wv:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 strox:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroy:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 stroz:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttrx:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 sttry:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     update_frequency: 400
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
@@ -2102,30 +2102,30 @@
 
 ############################################################
 #################### Read-only signals #####################
 ############################################################
 
 ring_current_sim:
   readoutPriority: monitored
-  deviceClass: ReadOnlySignal
+  deviceClass: ophyd_devices.ReadOnlySignal
   deviceConfig:
   deviceTags:
     - beamline
   enabled: true
   readOnly: false
 ################ Read-only signals end here ################
 
 
 ############################################################
 ##################### Disabled devices #####################
 ############################################################
 
 motor1_disabled:
   readoutPriority: monitored
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     labels: motor1_disabled
     limits:
     - -50
     - 50
     name: motor1_disabled
@@ -2133,15 +2133,15 @@
     update_frequency: 400
   deviceTags:
   - user motors
   enabled: false
   readOnly: false
 motor1_disabled_set:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     labels: motor1_disabled_set
     limits:
     - -50
     - 50
     name: motor1_disabled_set
@@ -2149,15 +2149,15 @@
     update_frequency: 400
   deviceTags:
   - user motors
   enabled: true
   readOnly: true
 motor2_disabled:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     labels: motor2_disabled
     limits:
     - -50
     - 50
     name: motor2_disabled
@@ -2165,15 +2165,15 @@
     update_frequency: 400
   deviceTags:
   - user motors
   enabled: false
   readOnly: false
 motor2_disabled_set:
   readoutPriority: baseline
-  deviceClass: SimPositioner
+  deviceClass: ophyd_devices.SimPositioner
   deviceConfig:
     delay: 1
     labels: motor2_disabled_set
     limits:
     - -50
     - 50
     name: motor2_disabled_set
@@ -2182,25 +2182,25 @@
   deviceTags:
   - user motors
   enabled: true
   readOnly: true
 ######### DeviceProxy and SimCamera for delayed init tests ##########
 proxy_cam_test:
   readoutPriority: monitored
-  deviceClass: SimCamera
+  deviceClass: ophyd_devices.SimCamera
   deviceConfig:
     device_access: true
   deviceTags:
     - detector
   enabled: true
   readOnly: false
   softwareTrigger: false
 sim_proxy_test:
   readoutPriority: on_request
-  deviceClass: SlitProxy
+  deviceClass: ophyd_devices.SlitProxy
   deviceConfig:
     proxy_cam_test:
       signal_name: image
       center_offset: [0, 0] # [x,y]
       covariance: [[1000, 500], [200, 1000]] # [[x,x],[y,y]]
       pixel_size: 0.01
       ref_motors: [samx, samy]
```

### Comparing `bec_lib-2.5.0/bec_lib/tests/utils.py` & `bec_lib-2.6.0/bec_lib/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_async_data.py` & `bec_lib-2.6.0/tests/test_async_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_beamline_checks.py` & `bec_lib-2.6.0/tests/test_beamline_checks.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_bec_logger.py` & `bec_lib-2.6.0/tests/test_bec_logger.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_bec_messages.py` & `bec_lib-2.6.0/tests/test_bec_messages.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_bec_service.py` & `bec_lib-2.6.0/tests/test_bec_service.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_bl_conditions.py` & `bec_lib-2.6.0/tests/test_bl_conditions.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_callback_handler.py` & `bec_lib-2.6.0/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_channel_monitor.py` & `bec_lib-2.6.0/tests/test_channel_monitor.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_config_helper.py` & `bec_lib-2.6.0/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_core_utils.py` & `bec_lib-2.6.0/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_dap_plugins.py` & `bec_lib-2.6.0/tests/test_dap_plugins.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_device_manager.py` & `bec_lib-2.6.0/tests/test_device_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_devices.py` & `bec_lib-2.6.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_file_utils.py` & `bec_lib-2.6.0/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_lmfit_serializer.py` & `bec_lib-2.6.0/tests/test_lmfit_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_observer.py` & `bec_lib-2.6.0/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_redis_connector.py` & `bec_lib-2.6.0/tests/test_redis_connector.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_redis_connector_fakeredis.py` & `bec_lib-2.6.0/tests/test_redis_connector_fakeredis.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_scan_context.py` & `bec_lib-2.6.0/tests/test_scan_context.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_scan_data.py` & `bec_lib-2.6.0/tests/test_scan_data.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_scan_items.py` & `bec_lib-2.6.0/tests/test_scan_items.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_scan_manager.py` & `bec_lib-2.6.0/tests/test_scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_scan_object.py` & `bec_lib-2.6.0/tests/test_scan_object.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_scan_report.py` & `bec_lib-2.6.0/tests/test_scan_report.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_serializer.py` & `bec_lib-2.6.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_signature_serializer.py` & `bec_lib-2.6.0/tests/test_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/tests/test_user_scripts_mixin.py` & `bec_lib-2.6.0/tests/test_user_scripts_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/util_scripts/create_plugin_structure.py` & `bec_lib-2.6.0/util_scripts/create_plugin_structure.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/util_scripts/init_config.py` & `bec_lib-2.6.0/util_scripts/init_config.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/util_scripts/plugin_setup_files/post_startup.py` & `bec_lib-2.6.0/util_scripts/plugin_setup_files/post_startup.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/util_scripts/plugin_setup_files/pre_startup.py` & `bec_lib-2.6.0/util_scripts/plugin_setup_files/pre_startup.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/util_scripts/plugin_setup_files/scan_plugin_template.py` & `bec_lib-2.6.0/util_scripts/plugin_setup_files/scan_plugin_template.py`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/util_scripts/plugin_setup_files/setup.cfg` & `bec_lib-2.6.0/util_scripts/plugin_setup_files/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/.gitignore` & `bec_lib-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_lib-2.5.0/pyproject.toml` & `bec_lib-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_lib"
-version = "2.5.0"
+version = "2.6.0"
 description = "BEC library"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `bec_lib-2.5.0/PKG-INFO` & `bec_lib-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec_lib
-Version: 2.5.0
+Version: 2.6.0
 Summary: BEC library
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

