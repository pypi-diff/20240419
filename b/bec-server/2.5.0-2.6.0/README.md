# Comparing `tmp/bec_server-2.5.0.tar.gz` & `tmp/bec_server-2.6.0.tar.gz`

## Comparing `bec_server-2.5.0.tar` & `bec_server-2.6.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/README.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    18964 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    23444 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0    11717 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/file_writer_plugins/default_writer.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    34791 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/LamNIFermatScan.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/owis_grid.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scan_server/scan_plugins/sgalil_grid.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.5.0/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25541 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_flomni_fermat_scan.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11570 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    26372 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    53971 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0   108162 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scan_server/utils.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.5.0/tests/tests_scihub/test_scilog_connector.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.5.0/.gitignore
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 bec_server-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 bec_server-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/README.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    18964 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    34791 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0    21424 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_plugins/LamNIFermatScan.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_plugins/owis_grid.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scan_server/scan_plugins/sgalil_grid.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.6.0/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6020 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25541 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_flomni_fermat_scan.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11570 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    26372 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    53971 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0   108162 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scan_server/utils.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.6.0/tests/tests_scihub/test_scilog_connector.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.6.0/.gitignore
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 bec_server-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_server-2.6.0/PKG-INFO
```

### Comparing `bec_server-2.5.0/bec_server/bec_server_utils/launch.py` & `bec_server-2.6.0/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/bec_server_utils/service_handler.py` & `bec_server-2.6.0/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/bec_server_utils/subprocess_launch.py` & `bec_server-2.6.0/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/bec_server_utils/tmux_launch.py` & `bec_server-2.6.0/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/data_processing/dap_server.py` & `bec_server-2.6.0/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/data_processing/dap_service.py` & `bec_server-2.6.0/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/data_processing/dap_service_manager.py` & `bec_server-2.6.0/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/data_processing/lmfit1d_service.py` & `bec_server-2.6.0/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/data_processing/cli/launch.py` & `bec_server-2.6.0/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/device_server/device_server.py` & `bec_server-2.6.0/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/device_server/rpc_mixin.py` & `bec_server-2.6.0/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/device_server/cli/launch.py` & `bec_server-2.6.0/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/device_server/devices/config_update_handler.py` & `bec_server-2.6.0/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/device_server/devices/device_serializer.py` & `bec_server-2.6.0/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/device_server/devices/devicemanager.py` & `bec_server-2.6.0/bec_server/device_server/devices/devicemanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,38 +9,32 @@
 import inspect
 import time
 import traceback
 from functools import reduce
 
 import numpy as np
 import ophyd
-import ophyd.sim as ops
 import ophyd_devices as opd
 from ophyd.ophydobj import OphydObject
 from ophyd.signal import EpicsSignalBase
 from typeguard import typechecked
 
 from bec_lib import (
     BECService,
     DeviceBase,
     DeviceConfigError,
     DeviceManagerBase,
     MessageEndpoints,
     bec_logger,
     messages,
+    plugin_helper,
 )
 from bec_server.device_server.devices.config_update_handler import ConfigUpdateHandler
 from bec_server.device_server.devices.device_serializer import get_device_info
 
-try:
-    from bec_plugins import devices as plugin_devices
-except ImportError:
-    plugin_devices = None
-
-
 logger = bec_logger.logger
 
 
 def rgetattr(obj, attr, *args):
     """See https://stackoverflow.com/questions/31174295/getattr-and-setattr-on-nested-objects"""
 
     def _getattr(obj, attr):
@@ -114,38 +108,16 @@
         super().initialize(bootstrap_server)
 
     def _reload_action(self) -> None:
         pass
 
     @staticmethod
     def _get_device_class(dev_type: str) -> type:
-        """
-        Return the class object from 'dev_type' string in the form '[module:][submodule:]class_name'
-        The class is looked after in ophyd devices[.module][.submodule] first, if it is not
-        present plugin_devices, ophyd, ophyd_devices.sim are searched too
-
-        Args:
-            dev_type (str): device type string
-
-        Returns:
-            type: class object
-        """
-        submodule, _, class_name = dev_type.rpartition(":")
-        if submodule:
-            submodule = f".{submodule.replace(':', '.')}"
-        for parent_module in (opd, plugin_devices, ophyd, ops):
-            try:
-                module = __import__(f"{parent_module.__name__}{submodule}", fromlist=[""])
-            except ModuleNotFoundError:
-                continue
-            else:
-                break
-        else:
-            raise TypeError(f"Unknown device class {dev_type}")
-        return getattr(module, class_name)
+        """Get the device class from the device type"""
+        return plugin_helper.get_plugin_class(dev_type, [opd, ophyd])
 
     def _load_session(self, *_args, **_kwargs):
         delayed_init = []
         if not self._is_config_valid():
             self._reset_config()
             return
