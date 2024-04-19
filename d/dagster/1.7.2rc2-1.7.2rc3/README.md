# Comparing `tmp/dagster-1.7.2rc2.tar.gz` & `tmp/dagster-1.7.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.2rc2.tar", last modified: Tue Apr 16 20:27:24 2024, max compression
+gzip compressed data, was "dagster-1.7.2rc3.tar", last modified: Thu Apr 18 21:10:34 2024, max compression
```

## Comparing `dagster-1.7.2rc2.tar` & `dagster-1.7.2rc3.tar`

### file list

```diff
@@ -1,693 +1,693 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.578915 dagster-1.7.2rc2/
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9870 2024-04-16 20:27:24.578915 dagster-1.7.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8153 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.466915 dagster-1.7.2rc2/dagster/
--rw-r--r--   0 root         (0) root         (0)    29906 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.466915 dagster-1.7.2rc2/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.466915 dagster-1.7.2rc2/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.470915 dagster-1.7.2rc2/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26898 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30542 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.470915 dagster-1.7.2rc2/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.474915 dagster-1.7.2rc2/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.478915 dagster-1.7.2rc2/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18042 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11496 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4022 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)    41251 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.482915 dagster-1.7.2rc2/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.482915 dagster-1.7.2rc2/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21047 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.482915 dagster-1.7.2rc2/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.502915 dagster-1.7.2rc2/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7827 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_check_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     7052 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5416 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6073 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.506915 dagster-1.7.2rc2/dagster/_core/definitions/asset_condition/
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_condition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21141 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_condition/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16508 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
--rw-r--r--   0 root         (0) root         (0)    26314 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)    10648 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10133 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7700 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16636 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    29917 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     6060 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6945 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6764 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)    10466 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    79909 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    13905 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    54478 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21726 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    34666 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30060 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.506915 dagster-1.7.2rc2/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    69203 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12664 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42247 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    26888 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9766 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_based_auto_materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.506915 dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5838 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7677 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     7938 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/shared_builder.py
--rw-r--r--   0 root         (0) root         (0)     4669 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)    10573 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53689 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.510915 dagster-1.7.2rc2/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    42305 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    23141 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27737 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.510915 dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3383 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    44126 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     6225 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19244 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    21859 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102142 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11017 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    27136 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    18062 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.510915 dagster-1.7.2rc2/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7635 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.514915 dagster-1.7.2rc2/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    64654 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.518915 dagster-1.7.2rc2/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    56002 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14247 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.522915 dagster-1.7.2rc2/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    17019 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40549 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11036 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    14043 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.522915 dagster-1.7.2rc2/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.522915 dagster-1.7.2rc2/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.522915 dagster-1.7.2rc2/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.526915 dagster-1.7.2rc2/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   132749 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16700 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24178 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.526915 dagster-1.7.2rc2/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     5736 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.526915 dagster-1.7.2rc2/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.530915 dagster-1.7.2rc2/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37482 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    83392 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.530915 dagster-1.7.2rc2/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.530915 dagster-1.7.2rc2/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28809 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10931 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.530915 dagster-1.7.2rc2/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.530915 dagster-1.7.2rc2/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.530915 dagster-1.7.2rc2/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.538915 dagster-1.7.2rc2/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.538915 dagster-1.7.2rc2/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.550915 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.550915 dagster-1.7.2rc2/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25656 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.550915 dagster-1.7.2rc2/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18869 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   122582 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32629 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    17131 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13903 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37454 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7236 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25146 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.554915 dagster-1.7.2rc2/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19215 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.558915 dagster-1.7.2rc2/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.558915 dagster-1.7.2rc2/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.558915 dagster-1.7.2rc2/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     2679 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/batch_asset_record_loader.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    29210 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    41795 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12112 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18369 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39110 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.462915 dagster-1.7.2rc2/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.562915 dagster-1.7.2rc2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.566915 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.566915 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.566915 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.566915 dagster-1.7.2rc2/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)      919 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41378 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9680 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    42415 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.570915 dagster-1.7.2rc2/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.578915 dagster-1.7.2rc2/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    24377 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5404 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    42615 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    12887 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    33171 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.578915 dagster-1.7.2rc2/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7622 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    36138 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.578915 dagster-1.7.2rc2/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 20:27:24.466915 dagster-1.7.2rc2/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9870 2024-04-16 20:27:24.000000 dagster-1.7.2rc2/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28041 2024-04-16 20:27:24.000000 dagster-1.7.2rc2/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 20:27:24.000000 dagster-1.7.2rc2/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-16 20:27:24.000000 dagster-1.7.2rc2/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1461 2024-04-16 20:27:24.000000 dagster-1.7.2rc2/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 20:27:24.000000 dagster-1.7.2rc2/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-04-16 20:27:24.582915 dagster-1.7.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6830 2024-04-16 20:26:55.000000 dagster-1.7.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.663172 dagster-1.7.2rc3/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9870 2024-04-18 21:10:34.663172 dagster-1.7.2rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8153 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.547171 dagster-1.7.2rc3/dagster/
+-rw-r--r--   0 root         (0) root         (0)    29906 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.547171 dagster-1.7.2rc3/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.551172 dagster-1.7.2rc3/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52040 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.551172 dagster-1.7.2rc3/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26898 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30542 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.551172 dagster-1.7.2rc3/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.555172 dagster-1.7.2rc3/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.559172 dagster-1.7.2rc3/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18116 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    41265 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.563172 dagster-1.7.2rc3/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.567172 dagster-1.7.2rc3/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21047 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.567172 dagster-1.7.2rc3/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.599172 dagster-1.7.2rc3/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7827 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_check_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     7052 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6092 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.603172 dagster-1.7.2rc3/dagster/_core/definitions/asset_condition/
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_condition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21064 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_condition/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    16508 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
+-rw-r--r--   0 root         (0) root         (0)    26314 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)    10648 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    10133 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    29917 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7444 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6764 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    10466 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    79909 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13905 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    54478 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21726 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34666 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22990 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30060 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.607172 dagster-1.7.2rc3/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    69618 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12664 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42243 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_based_auto_materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.607172 dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     7677 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     7938 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/shared_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)    10573 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    53689 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.607172 dagster-1.7.2rc3/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    42209 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57203 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27733 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.607172 dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8858 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    44126 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6209 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    21859 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   102142 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    27136 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    18062 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.607172 dagster-1.7.2rc3/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7635 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.611172 dagster-1.7.2rc3/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    64654 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.611172 dagster-1.7.2rc3/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    56002 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14247 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.615172 dagster-1.7.2rc3/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40549 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11032 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    14043 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.619172 dagster-1.7.2rc3/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.619172 dagster-1.7.2rc3/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.619172 dagster-1.7.2rc3/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.619172 dagster-1.7.2rc3/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132705 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16700 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24178 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.619172 dagster-1.7.2rc3/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     5736 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.619172 dagster-1.7.2rc3/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.623172 dagster-1.7.2rc3/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37482 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    83392 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.623172 dagster-1.7.2rc3/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.623172 dagster-1.7.2rc3/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28809 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.623172 dagster-1.7.2rc3/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.623172 dagster-1.7.2rc3/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.623172 dagster-1.7.2rc3/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.627172 dagster-1.7.2rc3/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.627172 dagster-1.7.2rc3/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.639172 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.639172 dagster-1.7.2rc3/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25652 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.639172 dagster-1.7.2rc3/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18869 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   122582 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.639172 dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.639172 dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    32629 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.639172 dagster-1.7.2rc3/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    17398 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.643172 dagster-1.7.2rc3/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37611 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.643172 dagster-1.7.2rc3/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.643172 dagster-1.7.2rc3/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.643172 dagster-1.7.2rc3/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7236 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25146 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.643172 dagster-1.7.2rc3/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.643172 dagster-1.7.2rc3/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19215 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.643172 dagster-1.7.2rc3/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.647172 dagster-1.7.2rc3/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.647172 dagster-1.7.2rc3/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/batch_asset_record_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29210 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.647172 dagster-1.7.2rc3/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    41795 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.647172 dagster-1.7.2rc3/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12112 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18369 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39110 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.543172 dagster-1.7.2rc3/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.651172 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    60914 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_model/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41378 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.655172 dagster-1.7.2rc3/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9680 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    42415 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.659172 dagster-1.7.2rc3/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.659172 dagster-1.7.2rc3/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.663172 dagster-1.7.2rc3/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    24377 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    42615 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    12887 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    33171 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.663172 dagster-1.7.2rc3/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7622 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36138 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.663172 dagster-1.7.2rc3/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 21:10:34.547171 dagster-1.7.2rc3/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9870 2024-04-18 21:10:34.000000 dagster-1.7.2rc3/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28024 2024-04-18 21:10:34.000000 dagster-1.7.2rc3/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 21:10:34.000000 dagster-1.7.2rc3/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-18 21:10:34.000000 dagster-1.7.2rc3/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-04-18 21:10:34.000000 dagster-1.7.2rc3/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-18 21:10:34.000000 dagster-1.7.2rc3/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-04-18 21:10:34.663172 dagster-1.7.2rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6830 2024-04-18 21:10:09.000000 dagster-1.7.2rc3/setup.py
```

### Comparing `dagster-1.7.2rc2/COPYING` & `dagster-1.7.2rc3/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/LICENSE` & `dagster-1.7.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/MANIFEST.in` & `dagster-1.7.2rc3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/PKG-INFO` & `dagster-1.7.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.2rc2/README.md` & `dagster-1.7.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/__init__.py` & `dagster-1.7.2rc3/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_annotations.py` & `dagster-1.7.2rc3/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/get_server_id.py` & `dagster-1.7.2rc3/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/list_repositories.py` & `dagster-1.7.2rc3/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/notebook_data.py` & `dagster-1.7.2rc3/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.2rc3/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/snapshot_job.py` & `dagster-1.7.2rc3/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/snapshot_partition.py` & `dagster-1.7.2rc3/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/snapshot_repository.py` & `dagster-1.7.2rc3/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/snapshot_schedule.py` & `dagster-1.7.2rc3/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_api/snapshot_sensor.py` & `dagster-1.7.2rc3/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_check/README.md` & `dagster-1.7.2rc3/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_check/__init__.py` & `dagster-1.7.2rc3/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/__init__.py` & `dagster-1.7.2rc3/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/api.py` & `dagster-1.7.2rc3/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/asset.py` & `dagster-1.7.2rc3/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/code_server.py` & `dagster-1.7.2rc3/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/config_scaffolder.py` & `dagster-1.7.2rc3/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/debug.py` & `dagster-1.7.2rc3/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/dev.py` & `dagster-1.7.2rc3/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/instance.py` & `dagster-1.7.2rc3/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/job.py` & `dagster-1.7.2rc3/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/load_handle.py` & `dagster-1.7.2rc3/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/project.py` & `dagster-1.7.2rc3/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/run.py` & `dagster-1.7.2rc3/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/schedule.py` & `dagster-1.7.2rc3/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/sensor.py` & `dagster-1.7.2rc3/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/utils.py` & `dagster-1.7.2rc3/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.2rc3/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/__init__.py` & `dagster-1.7.2rc3/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/config_schema.py` & `dagster-1.7.2rc3/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/config_type.py` & `dagster-1.7.2rc3/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/errors.py` & `dagster-1.7.2rc3/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/evaluate_value_result.py` & `dagster-1.7.2rc3/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/field.py` & `dagster-1.7.2rc3/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/field_utils.py` & `dagster-1.7.2rc3/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/post_process.py` & `dagster-1.7.2rc3/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/primitive_mapping.py` & `dagster-1.7.2rc3/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/config.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Mapping,
     Optional,
     Set,
     Type,
     cast,
 )
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from typing_extensions import TypeVar
 
 import dagster._check as check
 from dagster import (
     Field as DagsterField,
     Shape,
 )
