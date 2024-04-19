# Comparing `tmp/onnxscript-0.1.0.dev20240417.tar.gz` & `tmp/onnxscript-0.1.0.dev20240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240417.tar", last modified: Wed Apr 17 00:01:34 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240418.tar", last modified: Thu Apr 18 00:01:40 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240417.tar` & `onnxscript-0.1.0.dev20240418.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.240448 onnxscript-0.1.0.dev20240417/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.240448 onnxscript-0.1.0.dev20240417/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6153 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/protobuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.232448 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.244448 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.256448 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.236448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.236448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.256448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.256448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.260448 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.260448 onnxscript-0.1.0.dev20240417/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2338 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65860 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18651 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44268 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.264448 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.268448 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.272448 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46294 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.276448 onnxscript-0.1.0.dev20240417/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7995 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-17 00:01:34.000000 onnxscript-0.1.0.dev20240417/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-17 00:01:34.280448 onnxscript-0.1.0.dev20240417/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-17 00:01:07.000000 onnxscript-0.1.0.dev20240417/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:40.007262 onnxscript-0.1.0.dev20240418/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-18 00:01:40.007262 onnxscript-0.1.0.dev20240418/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.967261 onnxscript-0.1.0.dev20240418/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.971261 onnxscript-0.1.0.dev20240418/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.971261 onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11116 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8872 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6153 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/protobuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36193 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.971261 onnxscript-0.1.0.dev20240418/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.975262 onnxscript-0.1.0.dev20240418/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.963261 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.975262 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.987262 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.963261 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.963261 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.987262 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.987262 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/_flags.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/graph_building.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.991262 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.991262 onnxscript-0.1.0.dev20240418/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2338 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    66691 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2696 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10417 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2525 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18800 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1489 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    45188 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.991262 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.999262 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:39.999262 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4288 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:40.003262 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1424 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6698 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2165 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      686 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8844 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      756 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46294 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:40.003262 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1222 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5082 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1943 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:40.003262 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1628 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24688 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39591 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:40.003262 onnxscript-0.1.0.dev20240418/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:40.007262 onnxscript-0.1.0.dev20240418/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 00:01:40.007262 onnxscript-0.1.0.dev20240418/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10897 2024-04-18 00:01:39.000000 onnxscript-0.1.0.dev20240418/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7995 2024-04-18 00:01:39.000000 onnxscript-0.1.0.dev20240418/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-18 00:01:39.000000 onnxscript-0.1.0.dev20240418/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-18 00:01:39.000000 onnxscript-0.1.0.dev20240418/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-18 00:01:39.000000 onnxscript-0.1.0.dev20240418/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-18 00:01:40.007262 onnxscript-0.1.0.dev20240418/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-18 00:01:01.000000 onnxscript-0.1.0.dev20240418/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240417/LICENSE` & `onnxscript-0.1.0.dev20240418/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/PKG-INFO` & `onnxscript-0.1.0.dev20240418/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240417
+Version: 0.1.0.dev20240418
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240417/README.md` & `onnxscript-0.1.0.dev20240418/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/irbuilder.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/protobuilder.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/protobuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240418/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240418/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240418/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240418/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240418/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240418/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240418/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,38 +156,40 @@
         else:
             rich.print(text)
 
 
 class Tensor(TensorBase, _protocols.TensorProtocol, Generic[TArrayCompatible]):
     """An immutable concrete value."""
 
-    __slots__ = ("_raw", "_dtype", "_shape", "name", "doc_string")
+    __slots__ = ("_raw", "_dtype", "_shape", "name", "doc_string", "_metadata_props")
 
     def __init__(
         self,
         value: TArrayCompatible,
         dtype: _enums.DataType,
         *,
         shape: Shape | None = None,
         name: str = "",
         doc_string: str | None = None,
+        metadata_props: dict[str, str] | None = None,
     ) -> None:
         # NOTE: We should not do any copying here for performance reasons
         if not _compatible_with_numpy(value) and not _compatible_with_dlpack(value):
             raise TypeError(f"Expected an array compatible object, got {type(value)}")
         if not hasattr(value, "shape") and shape is None:
             raise ValueError(
                 f"Expected an object with a shape attribute, but {type(value)} does not have shape. "
                 "Please specify the shape explicitly."
             )
         self._raw = value
         self._dtype = dtype
         self._shape = Shape(getattr(value, "shape"))  # noqa: B009
         self.name = name
         self.doc_string = doc_string