```

### Comparing `bec_server-2.5.0/bec_server/file_writer/file_writer.py` & `bec_server-2.6.0/bec_server/file_writer/file_writer.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 import datetime
 import json
 import os
 import traceback
 import typing
 
 import h5py
-import xmltodict
 
-import bec_server.file_writer_plugins as fwp
-from bec_lib import MessageEndpoints, bec_logger, messages
+from bec_lib import MessageEndpoints, bec_logger, messages, plugin_helper
 
+from .default_writer import NeXus_format as default_NeXus_format
 from .merged_dicts import merge_dicts
 
 logger = bec_logger.logger
 
 
 class NeXusLayoutError(Exception):
     pass
@@ -45,115 +44,14 @@
                 if dev not in device_storage:
                     device_storage[dev] = [data.scan_segments[point][dev]]
                     continue
                 device_storage[dev].append(data.scan_segments[point][dev])
         return device_storage
 
 
-class XMLWriter:
-    @staticmethod
-    def get_type(type_string: str):
-        if type_string == "float":
-            return float
-        if type_string == "string":
-            return str
-        if type_string == "int":
-            return int
-        raise NeXusLayoutError(f"Unsupported data type {type_string}.")
-
-    def get_value(self, value, entry, source, data_type):
-        if source == "constant":
-            if data_type:
-                return self.get_type(data_type)(value)
-            return value
-        return entry
-
-    def add_group(self, container, val):
-        name = val.pop("@name")
-        group = container.create_group(name)
-        self.add_content(group, val)
-
-    def add_dataset(self, container, val):
-        name = val.pop("@name")
-        source = val.pop("@source")
-        value = val.pop("@value", None)
-        data_type = val.pop("@type", None)
-        entry = val.pop("@entry", None)
-
-        data = self.get_value(value=value, entry=entry, source=source, data_type=data_type)
-        if data is None:
-            return
-        dataset = container.create_dataset(name, data=data)
-        self.add_content(dataset, val)
-        return
-
-    def add_attribute(self, container, val):
-        name = val.pop("@name")
-        source = val.pop("@source")
-        value = val.pop("@value", None)
-        data_type = val.pop("@type", None)
-        entry = val.pop("@entry", None)
-
-        data = self.get_value(value=value, entry=entry, source=source, data_type=data_type)
-        setattr(container.attrs, name, data)
-
-    def add_hardlink(self, container, val):
-        pass
-
-    def add_softlink(self, container, val):
-        pass
-
-    def add_content(self, container, layout):
-        for key, values in layout.items():
-            if not isinstance(values, list):
-                values = [values]
-            for val in values:
-                if key == "group":
-                    self.add_group(container, val)
-                elif key == "hdf5_layout":
-                    self.add_base_entry(container, val)
-                elif key == "attribute":
-                    self.add_attribute(container, val)
-                elif key == "dataset":
-                    self.add_dataset(container, val)
-                elif key == "hardlink":
-                    self.add_hardlink(container, val)
-                elif key == "softlink":
-                    self.add_softlink(container, val)
-                else:
-                    pass
-                    # raise NeXusLayoutError()
-
-    def add_base_entry(self, container, val):
-        self.add_group(container, val["group"])
-
-
-class NeXusFileXMLWriter(FileWriter, XMLWriter):
-    def configure(self, layout_file, **kwargs):
-        self.layout_file = layout_file
-        with open(self.layout_file, "br") as f:
-            self.layout = xmltodict.parse(f)
-
-    def get_value(self, value, entry, source, data_type):
-        if source == "constant":
-            if data_type:
-                return self.get_type(data_type)(value)
-            return value
-        if source == "bec":
-            return self.data.get(entry)
-        return entry
-
-    def write(self, file_path: str, data):
-        print(f"writing file to {file_path}")
-        self.data = self._create_device_data_storage(data)
-
-        with h5py.File(file_path, "w") as file:
-            self.add_content(file, self.layout)
-
-
 class HDF5Storage:
     """
     The HDF5Storage class is a container used by the HDF5 writer plugins to store data in the correct NeXus format.
     """
 
     def __init__(self, storage_type: str = "group", data=None) -> None:
         self._storage = {}