@@ -29,27 +29,27 @@
 )
 from dagster._core.errors import (
     DagsterInvalidConfigDefinitionError,
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidPythonicConfigDefinitionError,
 )
-from dagster._utils.cached_method import CACHED_METHOD_FIELD_SUFFIX
-
-from .attach_other_object_to_context import (
-    IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
-)
-from .conversion_utils import _convert_pydantic_field, safe_is_subclass
-from .pydantic_compat_layer import (
+from dagster._model.pydantic_compat_layer import (
     USING_PYDANTIC_2,
     ModelFieldCompat,
     PydanticUndefined,
     model_config,
     model_fields,
 )
+from dagster._utils.cached_method import CACHED_METHOD_FIELD_SUFFIX
+
+from .attach_other_object_to_context import (
+    IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
+)
+from .conversion_utils import _convert_pydantic_field, safe_is_subclass
 from .type_check_utils import is_literal
 from .typing_utils import BaseConfigMeta
 
 try:
     from functools import cached_property  # type: ignore  # (py37 compat)
 except ImportError:
 
@@ -81,27 +81,27 @@
 
 class MakeConfigCacheable(BaseModel):
     """This class centralizes and implements all the chicanery we need in order
     to support caching decorators. If we decide this is a bad idea we can remove it
     all in one go.
     """
 
-    # Pydantic config for this class
-    # Cannot use kwargs for base class as this is not support for pydnatic<1.8
-    class Config:
-        # Various pydantic model config (https://docs.pydantic.dev/usage/model_config/)
-        # Necessary to allow for caching decorators
-        arbitrary_types_allowed = True
-        # Avoid pydantic reading a cached property class as part of the schema
-        if USING_PYDANTIC_2:
-            ignored_types = (cached_property,)
-        else:
+    # - Frozen, to avoid complexity caused by mutation.
+    # - arbitrary_types_allowed, to allow non-model class params to be validated with isinstance.
+    # - Avoid pydantic reading a cached property class as part of the schema.
+    if USING_PYDANTIC_2:
+        model_config = ConfigDict(  # type: ignore
+            frozen=True, arbitrary_types_allowed=True, ignored_types=(cached_property,)
+        )
+    else:
+
+        class Config:
+            frozen = True
+            arbitrary_types_allowed = True
             keep_untouched = (cached_property,)
-        # Ensure the class is serializable, for caching purposes
-        frozen = True
 
     def __setattr__(self, name: str, value: Any):
         from .resource import ConfigurableResourceFactory
 
         # This is a hack to allow us to set attributes on the class that are not part of the
         # config schema. Pydantic will normally raise an error if you try to set an attribute
         # that is not part of the schema.
@@ -396,16 +396,20 @@
             )
         )
 
     """
 
     # Pydantic config for this class
     # Cannot use kwargs for base class as this is not support for pydantic<1.8
-    class Config:
-        extra = "allow"
+    if USING_PYDANTIC_2:
+        model_config = ConfigDict(extra="allow")  # type: ignore
+    else:
+
+        class Config:
+            extra = "allow"
 
 
 def infer_schema_from_config_class(
     model_cls: Type["Config"],
     description: Optional[str] = None,
     fields_to_omit: Optional[Set[str]] = None,
 ) -> DagsterField:
```

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 import dagster._check as check
 from dagster import Field, Selector
 from dagster._config.field_utils import (
     FIELD_NO_DEFAULT_PROVIDED,
     Map,
     convert_potential_field,
 )
+from dagster._model.pydantic_compat_layer import ModelFieldCompat, PydanticUndefined, model_fields
 
-from .pydantic_compat_layer import ModelFieldCompat, PydanticUndefined, model_fields
 from .type_check_utils import is_optional, safe_is_subclass
 
 
 # This is from https://github.com/dagster-io/dagster/pull/11470
 def _apply_defaults_to_schema_field(field: Field, additional_default_values: Any) -> Field:
     # This work by validating the top-level config and then
     # just setting it at that top-level field. Config fields
```

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/pydantic_compat_layer.py` & `dagster-1.7.2rc3/dagster/_model/pydantic_compat_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,14 @@
     Optional,
     Type,
 )
 
 import pydantic
 from pydantic import BaseModel
 
-from .attach_other_object_to_context import (
-    IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
-)
-
 USING_PYDANTIC_1 = int(pydantic.__version__.split(".")[0]) == 1
 USING_PYDANTIC_2 = int(pydantic.__version__.split(".")[0]) >= 2
 
 PydanticUndefined = None
 if USING_PYDANTIC_2:
     from pydantic_core import PydanticUndefined as _PydanticUndefined  # type: ignore
```

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 from dagster._config.validate import validate_config
 from dagster._core.definitions.definition_config_schema import (
     ConfiguredDefinitionConfigSchema,
     DefinitionConfigSchema,
 )
 from dagster._core.errors import DagsterInvalidConfigError
 from dagster._core.execution.context.init import InitResourceContext, build_init_resource_context
+from dagster._model.pydantic_compat_layer import (
+    model_fields,
+)
 from dagster._utils.cached_method import cached_method
 
 from .attach_other_object_to_context import (
     IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
 )
-from .pydantic_compat_layer import (
-    model_fields,
-)
 from .type_check_utils import is_optional
 
 try:
     from functools import cached_property  # type: ignore  # (py37 compat)
 except ImportError:
 
     class cached_property:
```

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.2rc3/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/snap.py` & `dagster-1.7.2rc3/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/source.py` & `dagster-1.7.2rc3/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/stack.py` & `dagster-1.7.2rc3/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/traversal_context.py` & `dagster-1.7.2rc3/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/type_printer.py` & `dagster-1.7.2rc3/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_config/validate.py` & `dagster-1.7.2rc3/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.2rc3/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/assets.py` & `dagster-1.7.2rc3/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/code_pointer.py` & `dagster-1.7.2rc3/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/container_context/config.py` & `dagster-1.7.2rc3/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/debug.py` & `dagster-1.7.2rc3/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/decorator_utils.py` & `dagster-1.7.2rc3/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/__init__.py` & `dagster-1.7.2rc3/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_check_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_check_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,12 +130,13 @@
         group_name=asset_def.group_names_by_key.get(asset_def.key),
         partitions_def=asset_def.partitions_def,
         check_specs=check_specs,
         description=asset_def.descriptions_by_key.get(asset_def.key),
         ins={name: AssetIn(key) for name, key in asset_def.keys_by_input_name.items()},
         resource_defs=asset_def.resource_defs,
         metadata=asset_def.metadata_by_key.get(asset_def.key),
+        tags=None,
         freshness_policy=asset_def.freshness_policies_by_key.get(asset_def.key),
         auto_materialize_policy=asset_def.auto_materialize_policies_by_key.get(asset_def.key),
         backfill_policy=asset_def.backfill_policy,
         config=None,  # gets config from asset_def.op
     )
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_condition/asset_condition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_condition/asset_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,17 +275,14 @@
 
             # At least one parent is newer and no parent is missing.
             my_policy = AutoMaterializePolicy(
                 asset_condition = AssetCondition.parent_newer() & ~AssetCondition.parent_missing()
             )
     """
 