+        self._metadata_props = metadata_props
 
     def __array__(self, dtype: Any = None) -> np.ndarray:
         # TODO(justinchuby): Support numpy unsupported types
         if isinstance(self._raw, np.ndarray) or _compatible_with_numpy(self._raw):
             return self._raw.__array__(dtype)
         assert _compatible_with_dlpack(
             self._raw
@@ -232,14 +234,19 @@
         """
         # TODO(justinchuby): Support DLPack
         array = self.numpy()
         if not IS_LITTLE_ENDIAN:
             return array.view(array.dtype.newbyteorder("<")).tobytes()
         return array.tobytes()
 
+    def metadata_props(self) -> dict[str, str]:
+        if self._metadata_props is None:
+            self._metadata_props = {}
+        return self._metadata_props
+
 
 class ExternalTensor(TensorBase, _protocols.TensorProtocol):
     """An immutable concrete tensor with its data store on disk.
 
     This class uses memory mapping to avoid loading the tensor into memory,
     when the data type is supported by numpy. Otherwise, the tensor is loaded
     into memory lazily when accessed.
@@ -257,48 +264,52 @@
         path: The path to the data file. This can be a relative path or an absolute path.
         offset: The offset in bytes from the start of the file.
         length: The length of the data in bytes.
         dtype: The data type of the tensor.
         shape: The shape of the tensor.
         name: The name of the tensor. It must be specified.
         doc_string: The documentation string.
+        metadata_props: The metadata properties.
     """
 
     __slots__ = (
         "_path",
         "_offset",
         "_length",
         "_dtype",
         "_shape",
         "name",
         "doc_string",
         "_array",
         "raw",
+        "_metadata_props",
     )
 
     def __init__(
         self,
         path: os.PathLike | str,
         offset: int | None,
         length: int | None,
         dtype: _enums.DataType,
         *,
         shape: Shape,
         name: str,
         doc_string: str | None = None,
+        metadata_props: dict[str, str] | None = None,
     ) -> None:
         self._path = path
         self._offset: int | None = offset
         self._length: int | None = length
         self._dtype: _enums.DataType = dtype
         self.name: str = name  # mutable
         self._shape: Shape = shape
         self.doc_string: str | None = doc_string  # mutable
         self._array: np.ndarray | None = None
         self.raw: mmap.mmap | None = None
+        self._metadata_props = metadata_props
 
     @property
     def path(self) -> str | os.PathLike:
         # Immutable
         return self._path
 
     @property
@@ -367,14 +378,20 @@
         if self.raw is None:
             self._load()
         assert self.raw is not None
         offset = self._offset or 0
         length = self._length or self.nbytes
         return self.raw[offset : offset + length]
 
+    @property
+    def metadata_props(self) -> dict[str, str]:
+        if self._metadata_props is None:
+            self._metadata_props = {}
+        return self._metadata_props
+
 
 class Dimension(_protocols.DimensionProtocol, _display.PrettyPrintable):
     __slots__ = ("_value", "_denotation")
 
     def __init__(self, value: int | str | None, denotation: str | None = None) -> None:
         self._value = value
         self._denotation = denotation
@@ -1151,28 +1168,29 @@
         outputs: Sequence[Value],
         *,
         nodes: Iterable[Node],
         initializers: Sequence[_protocols.TensorProtocol] = (),
         doc_string: str | None = None,
         opset_imports: dict[str, int] | None = None,
         name: str | None = None,
+        metadata_props: dict[str, str] | None = None,
     ):
         self.name = name
 
         # Private fields that are not to be accessed by any other classes
         self._inputs = list(inputs)
         self._outputs = list(outputs)
         for initializer in initializers:
             if initializer.name is None:
                 raise ValueError(f"Initializer must have a name: {initializer}")
         self._initializers = {tensor.name: tensor for tensor in initializers}
         self._doc_string = doc_string
         self._opset_imports = opset_imports or {}
         self._metadata: _metadata.MetadataStore | None = None
-        self._metadata_props: dict[str, str] | None = None
+        self._metadata_props: dict[str, str] | None = metadata_props
         self._nodes: _linked_list.DoublyLinkedSet[Node] = _linked_list.DoublyLinkedSet()
         # Be sure the initialize the name authority before extending the nodes
         # because it is used to name the nodes and their outputs
         self._name_authority = _name_authority.NameAuthority()
         # Call self.extend not self._nodes.extend so the graph reference is added to the nodes
         self.extend(nodes)
 
@@ -1530,25 +1548,26 @@
         ir_version: int,
         producer_name: str | None = None,
         producer_version: str | None = None,
         domain: str | None = None,
         model_version: int | None = None,
         doc_string: str | None = None,
         functions: Sequence[Function] = (),
+        meta_data_props: dict[str, str] | None = None,
     ) -> None:
         self.graph: Graph | GraphView = graph  # type: ignore[assignment]
         self.ir_version = ir_version
         self.producer_name = producer_name
         self.producer_version = producer_version
         self.domain = domain
         self.model_version = model_version
         self.doc_string = doc_string
         self._functions = {func.identifier(): func for func in functions}
         self._metadata: _metadata.MetadataStore | None = None
-        self._metadata_props: dict[str, str] | None = None
+        self._metadata_props: dict[str, str] | None = meta_data_props
 
     @property
     def functions(self) -> dict[_protocols.OperatorIdentifier, Function]:
         return self._functions
 
     @property
     def opset_imports(self) -> dict[str, int]:
@@ -1613,22 +1632,23 @@
         name: str,
         overload: str = "",
         *,
         # Ensure the inputs and outputs of the function belong to a graph
         # and not from an outer scope
         graph: Graph,
         attributes: Sequence[Attr],
+        metadata_props: dict[str, str] | None = None,
     ) -> None:
         self._domain = domain
         self._name = name
         self._overload = overload
         self._graph = graph
         self._attributes = OrderedDict((attr.name, attr) for attr in attributes)
         self._metadata: _metadata.MetadataStore | None = None
-        self._metadata_props: dict[str, str] | None = None
+        self._metadata_props: dict[str, str] | None = metadata_props
 
     def identifier(self) -> _protocols.OperatorIdentifier:
         return self.domain, self.name, self.overload
 
     @property
     def name(self) -> str:
         return self._name
```

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import typing
 from typing import (
     AbstractSet,
     Any,
     Iterable,
     Iterator,
     Mapping,
+    MutableMapping,
     MutableSequence,
     OrderedDict,
     Protocol,
     Sequence,
     Tuple,
     Union,
 )
@@ -93,14 +94,15 @@
     """
 
     name: str
     shape: ShapeProtocol
     dtype: _enums.DataType
     doc_string: str | None
     raw: Any
+    metadata_props: MutableMapping[str, str]
 
     @property
     def size(self) -> int: ...
 
     @property
     def nbytes(self) -> int: ...
 
@@ -144,16 +146,16 @@
         type: The type of the value.
         metadata_props: Metadata.
     """
 
     name: str
     shape: ShapeProtocol | None
     type: TypeProtocol | None
-    metadata_props: Mapping[str, str]
-    meta: Mapping[str, Any]
+    metadata_props: MutableMapping[str, str]
+    meta: MutableMapping[str, Any]
 
     def producer(self) -> NodeProtocol | None:
         """The node that produces this value."""
         ...
 
     def index(self) -> int | None:
         """The index of the output of the node that produces this value."""
@@ -213,16 +215,16 @@
     op_type: str
     overload: str
     inputs: Sequence[ValueProtocol]
     outputs: Sequence[ValueProtocol]
     attributes: OrderedDict[str, AttributeProtocol | ReferenceAttributeProtocol]
     version: int | None
     doc_string: str | None
-    metadata_props: Mapping[str, str]
-    meta: Mapping[str, Any]
+    metadata_props: MutableMapping[str, str]
+    meta: MutableMapping[str, Any]
 
     def replace_input_with(self, index: int, value: ValueProtocol | None) -> None:
         """Set the input at the given index to the given value, replacing the original value."""
         ...
 
 
 @typing.runtime_checkable
@@ -253,16 +255,16 @@
     name: str | None
     inputs: MutableSequence[ValueProtocol]
     outputs: MutableSequence[ValueProtocol]
     nodes: Sequence[NodeProtocol]
     initializers: Mapping[str, TensorProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
-    metadata_props: Mapping[str, str]
-    meta: Mapping[str, Any]
+    metadata_props: MutableMapping[str, str]
+    meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[NodeProtocol]: ...
     def __reversed__(self) -> Iterator[NodeProtocol]: ...
 
     # Mutation methods
@@ -314,16 +316,16 @@
     name: str | None
     inputs: Sequence[ValueProtocol]
     outputs: Sequence[ValueProtocol]
     nodes: Sequence[NodeProtocol]
     initializers: Mapping[str, TensorProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
-    metadata_props: Mapping[str, str]
-    meta: Mapping[str, Any]
+    metadata_props: MutableMapping[str, str]
+    meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[NodeProtocol]: ...
     def __reversed__(self) -> Iterator[NodeProtocol]: ...
 
 
@@ -352,16 +354,16 @@
     producer_version: str | None
     domain: str | None
     model_version: int | None
     doc_string: str | None
     functions: Mapping[str, FunctionProtocol]
     # TODO(justinchuby): Add training_info
     opset_imports: Mapping[str, int]
-    metadata_props: Mapping[str, str]
-    meta: Mapping[str, Any]
+    metadata_props: MutableMapping[str, str]
+    meta: MutableMapping[str, Any]
 
 
 @typing.runtime_checkable
 class AttributeProtocol(Protocol):
     """Protocol for ONNX attributes.
 
     Attributes:
@@ -514,16 +516,16 @@
     overload: str
     inputs: Sequence[ValueProtocol]
     attributes: OrderedDict[str, AttributeProtocol]
     outputs: Sequence[ValueProtocol]
     doc_string: str
     opset_imports: Mapping[str, int]
     nodes: Sequence[NodeProtocol]
-    metadata_props: Mapping[str, str]
-    meta: Mapping[str, Any]
+    metadata_props: MutableMapping[str, str]
+    meta: MutableMapping[str, Any]
 
     def __getitem__(self, index: int) -> NodeProtocol: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[NodeProtocol]: ...
     def __reversed__(self) -> Iterator[NodeProtocol]: ...
     def identifier(self) -> OperatorIdentifier:
         """Return the unique identifier of the function."""
```

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/convenience.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240418/onnxscript/ir/serde.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
 
 class TensorProtoTensor(_core.TensorBase):
     """A tensor initialized from a tensor proto."""
 
     def __init__(self, proto: onnx.TensorProto) -> None:
         self._proto = proto
+        self._metadata_props: dict[str, str] = deserialize_metadata_props(proto.metadata_props)
 
     @property
     def name(self) -> str:
         return self._proto.name
 
     @property
     def shape(self) -> _core.Shape:
@@ -122,14 +123,18 @@
         """Return the tensor as a byte string conformed to the ONNX specification, in little endian."""
         if not self._proto.HasField("raw_data"):
             raise ValueError(
                 "Cannot convert non-raw tensor to bytes. Use a specialized tensor class like FloatDataTensor instead."
             )
         return self._proto.raw_data
 
+    @property
+    def metadata_props(self) -> dict[str, str]:
+        return self._metadata_props
+
 
 class FloatDataTensor(TensorProtoTensor):  # pylint: disable=too-many-ancestors
     """Specialized tensor for float data.
 
     When serializing, the data can be stored in the float_data field.
     """
 
@@ -293,14 +298,15 @@
         ir_version=proto.ir_version,
         producer_name=_get_field(proto, "producer_name"),
         producer_version=_get_field(proto, "producer_version"),
         domain=_get_field(proto, "domain"),
         model_version=_get_field(proto, "model_version"),
         doc_string=_get_field(proto, "doc_string"),
         functions=functions,
+        meta_data_props=deserialize_metadata_props(proto.metadata_props),
     )
 
     # Handle experimental value info for functions created by the dynamo exporter in IR version 9
     if model.ir_version < _FUNCTION_VALUE_INFO_SUPPORTED_VERSION:
         _deserialized_experimental_value_info_for_function_ir9(
             model.functions, proto.graph.value_info
         )
@@ -412,14 +418,15 @@
     return _core.Graph(
         inputs,
         outputs,
         nodes=nodes,
         initializers=initializers,
         doc_string=_get_field(proto, "doc_string"),
         name=_get_field(proto, "name"),
+        metadata_props=deserialize_metadata_props(proto.metadata_props),
     )
 
 
 def deserialize_function(proto: onnx.FunctionProto) -> _core.Function:
     inputs = [_core.Input(name) for name in proto.input]
     values: dict[str, _core.Value] = {v.name: v for v in inputs}  # type: ignore[misc]
     value_info = {info.name: info for info in getattr(proto, "value_info", [])}
@@ -447,25 +454,27 @@
     ]
     return _core.Function(
         domain=proto.domain,
         name=proto.name,
         overload=getattr(proto, "overload", ""),
         graph=graph,
         attributes=typing.cast(List[_core.Attr], attributes),
+        metadata_props=deserialize_metadata_props(proto.metadata_props),
     )
 
 
 def deserialize_value_info_proto(
     proto: onnx.ValueInfoProto, value: _core.Value | None
 ) -> _core.Value:
     if value is None:
         value = _core.Value(None, index=None)
         value.name = proto.name
     value.shape = deserialize_type_proto_for_shape(proto.type)
     value.type = deserialize_type_proto_for_type(proto.type)
+    value.metadata_props.update(deserialize_metadata_props(proto.metadata_props))
     return value
 
 
 def deserialize_type_proto_for_shape(proto: onnx.TypeProto) -> _core.Shape | None:
     if proto.HasField("tensor_type"):
         if (shape_proto := _get_field(proto.tensor_type, "shape")) is None:
             return None
@@ -532,48 +541,53 @@
     denotation = _get_field(proto, "denotation")
     if value_field is not None:
         return _core.Dimension(getattr(proto, value_field), denotation=denotation)
     return _core.Dimension(None)
 
 
 def deserialize_tensor(
-    tensor: onnx.TensorProto, base_path: str | os.PathLike = ""
+    proto: onnx.TensorProto, base_path: str | os.PathLike = ""
 ) -> _protocols.TensorProtocol:
     # TODO: Sanitize base_path
-    if tensor.data_location == onnx.TensorProto.EXTERNAL:
-        external_info = onnx.external_data_helper.ExternalDataInfo(tensor)
+    if proto.data_location == onnx.TensorProto.EXTERNAL:
+        external_info = onnx.external_data_helper.ExternalDataInfo(proto)
         return _core.ExternalTensor(
             path=os.path.join(base_path, external_info.location),
             offset=external_info.offset,
             length=external_info.length,
-            dtype=_enums.DataType(tensor.data_type),
-            name=tensor.name,
-            shape=_core.Shape(tensor.dims),
-            doc_string=tensor.doc_string,
+            dtype=_enums.DataType(proto.data_type),
+            name=proto.name,
+            shape=_core.Shape(proto.dims),
+            doc_string=proto.doc_string,
+            metadata_props=deserialize_metadata_props(proto.metadata_props),
         )
     # Check for the raw_data filed first. The rest of the repeating fields can be
     # empty and still valid, so we don't need to check their length
     # For example, int32_data can be empty and still be a valid tensor.
-    if tensor.HasField("raw_data"):
-        return TensorProtoTensor(tensor)
-    if tensor.data_type in FloatDataTensor.compatible_types:
-        return FloatDataTensor(tensor)
-    if tensor.data_type in Int32DataTensor.compatible_types:
-        return Int32DataTensor(tensor)
-    if tensor.data_type in Int64DataTensor.compatible_types:
-        return Int64DataTensor(tensor)
-    if tensor.data_type in DoubleDataTensor.compatible_types:
-        return DoubleDataTensor(tensor)
-    if tensor.data_type in UInt64DataTensor.compatible_types:
-        return UInt64DataTensor(tensor)
+    if proto.HasField("raw_data"):
+        return TensorProtoTensor(proto)
+    if proto.data_type in FloatDataTensor.compatible_types:
+        return FloatDataTensor(proto)
+    if proto.data_type in Int32DataTensor.compatible_types:
+        return Int32DataTensor(proto)
+    if proto.data_type in Int64DataTensor.compatible_types:
+        return Int64DataTensor(proto)
+    if proto.data_type in DoubleDataTensor.compatible_types:
+        return DoubleDataTensor(proto)
+    if proto.data_type in UInt64DataTensor.compatible_types:
+        return UInt64DataTensor(proto)
     raise ValueError(
-        f"TensorProto(name={tensor.name}) does not have any data fields set and is not an external tensor."
+        f"TensorProto(name={proto.name}) does not have any data fields set and is not an external tensor."
     )
 
 
+def deserialize_metadata_props(proto: Sequence[onnx.StringStringEntryProto]) -> dict[str, str]:
+    return {entry.key: entry.value for entry in proto}
+
+
 def deserialize_attribute(proto: onnx.AttributeProto) -> _core.Attr | _core.RefAttr:
     return _deserialize_attribute(proto, [])
 
 
 def _deserialize_attribute(
     proto: onnx.AttributeProto, scoped_values: list[dict[str, _core.Value]]
 ) -> _core.Attr | _core.RefAttr:
@@ -977,14 +991,16 @@
 
 def serialize_tensor_into(
     tensor_proto: onnx.TensorProto, from_: _protocols.TensorProtocol
 ) -> None:
     if isinstance(from_, TensorProtoTensor):
         # Directly copy from the tensor proto if it is available
         tensor_proto.CopyFrom(from_.raw)
+        if from_.metadata_props:
+            _serialize_metadata_props_into(tensor_proto.metadata_props, from_.metadata_props)
         return
 
     tensor_proto.name = from_.name
     if from_.doc_string:
         tensor_proto.doc_string = from_.doc_string
     tensor_proto.data_type = from_.dtype.value
     tensor_proto.dims.extend(from_.shape.numpy())
@@ -998,14 +1014,15 @@
         }.items():
             if v is not None:
                 entry = tensor_proto.external_data.add()
                 entry.key = k
                 entry.value = str(v)
     else:
         tensor_proto.raw_data = from_.tobytes()
+    _serialize_metadata_props_into(tensor_proto.metadata_props, from_.metadata_props)
 
 
 def serialize_attribute(attribute: _protocols.AttributeProtocol) -> onnx.AttributeProto:
     attribute_proto = onnx.AttributeProto()
     serialize_attribute_into(attribute_proto, from_=attribute)
     return attribute_proto
```

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240418/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/main.py` & `onnxscript-0.1.0.dev20240418/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240418/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240418/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240418/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240418/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240418/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240418/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240418/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240418/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240418/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240418/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript/values.py` & `onnxscript-0.1.0.dev20240418/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240418/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240417
+Version: 0.1.0.dev20240418
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240417/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240418/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/pyproject.toml` & `onnxscript-0.1.0.dev20240418/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240417/setup.py` & `onnxscript-0.1.0.dev20240418/setup.py`

 * *Files identical despite different names*