@@ -306,15 +204,24 @@
         # NeXus needs start_time and end_time in ISO8601 format, so we have to convert it
         if data.start_time is not None:
             device_storage["start_time"] = datetime.datetime.fromtimestamp(
                 data.start_time
             ).isoformat()
         if data.end_time is not None:
             device_storage["end_time"] = datetime.datetime.fromtimestamp(data.end_time).isoformat()
-        writer_format = getattr(fwp, self.file_writer_manager.file_writer_config.get("plugin"))
+
+        requested_plugin = self.file_writer_manager.file_writer_config.get("plugin")
+        if requested_plugin == "default_NeXus_format":
+            writer_format = default_NeXus_format
+        else:
+            plugins = plugin_helper.get_file_writer_plugins()
+            if requested_plugin not in plugins:
+                logger.error(f"Plugin {requested_plugin} not found. Using default plugin.")
+                writer_format = default_NeXus_format
+
         for file_ref in data.file_references.values():
             rel_path = os.path.relpath(file_ref["path"], os.path.dirname(file_path))
             file_ref["path"] = rel_path
 
         writer_storage = writer_format(
             storage=HDF5Storage(),
             data=device_storage,
```

### Comparing `bec_server-2.5.0/bec_server/file_writer/file_writer_manager.py` & `bec_server-2.6.0/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/file_writer/merged_dicts.py` & `bec_server-2.6.0/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/file_writer/cli/launch.py` & `bec_server-2.6.0/bec_server/file_writer/cli/launch.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,14 @@
     parser.add_argument("--config", default="", help="path to the config file")
     clargs = parser.parse_args()
     config_path = clargs.config
 
     config = ServiceConfig(config_path)
 
     file_writer_manager = file_writer.FileWriterManager(config, RedisConnector)
-    file_writer_manager.file_writer.configure(
-        layout_file=os.path.abspath("./layout_cSAXS_NXsas.xml")
-    )
     try:
         event = threading.Event()
         logger.success("Started FileWriter")
         event.wait()
     except KeyboardInterrupt:
         file_writer_manager.shutdown()
```

### Comparing `bec_server-2.5.0/bec_server/file_writer_plugins/cSAXS.py` & `bec_server-2.6.0/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/file_writer_plugins/default_writer.py` & `bec_server-2.6.0/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_bundler/bec_emitter.py` & `bec_server-2.6.0/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_bundler/bluesky_emitter.py` & `bec_server-2.6.0/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_bundler/emitter.py` & `bec_server-2.6.0/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_bundler/scan_bundler.py` & `bec_server-2.6.0/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_bundler/cli/launch.py` & `bec_server-2.6.0/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/device_validation.py` & `bec_server-2.6.0/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/path_optimization.py` & `bec_server-2.6.0/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_assembler.py` & `bec_server-2.6.0/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_guard.py` & `bec_server-2.6.0/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_queue.py` & `bec_server-2.6.0/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_server.py` & `bec_server-2.6.0/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_stubs.py` & `bec_server-2.6.0/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_worker.py` & `bec_server-2.6.0/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scans.py` & `bec_server-2.6.0/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/cli/launch.py` & `bec_server-2.6.0/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_plugins/LamNIFermatScan.py` & `bec_server-2.6.0/bec_server/scan_server/scan_plugins/LamNIFermatScan.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py` & `bec_server-2.6.0/bec_server/scan_server/scan_plugins/flomni_fermat_scan.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_plugins/otf_scan.py` & `bec_server-2.6.0/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_plugins/owis_grid.py` & `bec_server-2.6.0/bec_server/scan_server/scan_plugins/owis_grid.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scan_server/scan_plugins/sgalil_grid.py` & `bec_server-2.6.0/bec_server/scan_server/scan_plugins/sgalil_grid.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scihub/repeated_timer.py` & `bec_server-2.6.0/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scihub/scihub.py` & `bec_server-2.6.0/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scihub/cli/launch.py` & `bec_server-2.6.0/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scihub/scibec/config_handler.py` & `bec_server-2.6.0/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scihub/scibec/scibec_connector.py` & `bec_server-2.6.0/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scihub/scibec/scibec_metadata_handler.py` & `bec_server-2.6.0/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/bec_server/scihub/scilog/scilog.py` & `bec_server-2.6.0/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_bec_server_utils/test_main.py` & `bec_server-2.6.0/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_bec_server_utils/test_service_handler.py` & `bec_server-2.6.0/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_bec_server_utils/test_tmux_launch.py` & `bec_server-2.6.0/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_data_processing/test_dap_cli_launch.py` & `bec_server-2.6.0/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_data_processing/test_dap_service_manager.py` & `bec_server-2.6.0/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_data_processing/test_lmfit1d_service.py` & `bec_server-2.6.0/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_device_server/conftest.py` & `bec_server-2.6.0/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_device_server/test_config_handler.py` & `bec_server-2.6.0/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_device_server/test_device_manager_ds.py` & `bec_server-2.6.0/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_device_server/test_device_serializer.py` & `bec_server-2.6.0/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_device_server/test_device_server.py` & `bec_server-2.6.0/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_device_server/test_device_server_cli_launch.py` & `bec_server-2.6.0/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_device_server/test_rpc_mixin.py` & `bec_server-2.6.0/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_file_writer/test_file_writer.py` & `bec_server-2.6.0/tests/tests_file_writer/test_file_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import h5py
 import numpy as np
 import pytest
 from test_file_writer_manager import file_writer_manager_mock
 
 from bec_lib.tests.fixtures import dm_with_devices
 from bec_server import file_writer
-from bec_server.file_writer import NexusFileWriter, NeXusFileXMLWriter
+from bec_server.file_writer import NexusFileWriter
 from bec_server.file_writer.file_writer import HDF5Storage
 from bec_server.file_writer.file_writer_manager import ScanStorage
 from bec_server.file_writer_plugins.cSAXS import NeXus_format as cSAXS_Nexus_format
 
 dir_path = os.path.dirname(file_writer.__file__)
```

### Comparing `bec_server-2.5.0/tests/tests_file_writer/test_file_writer_cli_launch.py` & `bec_server-2.6.0/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_file_writer/test_file_writer_manager.py` & `bec_server-2.6.0/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_bundler/conftest.py` & `bec_server-2.6.0/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_bundler/test_bec_emitter.py` & `bec_server-2.6.0/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_bundler/test_bluesky_emitter.py` & `bec_server-2.6.0/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_bundler/test_emitter.py` & `bec_server-2.6.0/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_bundler/test_scan_bundler.py` & `bec_server-2.6.0/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `bec_server-2.6.0/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_flomni_fermat_scan.py` & `bec_server-2.6.0/tests/tests_scan_server/test_flomni_fermat_scan.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_path_optimization.py` & `bec_server-2.6.0/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_scan_guard.py` & `bec_server-2.6.0/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_scan_server_cli_launch.py` & `bec_server-2.6.0/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_scan_server_queue.py` & `bec_server-2.6.0/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_scan_stubs.py` & `bec_server-2.6.0/tests/tests_scan_server/test_scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_scan_worker.py` & `bec_server-2.6.0/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/test_scans.py` & `bec_server-2.6.0/tests/tests_scan_server/test_scans.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scan_server/utils.py` & `bec_server-2.6.0/tests/tests_scan_server/utils.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scihub/test_repeated_timer.py` & `bec_server-2.6.0/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scihub/test_scibec_config_handler.py` & `bec_server-2.6.0/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scihub/test_scibec_connector.py` & `bec_server-2.6.0/tests/tests_scihub/test_scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scihub/test_scibec_metadata_handler.py` & `bec_server-2.6.0/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scihub/test_scihub_cli_launch.py` & `bec_server-2.6.0/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/tests/tests_scihub/test_scilog_connector.py` & `bec_server-2.6.0/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/.gitignore` & `bec_server-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_server-2.5.0/pyproject.toml` & `bec_server-2.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.5.0"
+version = "2.6.0"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
@@ -23,15 +23,14 @@
     "ophyd",
     "ophyd_devices",
     "pydantic",
     "py-scibec",
     "pyyaml",
     "python-dotenv",
     "rich",
-    "xmltodict",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
     "isort",
     "coverage",
```

### Comparing `bec_server-2.5.0/PKG-INFO` & `bec_server-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec-server
-Version: 2.5.0
+Version: 2.6.0
 Summary: BEC server
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
@@ -18,15 +18,14 @@
 Requires-Dist: ophyd
 Requires-Dist: ophyd-devices
 Requires-Dist: py-scibec
 Requires-Dist: pydantic
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: rich
-Requires-Dist: xmltodict
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-random-order; extra == 'dev'
```