-    class Config:
-        keep_untouched = (functools.cached_property,)
-
     @property
     def unique_id(self) -> str:
         parts = [
             self.__class__.__name__,
             *[child.unique_id for child in self.children],
         ]
         return hashlib.md5("".join(parts).encode()).hexdigest()
@@ -378,15 +375,15 @@
 
         return RuleCondition(rule=AutoMaterializeRule.skip_on_parent_missing())
 
     @staticmethod
     def updated_since_cron(cron_schedule: str, timezone: str = "UTC") -> "AssetCondition":
         """Returns an AssetCondition that is true for an asset partition when it has been updated
         since the latest tick of the given cron schedule. For partitioned assets with a time
-        component, this can only be true for the the most recent partition.
+        component, this can only be true for the most recent partition.
         """
         from ..auto_materialize_rule import AutoMaterializeRule
 
         return ~RuleCondition(rule=AutoMaterializeRule.materialize_on_cron(cron_schedule, timezone))
 
     @staticmethod
     def parents_updated_since_cron(cron_schedule: str, timezone: str = "UTC") -> "AssetCondition":
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_daemon_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_graph_differ.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         )
 
     def _compare_base_and_branch_assets(self, asset_key: "AssetKey") -> Sequence[ChangeReason]:
         """Computes the diff between a branch deployment asset and the
         corresponding base deployment asset.
         """
         if self.base_asset_graph is None:
-            # if the base asset graph is None, it is because the the asset graph in the branch deployment
+            # if the base asset graph is None, it is because the asset graph in the branch deployment
             # is new and doesn't exist in the base deployment. Thus all assets are new.
             return [ChangeReason.NEW]
 
         if asset_key not in self.base_asset_graph.all_asset_keys:
             return [ChangeReason.NEW]
 
         branch_asset = self.branch_asset_graph.get(asset_key)
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_in.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_job.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_key.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_out.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.2rc3/dagster/_core/definitions/asset_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/assets.py` & `dagster-1.7.2rc3/dagster/_core/definitions/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.2rc3/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.2rc3/dagster/_core/definitions/base_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.2rc3/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/composition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/config.py` & `dagster-1.7.2rc3/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/configurable.py` & `dagster-1.7.2rc3/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/data_time.py` & `dagster-1.7.2rc3/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/data_version.py` & `dagster-1.7.2rc3/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1056,34 +1056,37 @@
     description: Optional[str] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     config: Optional[Union[ConfigMapping, Mapping[str, Any]]] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     group_name: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     metadata: Optional[RawMetadataMapping] = ...,
+    tags: Optional[Mapping[str, str]] = ...,
     freshness_policy: Optional[FreshnessPolicy] = ...,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = ...,
     backfill_policy: Optional[BackfillPolicy] = ...,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = ...,
     check_specs: Optional[Sequence[AssetCheckSpec]] = None,
     key: Optional[CoercibleToAssetKey] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]: ...
 
 
+@experimental_param(param="tags")
 def graph_asset(
     compose_fn: Optional[Callable] = None,
     *,
     name: Optional[str] = None,
     description: Optional[str] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     config: Optional[Union[ConfigMapping, Mapping[str, Any]]] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     group_name: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     metadata: Optional[RawMetadataMapping] = None,
+    tags: Optional[Mapping[str, str]] = None,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
     backfill_policy: Optional[BackfillPolicy] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     check_specs: Optional[Sequence[AssetCheckSpec]] = None,
     key: Optional[CoercibleToAssetKey] = None,
 ) -> Union[AssetsDefinition, Callable[[Callable[..., Any]], AssetsDefinition]]:
@@ -1120,14 +1123,16 @@
             contains letters, numbers, and underscores) and may not contain Python reserved keywords.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. If
             not provided, the name "default" is used.
         partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
             compose the asset.
         metadata (Optional[RawMetadataMapping]): Dictionary of metadata to be associated with
             the asset.
+        tags (Optional[Mapping[str, str]]): Tags for filtering and organizing. These tags are not
+            attached to runs of the asset.
         freshness_policy (Optional[FreshnessPolicy]): A constraint telling Dagster how often this asset is
             intended to be updated with respect to its root data.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): The AutoMaterializePolicy to use
             for this asset.
         backfill_policy (Optional[BackfillPolicy]): The BackfillPolicy to use for this asset.
         key (Optional[CoeercibleToAssetKey]): The key for this asset. If provided, cannot specify key_prefix or name.
 
@@ -1153,14 +1158,15 @@
             description=description,
             ins=ins,
             config=config,
             key_prefix=key_prefix,
             group_name=group_name,
             partitions_def=partitions_def,
             metadata=metadata,
+            tags=tags,
             freshness_policy=freshness_policy,
             auto_materialize_policy=auto_materialize_policy,
             backfill_policy=backfill_policy,
             resource_defs=resource_defs,
             check_specs=check_specs,
             key=key,
         )
@@ -1171,14 +1177,15 @@
             description=description,
             ins=ins,
             config=config,
             key_prefix=key_prefix,
             group_name=group_name,
             partitions_def=partitions_def,
             metadata=metadata,
+            tags=tags,
             freshness_policy=freshness_policy,
             auto_materialize_policy=auto_materialize_policy,
             backfill_policy=backfill_policy,
             resource_defs=resource_defs,
             check_specs=check_specs,
             key=key,
         )
@@ -1191,14 +1198,15 @@
     description: Optional[str],
     ins: Optional[Mapping[str, AssetIn]],
     config: Optional[Union[ConfigMapping, Mapping[str, Any]]],
     key_prefix: Optional[CoercibleToAssetKeyPrefix],
     group_name: Optional[str],
     partitions_def: Optional[PartitionsDefinition],
     metadata: Optional[RawMetadataMapping],
+    tags: Optional[Mapping[str, str]],
     freshness_policy: Optional[FreshnessPolicy],
     auto_materialize_policy: Optional[AutoMaterializePolicy],
     backfill_policy: Optional[BackfillPolicy],
     resource_defs: Optional[Mapping[str, ResourceDefinition]],
     check_specs: Optional[Sequence[AssetCheckSpec]],
     key: Optional[CoercibleToAssetKey],
 ) -> AssetsDefinition:
@@ -1242,14 +1250,15 @@
         op_graph,
         keys_by_input_name=keys_by_input_name,
         keys_by_output_name={"result": out_asset_key},
         partitions_def=partitions_def,
         partition_mappings=partition_mappings if partition_mappings else None,
         group_name=group_name,
         metadata_by_output_name={"result": metadata} if metadata else None,
+        tags_by_output_name={"result": tags} if tags else None,
         freshness_policies_by_output_name=(
             {"result": freshness_policy} if freshness_policy else None
         ),
         auto_materialize_policies_by_output_name=(
             {"result": auto_materialize_policy} if auto_materialize_policy else None
         ),
         backfill_policy=backfill_policy,
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.2rc3/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.2rc3/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.2rc3/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/dependency.py` & `dagster-1.7.2rc3/dagster/_core/definitions/dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1031,15 +1031,15 @@
             for output_handle in output_handle_list
         ]
 
     def input_to_upstream_outputs_for_node(
         self, node_name: str
     ) -> Mapping[NodeInput, Sequence[NodeOutput]]:
         """Returns a Dict[NodeInput, List[NodeOutput]] that encodes
-        where all the the inputs are sourced from upstream. Usually the
+        where all the inputs are sourced from upstream. Usually the
         List[NodeOutput] will be a list of one, except for the
         multi-dependency case.
         """
         check.str_param(node_name, "node_name")
         return self._node_input_index[node_name]
 
     def output_to_downstream_inputs_for_node(
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/events.py` & `dagster-1.7.2rc3/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/external_asset.py` & `dagster-1.7.2rc3/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/last_update.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/last_update.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/sensor.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/shared_builder.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/shared_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/time_partition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/time_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_checks/utils.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_checks/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.2rc3/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/inference.py` & `dagster-1.7.2rc3/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/input.py` & `dagster-1.7.2rc3/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.2rc3/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/job_base.py` & `dagster-1.7.2rc3/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/job_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.2rc3/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.2rc3/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.2rc3/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/materialize.py` & `dagster-1.7.2rc3/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.2rc3/dagster/_core/definitions/metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,22 +13,22 @@
     Optional,
     Sequence,
     Type,
     Union,
     cast,
 )
 
-from pydantic import BaseModel
 from typing_extensions import Self, TypeAlias, TypeVar
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._annotations import PublicAttr, deprecated, deprecated_param, experimental, public
 from dagster._core.definitions.asset_key import AssetKey
 from dagster._core.errors import DagsterInvalidMetadata
+from dagster._model import DagsterModel
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import (
     FieldSerializer,
     PackableValue,
     UnpackContext,
     WhitelistMap,
     pack_value,
@@ -1217,28 +1217,26 @@
 
     @property
     def value(self):
         """Alias of `entry_data`."""
         return self.entry_data
 
 
-T_NamespacedMetadataEntries = TypeVar(
-    "T_NamespacedMetadataEntries", bound="NamespacedMetadataEntries"
-)
+T_NamespacedMetadataSet = TypeVar("T_NamespacedMetadataSet", bound="NamespacedMetadataSet")
 
 
-class NamespacedMetadataEntries(ABC, BaseModel, frozen=True):
+class NamespacedMetadataSet(ABC, DagsterModel):
     """Extend this class to define a set of metadata fields in the same namespace.
 
     Supports splatting to a dictionary that can be placed inside a metadata argument along with
     other dictionary-structured metadata.
 
     .. code-block:: python
 
-        my_metadata: NamespacedMetadataEntries = ...
+        my_metadata: NamespacedMetadataSet = ...
         return MaterializeResult(metadata={**my_metadata, ...})
     """
 
     @classmethod
     @abstractmethod
     def namespace(cls) -> str:
         raise NotImplementedError()
@@ -1261,30 +1259,30 @@
 
     def __getitem__(self, key: str) -> Any:
         # getattr returns the pydantic property on the subclass
         return getattr(self, self._strip_namespace_from_key(key))
 
     @classmethod
     def extract(
-        cls: Type[T_NamespacedMetadataEntries], metadata: Mapping[str, Any]
-    ) -> T_NamespacedMetadataEntries:
+        cls: Type[T_NamespacedMetadataSet], metadata: Mapping[str, Any]
+    ) -> T_NamespacedMetadataSet:
         """Extracts entries from the provided metadata dictionary into an instance of this class.
 
         Ignores any entries in the metadata dictionary whose keys don't correspond to fields on this
         class.
 
         In general, the following should always pass:
 
         .. code-block:: python
 
-            class MyMetadataEntries(NamedspacedMetadataEntries):
+            class MyMetadataSet(NamedspacedMetadataSet):
                 ...
 
-            metadata_entries: MyMetadataEntries  = ...
-            assert MyMetadataEntries.extract(dict(metadata_entries)) == metadata_entries
+            metadata: MyMetadataSet  = ...
+            assert MyMetadataSet.extract(dict(metadata)) == metadata
 
         Args:
             metadata (Mapping[str, Any]): A dictionary of metadata entries.
         """
         kwargs = {}
         for namespaced_key, value in metadata.items():
             splits = namespaced_key.split("/")
@@ -1292,15 +1290,15 @@
                 namespace, key = splits
                 if namespace == cls.namespace() and key in cls.__fields__:
                     kwargs[key] = value.value if isinstance(value, MetadataValue) else value
 
         return cls(**kwargs)
 
 
-class TableMetadataEntries(NamespacedMetadataEntries, frozen=True):
+class TableMetadataSet(NamespacedMetadataSet):
     """Metadata entries that apply to definitions, observations, or materializations of assets that
     are tables.
 
     Args:
         column_schema (Optional[TableSchema]): The schema of the columns in the table.
         column_lineage (Optional[TableColumnLineage]): The lineage of column inputs to column
             outputs for the table.
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.2rc3/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.2rc3/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/node_container.py` & `dagster-1.7.2rc3/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/node_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/observe.py` & `dagster-1.7.2rc3/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/op_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.2rc3/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/op_selection.py` & `dagster-1.7.2rc3/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/output.py` & `dagster-1.7.2rc3/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/partition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.2rc3/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.2rc3/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.2rc3/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/policy.py` & `dagster-1.7.2rc3/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.2rc3/dagster/_core/definitions/reconstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,15 @@
     return ReconstructableJob(
         repository=ReconstructableRepository(pointer),  # creates ephemeral repo
         job_name=job_def.name,
     )
 
 
 def bootstrap_standalone_recon_job(pointer: CodePointer) -> ReconstructableJob:
-    # So this actually straps the the job for the sole
+    # So this actually straps the job for the sole
     # purpose of getting the job name. If we changed ReconstructableJob
     # to get the job on demand in order to get name, we could avoid this.
     job_def = job_def_from_pointer(pointer)
     return ReconstructableJob(
         repository=ReconstructableRepository(pointer),  # creates ephemeral repo
         job_name=job_def.name,
     )
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.2rc3/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.2rc3/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.2rc3/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.2rc3/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.2rc3/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.2rc3/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/result.py` & `dagster-1.7.2rc3/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/run_config.py` & `dagster-1.7.2rc3/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.2rc3/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/run_request.py` & `dagster-1.7.2rc3/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/schema_change_checks.py` & `dagster-1.7.2rc3/dagster/_core/definitions/schema_change_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from .asset_check_result import AssetCheckResult
 from .asset_check_spec import AssetCheckSeverity, AssetCheckSpec
 from .asset_checks import AssetChecksDefinition
 from .asset_key import AssetKey, CoercibleToAssetKey
 from .assets import AssetsDefinition, SourceAsset
 from .decorators.asset_check_decorator import multi_asset_check
 from .events import AssetMaterialization
-from .metadata import TableColumn, TableMetadataEntries, TableSchema
+from .metadata import TableColumn, TableMetadataSet, TableSchema
 
 
 @experimental
 def build_column_schema_change_checks(
     *,
     assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
     severity: AssetCheckSeverity = AssetCheckSeverity.WARN,
 ) -> Sequence[AssetChecksDefinition]:
-    """Returns asset checks that pass if the the column schema of the asset's latest materialization
+    """Returns asset checks that pass if the column schema of the asset's latest materialization
     is the same as the column schema of the asset's previous materialization.
 
     Args:
         assets (Sequence[Union[AssetKey, str, AssetsDefinition, SourceAsset]]): The assets to create
             asset checks for.
         severity (AssetCheckSeverity): The severity if the check fails. Defaults to WARN.
 
@@ -65,16 +65,16 @@
             else:
                 record, prev_record = materialization_records
                 metadata = cast(AssetMaterialization, record.asset_materialization).metadata
                 prev_metadata = cast(
                     AssetMaterialization, prev_record.asset_materialization
                 ).metadata
 
-                column_schema = TableMetadataEntries.extract(metadata).column_schema
-                prev_column_schema = TableMetadataEntries.extract(prev_metadata).column_schema
+                column_schema = TableMetadataSet.extract(metadata).column_schema
+                prev_column_schema = TableMetadataSet.extract(prev_metadata).column_schema
                 if column_schema is None:
                     yield AssetCheckResult(
                         passed=False,
                         description="Latest materialization has no column schema metadata",
                     )
                 if prev_column_schema is None:
                     yield AssetCheckResult(
```

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.2rc3/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/selector.py` & `dagster-1.7.2rc3/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/source_asset.py` & `dagster-1.7.2rc3/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.2rc3/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/target.py` & `dagster-1.7.2rc3/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.2rc3/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.2rc3/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.2rc3/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/utils.py` & `dagster-1.7.2rc3/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.2rc3/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/errors.py` & `dagster-1.7.2rc3/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/event_api.py` & `dagster-1.7.2rc3/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/events/__init__.py` & `dagster-1.7.2rc3/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/events/log.py` & `dagster-1.7.2rc3/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/events/utils.py` & `dagster-1.7.2rc3/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/api.py` & `dagster-1.7.2rc3/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.2rc3/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/backfill.py` & `dagster-1.7.2rc3/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/build_resources.py` & `dagster-1.7.2rc3/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/compute_logs.py` & `dagster-1.7.2rc3/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/compute.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/hook.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/init.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/input.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/invocation.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/logger.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/output.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context/system.py` & `dagster-1.7.2rc3/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.2rc3/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.2rc3/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.2rc3/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/execution_result.py` & `dagster-1.7.2rc3/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/host_mode.py` & `dagster-1.7.2rc3/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/job_backfill.py` & `dagster-1.7.2rc3/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.2rc3/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/memoization.py` & `dagster-1.7.2rc3/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/active.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/compute.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/external_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 def external_instance_from_step_run_ref(
     step_run_ref: StepRunRef, event_listener_fn: Optional[Callable[[EventLogEntry], object]] = None
 ) -> DagsterInstance:
     """Create an ephemeral DagsterInstance that is suitable for executing steps that are specified
     by a StepRunRef by pre-populating certain values.
 
     Args:
-        step_run_ref (StepRunRef): The reference to the the step that we want to execute
+        step_run_ref (StepRunRef): The reference to the step that we want to execute
         event_listener_fn (EventLogEntry -> Any): A function that handles each individual
             EventLogEntry created on this instance. Generally used to send these events back to
             the host instance.
 
     Returns:
         DagsterInstance: A DagsterInstance that can be used to execute an external step.
     """
```

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/handle.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/objects.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/plan.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/state.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/step.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/plan/utils.py` & `dagster-1.7.2rc3/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.2rc3/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.2rc3/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/resources_init.py` & `dagster-1.7.2rc3/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/retries.py` & `dagster-1.7.2rc3/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.2rc3/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/stats.py` & `dagster-1.7.2rc3/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.2rc3/dagster/_core/execution/submit_asset_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/tags.py` & `dagster-1.7.2rc3/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.2rc3/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.2rc3/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/execution/with_resources.py` & `dagster-1.7.2rc3/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/executor/base.py` & `dagster-1.7.2rc3/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.2rc3/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/executor/in_process.py` & `dagster-1.7.2rc3/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/executor/init.py` & `dagster-1.7.2rc3/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/executor/multiprocess.py` & `dagster-1.7.2rc3/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.2rc3/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.2rc3/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/instance/__init__.py` & `dagster-1.7.2rc3/dagster/_core/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2885,33 +2885,32 @@
             InstigatorStatus,
             SensorInstigatorData,
         )
 
         stored_state = self.get_instigator_state(
             external_sensor.get_external_origin_id(), external_sensor.selector_id
         )
-        new_instigator_data = SensorInstigatorData(
-            min_interval=external_sensor.min_interval_seconds,
-            sensor_type=external_sensor.sensor_type,
-        )
         new_status = InstigatorStatus.DECLARED_IN_CODE
 
         if not stored_state:
+            new_instigator_data = SensorInstigatorData(
+                min_interval=external_sensor.min_interval_seconds,
+                sensor_type=external_sensor.sensor_type,
+            )
+
             reset_state = self.add_instigator_state(
                 state=InstigatorState(
                     external_sensor.get_external_origin(),
                     InstigatorType.SENSOR,
                     new_status,
                     new_instigator_data,
                 )
             )
         else:
-            reset_state = self.update_instigator_state(
-                state=stored_state.with_status(new_status).with_data(new_instigator_data)
-            )
+            reset_state = self.update_instigator_state(state=stored_state.with_status(new_status))
 
         return reset_state
 
     @traced
     def all_instigator_state(
         self,
         repository_origin_id: Optional[str] = None,
```

### Comparing `dagster-1.7.2rc2/dagster/_core/instance/config.py` & `dagster-1.7.2rc3/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/instance/ref.py` & `dagster-1.7.2rc3/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/instance_for_test.py` & `dagster-1.7.2rc3/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/launcher/base.py` & `dagster-1.7.2rc3/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.2rc3/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.2rc3/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/log_manager.py` & `dagster-1.7.2rc3/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/nux.py` & `dagster-1.7.2rc3/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.2rc3/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/origin.py` & `dagster-1.7.2rc3/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/pipes/client.py` & `dagster-1.7.2rc3/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/pipes/context.py` & `dagster-1.7.2rc3/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/pipes/subprocess.py` & `dagster-1.7.2rc3/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/pipes/utils.py` & `dagster-1.7.2rc3/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/external.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/handle.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/historical.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/origin.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/remote_representation/represented.py` & `dagster-1.7.2rc3/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/run_coordinator/base.py` & `dagster-1.7.2rc3/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.2rc3/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.2rc3/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/scheduler/__init__.py` & `dagster-1.7.2rc3/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/scheduler/execution.py` & `dagster-1.7.2rc3/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/scheduler/instigation.py` & `dagster-1.7.2rc3/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.2rc3/dagster/_core/scheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,32 +167,33 @@
         """
         check.inst_param(instance, "instance", DagsterInstance)
         check.inst_param(external_schedule, "external_schedule", ExternalSchedule)
 
         stored_state = instance.get_instigator_state(
             external_schedule.get_external_origin_id(), external_schedule.selector_id
         )
-        new_instigator_data = ScheduleInstigatorData(
-            external_schedule.cron_schedule,
-            start_timestamp=None,
-        )
+
         new_status = InstigatorStatus.DECLARED_IN_CODE
 
         if not stored_state:
+            new_instigator_data = ScheduleInstigatorData(
+                external_schedule.cron_schedule,
+                start_timestamp=None,
+            )
             reset_state = instance.add_instigator_state(
                 state=InstigatorState(
                     external_schedule.get_external_origin(),
                     InstigatorType.SCHEDULE,
                     new_status,
                     new_instigator_data,
                 )
             )
         else:
             reset_state = instance.update_instigator_state(
-                state=stored_state.with_status(new_status).with_data(new_instigator_data)
+                state=stored_state.with_status(new_status)
             )
 
         return reset_state
 
     @abc.abstractmethod
     def debug_info(self) -> str:
         """Returns debug information about the scheduler."""
```

### Comparing `dagster-1.7.2rc2/dagster/_core/secrets/env_file.py` & `dagster-1.7.2rc3/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/selector/subset_selector.py` & `dagster-1.7.2rc3/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/__init__.py` & `dagster-1.7.2rc3/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/dagster_types.py` & `dagster-1.7.2rc3/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.2rc3/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.2rc3/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.2rc3/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/mode.py` & `dagster-1.7.2rc3/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/node.py` & `dagster-1.7.2rc3/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.2rc3/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.2rc3/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/README.md` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/env.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.2rc3/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.2rc3/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.2rc3/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/base_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/config.py` & `dagster-1.7.2rc3/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/dagster_run.py` & `dagster-1.7.2rc3/dagster/_core/storage/dagster_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     DagsterRunStatus.FAILURE,
     DagsterRunStatus.CANCELED,
 ]
 
 # Run statuses for runs that can be safely canceled.
 # Does not include the other unfinished statuses for the following reasons:
 # STARTING: Control has been ceded to the run worker, which will eventually move the run to a STARTED.
-# NOT_STARTED: Mostly replaced with STARTING. Runs are only here in the the brief window between
+# NOT_STARTED: Mostly replaced with STARTING. Runs are only here in the brief window between
 # creating the run and launching or enqueueing it.
 CANCELABLE_RUN_STATUSES = [DagsterRunStatus.STARTED, DagsterRunStatus.QUEUED]
 
 
 @whitelist_for_serdes(storage_name="PipelineRunStatsSnapshot")
 class DagsterRunStatsSnapshot(
     NamedTuple(
```

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/base.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,41 +44,47 @@
     def has_run_id(self, run_id: str) -> bool:
         run_id = check.str_param(run_id, "run_id")
         with self._dict_lock:
             _has_run_id = run_id in self._run_id_to_watcher_dict
         return _has_run_id
 
     def watch_run(
-        self, run_id: str, cursor: Optional[str], callback: Callable[[EventLogEntry, str], None]
-    ):
+        self,
+        run_id: str,
+        cursor: Optional[str],
+        callback: Callable[[EventLogEntry, str], None],
+    ) -> None:
         run_id = check.str_param(run_id, "run_id")
         cursor = check.opt_str_param(cursor, "cursor")
         callback = check.callable_param(callback, "callback")
+        check.invariant(not self._disposed, "Attempted to watch_run after close")
+
         with self._dict_lock:
             if run_id not in self._run_id_to_watcher_dict:
                 self._run_id_to_watcher_dict[run_id] = SqlPollingRunIdEventWatcherThread(
                     self._event_log_storage, run_id
                 )
                 self._run_id_to_watcher_dict[run_id].daemon = True
                 self._run_id_to_watcher_dict[run_id].start()
             self._run_id_to_watcher_dict[run_id].add_callback(cursor, callback)
 
-    def unwatch_run(self, run_id: str, handler: Callable[[EventLogEntry, str], None]):
+    def unwatch_run(
+        self,
+        run_id: str,
+        handler: Callable[[EventLogEntry, str], None],
+    ) -> None:
         run_id = check.str_param(run_id, "run_id")
         handler = check.callable_param(handler, "handler")
         with self._dict_lock:
             if run_id in self._run_id_to_watcher_dict:
                 self._run_id_to_watcher_dict[run_id].remove_callback(handler)
                 if self._run_id_to_watcher_dict[run_id].should_thread_exit.is_set():
                     del self._run_id_to_watcher_dict[run_id]
 
-    def __del__(self):
-        self.close()
-
-    def close(self):
+    def close(self) -> None:
         if not self._disposed:
             self._disposed = True
             with self._dict_lock:
                 for watcher_thread in self._run_id_to_watcher_dict.values():
                     if not watcher_thread.should_thread_exit.is_set():
                         watcher_thread.should_thread_exit.set()
                 for run_id in self._run_id_to_watcher_dict:
@@ -142,15 +148,15 @@
                 callback_with_cursor
                 for callback_with_cursor in self._callback_fn_list
                 if callback_with_cursor.callback != callback
             ]
             if not self._callback_fn_list:
                 self._should_thread_exit.set()
 
-    def run(self):
+    def run(self) -> None:
         """Polling function to update Observers with EventLogEntrys from Event Log DB.
         Wakes every POLLING_CADENCE &
             1. executes a SELECT query to get new EventLogEntrys
             2. fires each callback (taking into account the callback.cursor) on the new EventLogEntrys
         Uses max_index_so_far as a cursor in the DB to make sure that only new records are retrieved.
         """
         cursor = None
```

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.2rc3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/file_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/input_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/io_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.2rc3/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/migration/utils.py` & `dagster-1.7.2rc3/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/output_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.2rc3/dagster/_core/storage/partition_status_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,34 +343,39 @@
         asset_key, after_storage_id=after_storage_id
     )
 
     cursor = None
     if incomplete_materializations:
         to_fetch = list(set([run_id for run_id, _event_id in incomplete_materializations.values()]))
         finished_runs = {}
+        unfinished_runs = {}
+
         while to_fetch:
             chunk = to_fetch[:RUN_FETCH_BATCH_SIZE]
             to_fetch = to_fetch[RUN_FETCH_BATCH_SIZE:]
-            for r in instance.get_runs(
-                filters=RunsFilter(
-                    run_ids=chunk,
-                    statuses=FINISHED_STATUSES,
-                )
-            ):
-                finished_runs[r.run_id] = r.status
+            for r in instance.get_runs(filters=RunsFilter(run_ids=chunk)):
+                if r.status in FINISHED_STATUSES:
+                    finished_runs[r.run_id] = r.status
+                else:
+                    unfinished_runs[r.run_id] = r.status
+
         for partition, (run_id, event_id) in incomplete_materializations.items():
             if run_id in finished_runs:
                 status = finished_runs.get(run_id)
                 if status == DagsterRunStatus.FAILURE:
                     failed_partitions.add(partition)
-            else:
+            elif run_id in unfinished_runs:
                 in_progress_partitions.add(partition)
                 # If the run is not finished, keep track of the event id so we can check on it next time
                 if cursor is None or event_id < cursor:
                     cursor = event_id
+            else:
+                # Runs that are neither finished nor unfinished must have been deleted, so are
+                # considered neither in-progress nor failed
+                pass
 
     return (
         (
             partitions_def.empty_subset().with_partition_keys(
                 get_validated_partition_keys(
                     dynamic_partitions_store, partitions_def, failed_partitions
                 )
```

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/root.py` & `dagster-1.7.2rc3/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/runs/base.py` & `dagster-1.7.2rc3/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.2rc3/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/runs/migration.py` & `dagster-1.7.2rc3/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/runs/schema.py` & `dagster-1.7.2rc3/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,15 +926,19 @@
     def replace_job_origin(self, run: DagsterRun, job_origin: RemoteJobOrigin) -> None:
         new_label = job_origin.repository_origin.get_label()
         with self.connect() as conn:
             conn.execute(
                 RunsTable.update()
                 .where(RunsTable.c.run_id == run.run_id)
                 .values(
-                    run_body=serialize_value(run.with_job_origin(job_origin)),
+                    run_body=serialize_value(
+                        run.with_job_origin(job_origin).with_tags(
+                            {**run.tags, REPOSITORY_LABEL_TAG: new_label}
+                        )
+                    ),
                 )
             )
             conn.execute(
                 RunTagsTable.update()
                 .where(RunTagsTable.c.run_id == run.run_id)
                 .where(RunTagsTable.c.key == REPOSITORY_LABEL_TAG)
                 .values(value=new_label)
```

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.2rc3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/schedules/base.py` & `dagster-1.7.2rc3/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.2rc3/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.2rc3/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.2rc3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/sql.py` & `dagster-1.7.2rc3/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.2rc3/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/sqlite.py` & `dagster-1.7.2rc3/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.2rc3/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/tags.py` & `dagster-1.7.2rc3/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.2rc3/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.2rc3/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/system_config/objects.py` & `dagster-1.7.2rc3/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/telemetry.py` & `dagster-1.7.2rc3/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/telemetry_upload.py` & `dagster-1.7.2rc3/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/test_utils.py` & `dagster-1.7.2rc3/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.2rc3/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/config_schema.py` & `dagster-1.7.2rc3/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/dagster_type.py` & `dagster-1.7.2rc3/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/decorator.py` & `dagster-1.7.2rc3/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.2rc3/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.2rc3/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/python_dict.py` & `dagster-1.7.2rc3/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/python_set.py` & `dagster-1.7.2rc3/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/python_tuple.py` & `dagster-1.7.2rc3/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/types/transform_typing.py` & `dagster-1.7.2rc3/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/utility_ops.py` & `dagster-1.7.2rc3/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/utils.py` & `dagster-1.7.2rc3/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.2rc3/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/batch_asset_record_loader.py` & `dagster-1.7.2rc3/dagster/_core/workspace/batch_asset_record_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/config_schema.py` & `dagster-1.7.2rc3/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/context.py` & `dagster-1.7.2rc3/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/load.py` & `dagster-1.7.2rc3/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/load_target.py` & `dagster-1.7.2rc3/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/permissions.py` & `dagster-1.7.2rc3/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_core/workspace/workspace.py` & `dagster-1.7.2rc3/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/__init__.py` & `dagster-1.7.2rc3/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/asset_daemon.py` & `dagster-1.7.2rc3/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.2rc3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.2rc3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/backfill.py` & `dagster-1.7.2rc3/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/cli/__init__.py` & `dagster-1.7.2rc3/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/controller.py` & `dagster-1.7.2rc3/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/daemon.py` & `dagster-1.7.2rc3/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.2rc3/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.2rc3/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.2rc3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/sensor.py` & `dagster-1.7.2rc3/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/types.py` & `dagster-1.7.2rc3/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/utils.py` & `dagster-1.7.2rc3/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_daemon/workspace.py` & `dagster-1.7.2rc3/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_generate/download.py` & `dagster-1.7.2rc3/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_generate/generate.py` & `dagster-1.7.2rc3/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.2rc3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.2rc3/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.2rc3/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.2rc3/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/__init__.py` & `dagster-1.7.2rc3/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/client.py` & `dagster-1.7.2rc3/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/compile.py` & `dagster-1.7.2rc3/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/impl.py` & `dagster-1.7.2rc3/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/protos/api.proto` & `dagster-1.7.2rc3/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/proxy_server.py` & `dagster-1.7.2rc3/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/server.py` & `dagster-1.7.2rc3/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/server_watcher.py` & `dagster-1.7.2rc3/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/types.py` & `dagster-1.7.2rc3/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_grpc/utils.py` & `dagster-1.7.2rc3/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_loggers/__init__.py` & `dagster-1.7.2rc3/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_model/__init__.py` & `dagster-1.7.2rc3/dagster/_model/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,40 @@
+from functools import cached_property
 from typing import Any, Dict, Optional
 
-import pydantic
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from typing_extensions import Self
 
+from .pydantic_compat_layer import USING_PYDANTIC_2
+
 
 class DagsterModel(BaseModel):
     """Standardizes on Pydantic settings that are stricter than the default.
     - Frozen, to avoid complexity caused by mutation.
     - extra=forbid, to avoid bugs caused by accidentally constructing with the wrong arguments.
     - arbitrary_types_allowed, to allow non-model class params to be validated with isinstance.
+    - Avoid pydantic reading a cached property class as part of the schema.
     """
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
-    class Config:
-        extra = "forbid"
-        frozen = True
-        arbitrary_types_allowed = True
+    if USING_PYDANTIC_2:
+        model_config = ConfigDict(  # type: ignore
+            extra="forbid",
+            frozen=True,
+            arbitrary_types_allowed=True,
+            ignored_types=(cached_property,),
+        )
+    else:
+
+        class Config:
+            extra = "forbid"
+            frozen = True
+            arbitrary_types_allowed = True
+            keep_untouched = (cached_property,)
 
     def model_copy(self, *, update: Optional[Dict[str, Any]] = None) -> Self:
-        if pydantic.__version__ >= "2":
+        if USING_PYDANTIC_2:
             return super().model_copy(update=update)  # type: ignore
         else:
             return super().copy(update=update)
```

### Comparing `dagster-1.7.2rc2/dagster/_module_alias_map.py` & `dagster-1.7.2rc3/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_scheduler/scheduler.py` & `dagster-1.7.2rc3/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_scheduler/stale.py` & `dagster-1.7.2rc3/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_serdes/__init__.py` & `dagster-1.7.2rc3/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_serdes/config_class.py` & `dagster-1.7.2rc3/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_serdes/ipc.py` & `dagster-1.7.2rc3/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_serdes/serdes.py` & `dagster-1.7.2rc3/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_serdes/utils.py` & `dagster-1.7.2rc3/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_seven/__init__.py` & `dagster-1.7.2rc3/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_seven/abc.py` & `dagster-1.7.2rc3/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_seven/compat/pendulum.py` & `dagster-1.7.2rc3/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/__init__.py` & `dagster-1.7.2rc3/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/alert.py` & `dagster-1.7.2rc3/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/backoff.py` & `dagster-1.7.2rc3/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/cached_method.py` & `dagster-1.7.2rc3/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.2rc3/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/concurrency.py` & `dagster-1.7.2rc3/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/container.py` & `dagster-1.7.2rc3/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/dagster_type.py` & `dagster-1.7.2rc3/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/env.py` & `dagster-1.7.2rc3/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/error.py` & `dagster-1.7.2rc3/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/external.py` & `dagster-1.7.2rc3/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/forked_pdb.py` & `dagster-1.7.2rc3/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/hosted_user_process.py` & `dagster-1.7.2rc3/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/indenting_printer.py` & `dagster-1.7.2rc3/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/internal_init.py` & `dagster-1.7.2rc3/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/interrupts.py` & `dagster-1.7.2rc3/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/log.py` & `dagster-1.7.2rc3/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/merger.py` & `dagster-1.7.2rc3/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/net.py` & `dagster-1.7.2rc3/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/schedules.py` & `dagster-1.7.2rc3/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/tags.py` & `dagster-1.7.2rc3/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/temp_file.py` & `dagster-1.7.2rc3/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/test/__init__.py` & `dagster-1.7.2rc3/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/test/data_versions.py` & `dagster-1.7.2rc3/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.2rc3/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.2rc3/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.2rc3/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/timing.py` & `dagster-1.7.2rc3/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/typed_dict.py` & `dagster-1.7.2rc3/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/typing_api.py` & `dagster-1.7.2rc3/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/warnings.py` & `dagster-1.7.2rc3/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster/_utils/yaml_utils.py` & `dagster-1.7.2rc3/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.2rc2/dagster.egg-info/PKG-INFO` & `dagster-1.7.2rc3/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.2rc2
+Version: 1.7.2rc3
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.2rc2/dagster.egg-info/SOURCES.txt` & `dagster-1.7.2rc3/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 dagster/_config/type_printer.py
 dagster/_config/validate.py
 dagster/_config/pythonic_config/__init__.py
 dagster/_config/pythonic_config/attach_other_object_to_context.py
 dagster/_config/pythonic_config/config.py
 dagster/_config/pythonic_config/conversion_utils.py
 dagster/_config/pythonic_config/io_manager.py
-dagster/_config/pythonic_config/pydantic_compat_layer.py
 dagster/_config/pythonic_config/resource.py
 dagster/_config/pythonic_config/type_check_utils.py
 dagster/_config/pythonic_config/typing_utils.py
 dagster/_core/__init__.py
 dagster/_core/assets.py
 dagster/_core/code_pointer.py
 dagster/_core/debug.py
@@ -552,14 +551,15 @@
 dagster/_grpc/__generated__/api_pb2.py
 dagster/_grpc/__generated__/api_pb2.pyi
 dagster/_grpc/__generated__/api_pb2_grpc.py
 dagster/_grpc/protos/api.proto
 dagster/_legacy/__init__.py
 dagster/_loggers/__init__.py
 dagster/_model/__init__.py
+dagster/_model/pydantic_compat_layer.py
 dagster/_scheduler/__init__.py
 dagster/_scheduler/scheduler.py
 dagster/_scheduler/stale.py
 dagster/_serdes/__init__.py
 dagster/_serdes/config_class.py
 dagster/_serdes/errors.py
 dagster/_serdes/ipc.py
```

### Comparing `dagster-1.7.2rc2/dagster.egg-info/requires.txt` & `dagster-1.7.2rc3/dagster.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 structlog
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
-dagster-pipes==1.7.2rc2
+dagster-pipes==1.7.2rc3
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
```

### Comparing `dagster-1.7.2rc2/setup.py` & `dagster-1.7.2rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         'pywin32!=226; platform_system=="Windows"',
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
-        "dagster-pipes==1.7.2rc2",
+        "dagster-pipes==1.7.2rc3",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
```

